# Comparing `tmp/perming-1.3.0-py3-none-any.whl.zip` & `tmp/perming-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13155 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-03 08:11 perming/__init__.py
+Zip file size: 13221 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-13 03:59 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    20745 b- defN 23-Jul-03 08:32 perming/_utils.py
+-rw-rw-rw-  2.0 fat    21066 b- defN 23-Jul-13 04:36 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
--rw-rw-rw-  2.0 fat    14049 b- defN 23-Jul-03 08:59 perming/common.py
--rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-03 09:34 perming/general.py
--rw-rw-rw-  2.0 fat     8772 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      746 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/RECORD
-10 files, 51648 bytes uncompressed, 11901 bytes compressed:  77.0%
+-rw-rw-rw-  2.0 fat    13988 b- defN 23-Jul-13 04:45 perming/common.py
+-rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-13 04:43 perming/general.py
+-rw-rw-rw-  2.0 fat     8772 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      746 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/RECORD
+10 files, 51908 bytes uncompressed, 11967 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.3.0.dist-info/METADATA
+Filename: perming-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.3.0.dist-info/WHEEL
+Filename: perming-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.3.0.dist-info/top_level.txt
+Filename: perming-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.3.0.dist-info/RECORD
+Filename: perming-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -23,8 +23,8 @@
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler,
     'Multi-outputs': Ranker
 }
 
-__version__ = '1.3.0'
+__version__ = '1.3.1'
```

## perming/_utils.py

```diff
@@ -30,25 +30,26 @@
     :param num_classes: int, total number of correct label categories.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation:, activation configured by Classfier. default: torch.nn.ReLU().
     '''
     def __init__(self, input_: int, num_classes: int, hidden_layer_sizes: Tuple[int], activation) -> None:
         super(MLP, self).__init__()
         self.squeeze: bool = False if num_classes > 1 else True
-        if hidden_layer_sizes:
+        if hidden_layer_sizes: # for linear indivisible datasets
             assert hidden_layer_sizes[0] > 0, "Please ensure any layer of hidden_layer_sizes > 0"
             model_layers, hidden_length = OrderedDict(), len(hidden_layer_sizes)
             model_layers['Linear0'] = torch.nn.Linear(input_, hidden_layer_sizes[0])
             model_layers['Activation0'] = activation
             for index in range(1, hidden_length):
                 assert hidden_layer_sizes[index] > 0, "Please ensure any layer of hidden_layer_sizes > 0"
-                linear_, activation_ = "Linear" + str(index), "Activation" + str(index)
+                ind_str = str(index)
+                linear_, activation_ = 'Linear'.join(('', ind_str)), 'Activation'.join(('', ind_str))
                 model_layers[linear_] = torch.nn.Linear(hidden_layer_sizes[index - 1], hidden_layer_sizes[index])
                 model_layers[activation_] = activation
-            model_layers["Linear" + str(hidden_length)] = torch.nn.Linear(hidden_layer_sizes[hidden_length - 1], num_classes)
+            model_layers['Linear'.join(('', str(hidden_length)))] = torch.nn.Linear(hidden_layer_sizes[hidden_length - 1], num_classes)
             self.mlp = torch.nn.Sequential(model_layers)
         else:
             self.mlp = torch.nn.Linear(input_, num_classes)
 
     def forward(self, x):
         output = self.mlp(x)
         return output.squeeze(-1) if self.squeeze else output
@@ -81,29 +82,29 @@
 
         assert input_ > 0, 'BaseModel need samples with dataset features named input_ > 0.'
         assert num_classes > 0, 'Supervised learning problems with num_classes ranges from (1, 2, 3, ...).'
         assert batch_size > 0, 'Batch size initialized with int value mostly 2^n(n=1, 2, 3), like 64, 128, 256.'
         assert learning_rate_init > 0 and learning_rate_init < 1.0, 'Please assert learning rate initialized value in (0, 1.0).'
         self.input: int = input_
         self.num_classes: int = num_classes
-        self.activation = activation
+        self.activation = activation # function activate high-dimensional features
         self.device = device # device configuration
-        self.criterion = criterion
+        self.criterion = criterion # criterion with classification & torch.long, regression & torch.float, and multi-outputs & roc
         self.batch_size: int = batch_size
         self.lr: float = learning_rate_init
         self.model = MLP(self.input, self.num_classes, hidden_layer_sizes, self.activation).to(self.device)
         if parse_torch_version(torch.__version__)[0] >= ['2', '0', '0']:
             self.model = torch.compile(self.model)
         self.solver = self._solver(solver)
         self.lr_scheduler = self._scheduler(lr_scheduler)
 
     def _solver(self, solver: str):
         '''
         Configure Optimizer with `solver`.
-        :param solver: str, "sgd", "momentum", "adam", "adagrad", "rmsprop". default: adam.
+        :param solver: str, 'sgd', 'momentum', 'adam', 'adagrad', 'rmsprop'. default: adam.
         '''
         if solver == 'sgd':
             return torch.optim.SGD(self.model.parameters(), lr=self.lr)
         elif solver == 'adam':
             return torch.optim.Adam(self.model.parameters(), lr=self.lr, betas=(0.9, 0.99))
         elif solver == 'momentum':
             return torch.optim.SGD(self.model.parameters(), lr=self.lr, momentum=0.9, nesterov=True)
@@ -113,15 +114,15 @@
             return torch.optim.RMSprop(self.model.parameters(), lr=self.lr, alpha=0.9)
         else:
             raise ValueError("Optimizer Configuration Supports Options: sgd, momentum, adam, adagrad, rmsprop.")
 
     def _scheduler(self, lr_scheduler: Optional[str]):
         '''
         Configure Learning Rate Scheduler with `lr_scheduler`.
-        :param lr_scheduler: str, "exponential_lr", "step_lr", "cosine_annealing_lr". default: None.
+        :param lr_scheduler: str, 'exponential_lr', 'step_lr', 'cosine_annealing_lr'. default: None.
         '''
         if lr_scheduler != None:
             if lr_scheduler == 'exponential_lr':
                 return torch.optim.lr_scheduler.ExponentialLR(self.solver, gamma=0.1)
             elif lr_scheduler == 'step_lr':
                 return torch.optim.lr_scheduler.StepLR(self.solver, step_size=2, gamma=0.1)
             elif lr_scheduler == 'cosine_annealing_lr':
@@ -138,15 +139,15 @@
             'torch -v': torch.__version__,
             'criterion': self.criterion,
             'batch_size': self.batch_size,
             'solver': self.solver,
             'lr_scheduler': self.lr_scheduler,
             'device': self.device,
         })
-    
+
     def data_loader(self, 
                     features: TabularData, 
                     target: TabularData, 
                     ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}, 
                     worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1},
                     random_seed: Optional[int]=None) -> None:
         '''
@@ -165,26 +166,26 @@
         assert isinstance(target, TabularData), "Please ensure target format at numpy.ndarray noted as TabularData."
         target_dtype = str(target.dtype) # __str__
         is_int_type, is_float_type = "int" in target_dtype, "float" in target_dtype
         self.is_target_2d = isinstance(target[0], TabularData) # judge target is 2d matrix.
         if self.is_target_2d: # (n_samples, n_outputs)
             assert target.shape[1] == self.num_classes, "Please ensure target with (n_samples, n_outputs=num_classes)."
             assert is_int_type or is_float_type, "Please ensure target.dtype in any int or float type of numpy.dtype."
-            roc = not is_int_type and is_float_type
+            roc: bool = not is_int_type and is_float_type
         else: # (n_samples,)
             if self.num_classes >= 2:
                 self.unique = numpy.unique(target) # int indexes -> any class with single value noted
                 assert len(self.unique) == self.num_classes, "Please ensure `num_classes` is equal to `len(numpy.unique(labels))`."
                 self.indices = dict(zip(self.unique, range(self.num_classes))) # original classes -> int indexes
                 target = numpy.array([self.indices[value] for value in target], dtype=numpy.int8) # adjust int8 -> any int dtype
             else:
                 assert is_float_type, "Please ensure target.dtype in any float type of numpy.dtype." # continuous
             roc: bool = self.model.squeeze
         train_, test_, val_ = train_test_val_split(features, target, ratio_set, random_seed)
-        self.train_loader = torch.utils.data.DataLoader(TabularDataset(train_['features'], train_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['train'], )
+        self.train_loader = torch.utils.data.DataLoader(TabularDataset(train_['features'], train_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['train'])
         self.test_loader = torch.utils.data.DataLoader(TabularDataset(test_['features'], test_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['test'])
         self.val_loader = torch.utils.data.DataLoader(TabularDataset(val_['features'], val_['target'], roc), batch_size=self.batch_size, shuffle=False, num_workers=worker_set['val'])
 
     def train_val(self, 
                   num_epochs: int=2, 
                   interval: int=100, 
                   backend: str="threading", 
@@ -214,30 +215,31 @@
 
                 # backward and optimize
                 self.solver.zero_grad()
                 self.train_loss.backward()
                 _ = self.solver.step() if self.lr_scheduler == None else self.lr_scheduler.step()
 
                 # validation with val_container
-                self.val_loss = 0
+                self.val_loss = 0 # int value at cpu
                 with parallel_backend(backend, n_jobs=n_jobs):
                     for val_set in self.val_container:
-                        outputs_val = self.model(val_set[0].to(self.device))
+                        outputs_val = self.model(val_set[0].to(self.device)) # return value from cuda
                         self.val_loss += self.criterion(outputs_val, val_set[1].to(self.device))
                 self.val_loss /= val_length
 
                 # console print
                 if (i + 1) % interval == 0:
                     print ('Epoch [{}/{}], Step [{}/{}], Training Loss: {:.4f}, Validation Loss: {:.4f}'.format(epoch+1, num_epochs, i+1, total_step, self.train_loss.item(), self.val_loss.item()))
 
     def test(self, 
              sort_by: str='accuracy',
              sort_state: bool=True):
         '''
-        Test with Initialized Configuration. `accuracy > 0`, 'correct_class != None' and keywords only appears when `num_classes >= 2`.
+        Test with Initialized Configuration. `accuracy > 0`, 'correct_class != None'
+        Configured keywords only work when `not self.is_target_2d and num_classes >= 2`.
         :param sort_by: str, 'accuracy', 'numbers', 'num-total'. default: 'accuracy'.
         :param sort_state: bool, whether to use descending order when sorting. default: True.
         '''
         with torch.no_grad():
             self.test_loss, test_loader_step, correct = 0, len(self.test_loader), 0
             test_total = test_loader_step * self.batch_size
             self.correct_class = dict.fromkeys(self.unique, [0, 0]) if not self.is_target_2d and self.num_classes >= 2 else None
@@ -250,16 +252,16 @@
                     for index, value in enumerate(predicted):
                         self.correct_class[self.unique[value]][1] += 1 # record total numbers of each class
                         self.correct_class[self.unique[value]][0] += (value == target[index]).item() # record total true numbers of each class
                     correct += (predicted == target).sum().item()
                 self.test_loss += self.criterion(outputs, target)
             self.test_loss /= test_loader_step
             print('loss of {0} on the {1} test dataset: {2}. accuracy: {3:.4f} %'.format(self.__class__.__name__, test_total, self.test_loss.item(), 100 * correct / test_total))
-        return OrderedDict(self._packing(sort_by, sort_state))
-    
+        return OrderedDict(self._pack_info(sort_by, sort_state))
+
     def save(self, show: bool=True, dir: str='./model') -> None:
         '''
         Save Model Checkpoint with Box, Regressier, Binarier, Multipler, and Ranker.
         :param show: bool, whether to show `model.state_dict()`. default: True.
         :param dir: str, model save to dir. default: './model'.
         '''
         if show:
@@ -273,15 +275,15 @@
         :param dir: str, model load from dir. default: './model'.
         '''
         params = torch.load(dir)
         self.model.load_state_dict(params)
         if show:
             print(self.model.state_dict())
 
-    def _packing(self, by: str, state: bool) -> Dict[str, Any]:
+    def _pack_info(self, by: str, state: bool) -> Dict[str, Any]:
         '''
         Pack Test Returned Data including `correct_class` and returned result of `sorted`.
         :param by: str, choose which way to sort the order of 'correct_class'.
         :param state: bool, choose the state when `correct_class` is sorting.
         '''
         loss_, classify, regress, outputs = {
             'loss': {'train': self.train_loss.item(),
```

## perming/common.py

```diff
@@ -25,26 +25,26 @@
                  batch_size: int=32, 
                  learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
 
         super(Regressier, self).__init__(input_, 
                                          1, 
                                          hidden_layer_sizes, 
-                                         torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                         torch.device('cuda' if torch.cuda.is_available() else 'cpu'), 
                                          self._activate(activation), 
                                          self._criterion(criterion), 
                                          solver, 
                                          batch_size, 
                                          learning_rate_init, 
                                          lr_scheduler)
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace=True`.
-        :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu". default: 'relu'.
+        :param activation: str, 'relu', 'rrelu', 'leaky_relu', 'elu', 'celu'. default: 'relu'.
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'rrelu':
             return torch.nn.RReLU(inplace=True)
         elif activation == 'leaky_relu':
             return torch.nn.LeakyReLU(inplace=True)
@@ -54,15 +54,15 @@
             return torch.nn.CELU(inplace=True)
         else:
             raise ValueError("Activation Function Supports Options: relu, rrelu, leaky_relu, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "MSELoss", "L1Loss", "SmoothL1Loss", "KLDivLoss". default: MSELoss.
+        :param criterion: str, 'MSELoss', 'L1Loss', 'SmoothL1Loss', 'KLDivLoss'. default: MSELoss.
         '''
         if criterion == 'MSELoss':
             return torch.nn.MSELoss()
         elif criterion == 'L1Loss':
             return torch.nn.L1Loss()
         elif criterion == 'SmoothL1Loss':
             return torch.nn.SmoothL1Loss()
@@ -93,26 +93,26 @@
                  batch_size: int=32, 
                  learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
 
         super(Binarier, self).__init__(input_, 
                                        2, 
                                        hidden_layer_sizes, 
-                                       torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                       torch.device('cuda' if torch.cuda.is_available() else 'cpu'), 
                                        self._activate(activation), 
                                        self._criterion(criterion), 
                                        solver, 
                                        batch_size, 
                                        learning_rate_init, 
                                        lr_scheduler)
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace=True`.
-        :param activation: str, "relu", "tanh", "sigmoid", "rrelu", "leaky_relu", "elu", "celu".
+        :param activation: str, 'relu', 'tanh', 'sigmoid', 'rrelu', 'leaky_relu', 'elu', 'celu'.
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'tanh':
             return torch.nn.Tanh()
         elif activation == 'sigmoid':
             return torch.nn.Sigmoid()
@@ -126,15 +126,15 @@
             return torch.nn.CELU(inplace=True)
         else:
             raise ValueError("Activation Function Supports Options: relu, tanh, sigmoid, rrelu, leaky_relu, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "BCELoss", "BCEWithLogitsLoss". default: BCELoss.
+        :param criterion: str, 'BCELoss', 'BCEWithLogitsLoss'. default: BCELoss.
         '''
         if criterion == 'BCELoss':
             return torch.nn.BCELoss()
         elif criterion == 'BCEWithLogitsLoss':
             return torch.nn.BCEWithLogitsLoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: BCELoss, BCEWithLogitsLoss.")
@@ -164,27 +164,27 @@
                  batch_size: int=32, 
                  learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
 
         super(Mutipler, self).__init__(input_, 
                                        num_classes, 
                                        hidden_layer_sizes, 
-                                       torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                       torch.device('cuda' if torch.cuda.is_available() else 'cpu'), 
                                        self._activate(activation), 
                                        self._criterion(criterion), 
                                        solver, 
                                        batch_size, 
                                        learning_rate_init, 
                                        lr_scheduler)
         assert num_classes >= 2, "The predefined options of Multipler are more suitable for Multi-classification."
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace=True`.
-        :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu".
+        :param activation: str, 'relu', 'rrelu', 'leaky_relu', 'elu', 'celu'.
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'rrelu':
             return torch.nn.RReLU(inplace=True)
         elif activation == 'leaky_relu':
             return torch.nn.LeakyReLU(inplace=True)
@@ -194,15 +194,15 @@
             return torch.nn.CELU(inplace=True)
         else:
             raise ValueError("Activation Function Supports Options: relu, rrelu, leaky_relu, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "CrossEntropyLoss", "NLLLoss".
+        :param criterion: str, 'CrossEntropyLoss', 'NLLLoss'.
         '''
         if criterion == 'CrossEntropyLoss':
             return torch.nn.CrossEntropyLoss()
         elif criterion == 'NLLLoss':
             return torch.nn.NLLLoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: CrossEntropyLoss, NLLLoss.")
@@ -232,15 +232,15 @@
                  batch_size: int=32, 
                  learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
 
         super(Ranker, self).__init__(input_, 
                                      num_outputs, 
                                      hidden_layer_sizes, 
-                                     torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                     torch.device('cuda' if torch.cuda.is_available() else 'cpu'), 
                                      self._activate(activation), 
                                      self._criterion(criterion),
                                      solver, 
                                      batch_size, 
                                      learning_rate_init, 
                                      lr_scheduler)
 
@@ -261,17 +261,17 @@
             return torch.nn.CELU(inplace=True)
         else:
             raise ValueError("Activation Function Supports Options: relu, rrelu, leaky_relu, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "MultiLabelMarginLoss", "BCEWithLogitsLoss", "MSELoss". default: MultiLabelMarginLoss
+        :param criterion: str, 'MultiLabelMarginLoss', 'BCEWithLogitsLoss', 'MSELoss'. default: MultiLabelMarginLoss
         '''
-        if criterion == 'MultiLabelSoftMarginLoss': # np.array([[0, 1], [1, 1]])
+        if criterion == 'MultiLabelSoftMarginLoss': # torch.long
             return torch.nn.MultiLabelSoftMarginLoss()
-        elif criterion == 'BCEWithLogitsLoss': # np.array([[0.0, 1.0], [1.0, 1.0]])
+        elif criterion == 'BCEWithLogitsLoss': # torch.float
             return torch.nn.BCEWithLogitsLoss()
-        elif criterion == 'MSELoss': # np.array([[1.5, 2.0],[3.0, 1.6]])
+        elif criterion == 'MSELoss': # torch.float
             return torch.nn.MSELoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: MultiLabelSoftMarginLoss, BCEWithLogitsLoss, MSELoss.")
```

## perming/general.py

```diff
@@ -18,15 +18,15 @@
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-2.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
     '''
     def __init__(self, 
                  input_: int, 
                  num_classes: int, # num_classes=1
                  hidden_layer_sizes: Tuple[int]=(100,),
-                 device: str="cuda",
+                 device: str='cuda',
                  *,
                  activation: str='relu', 
                  inplace_on: bool=False, 
                  criterion: str='CrossEntropyLoss', # criterion='MSELoss'
                  solver: str='adam', 
                  batch_size: int=32, 
                  learning_rate_init: float=1e-2,
@@ -42,27 +42,27 @@
                                   batch_size, 
                                   learning_rate_init, 
                                   lr_scheduler)
 
     def _device(self, option: str) -> None:
         '''
         Set Device for Model and Training.
-        :param option: device configuration. str, "cuda" or "cpu".
+        :param option: device configuration. str, 'cuda' or 'cpu'.
         '''
-        if option == "cuda":
-            return torch.device(option if torch.cuda.is_available() else "cpu")
-        elif option == "cpu":
+        if option == 'cuda':
+            return torch.device(option if torch.cuda.is_available() else 'cpu')
+        elif option == 'cpu':
             return torch.device(option)
         else:
-            raise ValueError('Box Only Support 2 Options for Device Configuration: "cuda" or "cpu".')
+            raise ValueError("Box Only Support 2 Options for Device Configuration: 'cuda' or 'cpu'.")
 
     def _activate(self, activation: str, inplace_on: bool):
         '''
         Configure Activation with `activation` and `inplace_on`.
-        :param activation: str, "relu", "tanh", "sigmoid", "rrelu", "leaky_relu", "prelu", "softplus", "elu", "celu".
+        :param activation: str, 'relu', 'tanh', 'sigmoid', 'rrelu', 'leaky_relu', 'prelu', 'softplus', 'elu', 'celu'.
         :param inplace_on: bool, whether to use `inplace=True` on activations. default: False.
         '''
         if activation == 'relu': # most use
             return torch.nn.ReLU(inplace=inplace_on)
         elif activation == 'tanh':
             return torch.nn.Tanh()
         elif activation == 'sigmoid': # can be used in classification = 2
@@ -81,15 +81,15 @@
             return torch.nn.CELU(inplace=inplace_on)
         else:
             raise ValueError("Activation Function Supports Options: relu, tanh, sigmoid, rrelu, leaky_relu, softplus, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "CrossEntropyLoss", "NLLLoss", "MultiLabelMarginLoss", "BCELoss", "BCEWithLogitsLoss", "MSELoss", "L1Loss", "SmoothL1Loss", "KLDivLoss". default: CrossEntropyLoss.
+        :param criterion: str, 'CrossEntropyLoss', 'NLLLoss', 'MultiLabelMarginLoss', 'BCELoss', 'BCEWithLogitsLoss', 'MSELoss', 'L1Loss', 'SmoothL1Loss', 'KLDivLoss'. default: CrossEntropyLoss.
         '''
         if criterion == 'CrossEntropyLoss': # classification with num_classes > 2.
             return torch.nn.CrossEntropyLoss()
         elif criterion == 'NLLLoss':
             return torch.nn.NLLLoss()
         elif criterion == 'MultiLabelSoftMarginLoss':
             return torch.nn.MultiLabelSoftMarginLoss()
```

## Comparing `perming-1.3.0.dist-info/METADATA` & `perming-1.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.3.0
+Version: 1.3.1
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
```

## Comparing `perming-1.3.0.dist-info/RECORD` & `perming-1.3.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perming/__init__.py,sha256=4aona4mDIp6VRzAJBa7iz4nRP9-yd77_Ypff0KvQNRY,887
+perming/__init__.py,sha256=rL_phPpO1ftL_MoZLxTY0HwDkbrxLpoOwUm5S57ebLE,887
 perming/_typing.py,sha256=SGQP3QKfMZr-ciHT6jIrv4NUDmgqkx-RhYxIQloBSC4,176
-perming/_utils.py,sha256=HPF94TnQlIiGBw4Tlk8qhwF35W-g7lAGK5tyzww7G_0,20745
+perming/_utils.py,sha256=vGOP8DKHvt7t5Iu35VnVRQ5un23uHTIEPByb97S1P1k,21066
 perming/_version.py,sha256=K3CPQxLgHmXPNpNWlhpnrp6Bt8v5rU9wZyVRBsRTI3E,568
-perming/common.py,sha256=pOz6zWTF7cULulskyt3AGnoRj3P9kCLQUrECGwEaomM,14049
-perming/general.py,sha256=V2ZzelsVUeuDvp6zA44kCguSthncCoKmf-Hh5iKyTws,5605
-perming-1.3.0.dist-info/METADATA,sha256=0_jdJOlAZkezFjUyUKegLWg6Y_v13tHqFiVyf8KRNdM,8772
-perming-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-perming-1.3.0.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
-perming-1.3.0.dist-info/RECORD,,
+perming/common.py,sha256=_-wi8gZFYCtO81XNvu8y-WLJQiZj1-IJ9Ipr2YHWlYw,13988
+perming/general.py,sha256=sUjieRqdWa3o6PXdici5ABarVHcBTCVuv1Wg2K1kggI,5605
+perming-1.3.1.dist-info/METADATA,sha256=9qnNk_Vy8xrOXZ62pj8gm5nWkNJnxcFowZXdQujHGUM,8772
+perming-1.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+perming-1.3.1.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
+perming-1.3.1.dist-info/RECORD,,
```

