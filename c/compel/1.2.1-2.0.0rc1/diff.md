# Comparing `tmp/compel-1.2.1.tar.gz` & `tmp/compel-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-sibov8rl/compel-1.2.1.tar", last modified: Sun Jun  4 13:28:28 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-3zkjqq6r/compel-2.0.0rc1.tar", last modified: Wed Jul 12 22:59:45 2023, max compression
```

## Comparing `compel-1.2.1.tar` & `compel-2.0.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.2.1/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)    11033 2023-06-04 13:28:28.000000 compel-1.2.1/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)    10455 2023-06-04 12:40:31.000000 compel-1.2.1/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-06-04 12:40:07.000000 compel-1.2.1/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-06-04 13:28:28.000000 compel-1.2.1/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-1.2.1/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    15856 2023-06-04 13:25:19.000000 compel-1.2.1/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.2.1/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.2.1/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-1.2.1/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    25187 2023-06-03 06:15:11.000000 compel-1.2.1/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29912 2023-06-03 06:55:13.000000 compel-1.2.1/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    11033 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/test/
--rw-r--r--   0 damian     (501) staff       (20)    15682 2023-06-03 18:14:58.000000 compel-1.2.1/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-1.2.1/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-1.2.1/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.0rc1/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-12 22:59:45.000000 compel-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    10494 2023-07-04 22:01:43.000000 compel-2.0.0rc1/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-12 22:59:12.000000 compel-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-12 22:59:45.000000 compel-2.0.0rc1/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.0rc1/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    20003 2023-07-12 22:48:45.000000 compel-2.0.0rc1/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.0rc1/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.0rc1/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.0rc1/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    30339 2023-07-12 22:57:28.000000 compel-2.0.0rc1/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.0rc1/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/test/
+-rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-12 22:58:27.000000 compel-2.0.0rc1/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.0rc1/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.0rc1/test/test_prompt_parser.py
```

### Comparing `compel-1.2.1/LICENSE` & `compel-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.2.1/PKG-INFO` & `compel-2.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.2.1
+Version: 2.0.0rc1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -15,25 +15,29 @@
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embedding tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
-Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
+Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)).
 
 Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
 ### Installation
 
 `pip install compel`
 
+### Documentation
+
+Documentation is [here](doc/).
+
 ### Demo
 
-see [compel-demo.ipynb](compel-demo.ipynb)
+See [compel-demo.ipynb](compel-demo.ipynb)
 
 <a target="_blank" href="https://colab.research.google.com/github/damian0815/compel/blob/main/compel-demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ### Quickstart
 
@@ -82,15 +86,17 @@
 textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
     textual_inversion_manager=textual_inversion_manager)
 ```
 
 ## Memory usage/VRAM leaks
 
-If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
+If you run into memory issues, please make sure you're running compel inside `with torch.no_grad():` blocks. 
+
+If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
 #### 1.2.1 - actually apply `.and()` weights
```

### Comparing `compel-1.2.1/README.md` & `compel-2.0.0rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embedding tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
-Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
+Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)).
 
 Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
 ### Installation
 
 `pip install compel`
 
+### Documentation
+
+Documentation is [here](doc/).
+
 ### Demo
 
-see [compel-demo.ipynb](compel-demo.ipynb)
+See [compel-demo.ipynb](compel-demo.ipynb)
 
 <a target="_blank" href="https://colab.research.google.com/github/damian0815/compel/blob/main/compel-demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ### Quickstart
 
@@ -68,15 +72,17 @@
 textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
     textual_inversion_manager=textual_inversion_manager)
 ```
 
 ## Memory usage/VRAM leaks
 
-If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
+If you run into memory issues, please make sure you're running compel inside `with torch.no_grad():` blocks. 
+
+If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
 #### 1.2.1 - actually apply `.and()` weights
```

### Comparing `compel-1.2.1/pyproject.toml` & `compel-2.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.2.1"
+version = "2.0.0-pre1"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.2.1/src/compel/compel.py` & `compel-2.0.0rc1/src/compel/compel.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,37 +3,39 @@
 
 import torch
 from torch import Tensor
 from transformers import CLIPTokenizer, CLIPTextModel
 
 from . import cross_attention_control
 from .conditioning_scheduler import ConditioningScheduler, StaticConditioningScheduler
-from .embeddings_provider import EmbeddingsProvider, BaseTextualInversionManager, DownweightMode
+from .embeddings_provider import EmbeddingsProvider, BaseTextualInversionManager, DownweightMode, ReturnedEmbeddingsType, EmbeddingsProviderMulti
 from .prompt_parser import Blend, FlattenedPrompt, PromptParser, CrossAttentionControlSubstitute, Conjunction
 
 __all__ = ["Compel", "DownweightMode"]
 
 @dataclass
 class ExtraConditioningInfo:
     pass
 
 
 class Compel:
 
 
     def __init__(self,
-                 tokenizer: CLIPTokenizer,
-                 text_encoder: CLIPTextModel,
+                 tokenizer: Union[CLIPTokenizer, List[CLIPTokenizer]],
+                 text_encoder: Union[CLIPTextModel, List[CLIPTextModel]],
                  textual_inversion_manager: Optional[BaseTextualInversionManager] = None,
                  dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
                  truncate_long_prompts: bool = True,
                  padding_attention_mask_value: int = 1,
                  downweight_mode: DownweightMode = DownweightMode.MASK,
-                 use_penultimate_clip_layer: bool=False,
-                 device: Optional[str] = None):
+                 returned_embeddings_type: ReturnedEmbeddingsType = ReturnedEmbeddingsType.LAST_HIDDEN_STATES_NORMALIZED,
+                 requires_pooled: bool = False,
+                 device: Optional[str] = None
+                 ):
         """
         Initialize Compel. The tokenizer and text_encoder can be lifted directly from any DiffusionPipeline.
 
         `textual_inversion_manager`: Optional instance to handle expanding multi-vector textual inversion tokens.
         `dtype_for_device_getter`: A Callable that returns a torch dtype for a given device. You probably don't need to
             use this.
         `truncate_long_prompts`: if True, truncate input prompts to 77 tokens long including beginning/end markers
@@ -41,64 +43,115 @@
             If False, do not truncate, and instead assemble as many 77 token long chunks, each capped by beginning/end
             markers, as is necessary to encode the whole prompt. You will likely need to supply both positive and
             negative prompts in this case - use `pad_conditioning_tensors_to_same_length` to prevent having tensor
             length mismatch errors when passing the embeds on to your DiffusionPipeline for inference.
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
         `downweight_mode`: Specifies whether downweighting should be applied by MASKing out the downweighted tokens
             (default) or REMOVEing them (legacy behaviour; messes up position embeddings of tokens following).
-        `use_penultimate_clip_layer`: If True, use the penultimate hidden layer output of the CLIP text encoder's output,
-            rather than the final hidden layer output.
-        `device`: The torch device on which the tensors should be created. If a device is not specified, it'll use the
-            device the `text_encoder` is on (at the moment of calling `build_conditioning_tensor()`).
-        """
-        self.conditioning_provider = EmbeddingsProvider(tokenizer=tokenizer,
-                                                        text_encoder=text_encoder,
-                                                        textual_inversion_manager=textual_inversion_manager,
-                                                        dtype_for_device_getter=dtype_for_device_getter,
-                                                        truncate=truncate_long_prompts,
-                                                        padding_attention_mask_value = padding_attention_mask_value,
-                                                        downweight_mode=downweight_mode,
-                                                        use_penultimate_clip_layer=use_penultimate_clip_layer
-                                                        )
+        `returned_embeddings_type`: controls how the embedding vectors are taken from the result of running the text encoder over the parsed prompt's text
+        `requires_pooled`: for SDXL, append the pooled embeddings when returning conditioning tensors
+        `device`: The torch device on which the tensors should be created. If a device is not specified, the device will
+            be the same as that of the `text_encoder` at the moment when `build_conditioning_tensor()` is called.
+        """
+        if isinstance(tokenizer, (tuple, list)) and not isinstance(text_encoder, (tuple, list)):
+            raise ValueError("Cannot provide list of tokenizers, but not of text encoders.")
+        elif not isinstance(tokenizer, (tuple, list)) and isinstance(text_encoder, (tuple, list)):
+            raise ValueError("Cannot provide list of text encoders, but not of tokenizers.")
+        elif isinstance(tokenizer, (tuple, list)) and isinstance(text_encoder, (tuple, list)):
+            self.conditioning_provider = EmbeddingsProviderMulti(tokenizers=tokenizer,
+                                                            text_encoders=text_encoder,
+                                                            textual_inversion_manager=textual_inversion_manager,
+                                                            dtype_for_device_getter=dtype_for_device_getter,
+                                                            truncate=truncate_long_prompts,
+                                                            padding_attention_mask_value = padding_attention_mask_value,
+                                                            downweight_mode=downweight_mode,
+                                                            returned_embeddings_type=returned_embeddings_type,
+                                                            requires_pooled_mask = requires_pooled
+            )
+        else:
+            self.conditioning_provider = EmbeddingsProvider(tokenizer=tokenizer,
+                                                            text_encoder=text_encoder,
+                                                            textual_inversion_manager=textual_inversion_manager,
+                                                            dtype_for_device_getter=dtype_for_device_getter,
+                                                            truncate=truncate_long_prompts,
+                                                            padding_attention_mask_value = padding_attention_mask_value,
+                                                            downweight_mode=downweight_mode,
+                                                            returned_embeddings_type=returned_embeddings_type,
+                                                            )
         self._device = device
+        self.requires_pooled = requires_pooled
 
     @property
     def device(self):
         return self._device if self._device else self.conditioning_provider.text_encoder.device
 
-    def make_conditioning_scheduler(self, positive_prompt: str, negative_prompt: str='') -> ConditioningScheduler:
+    def make_conditioning_scheduler(self, positive_prompt: str, negative_prompt: str='')  -> ConditioningScheduler:
+        """
+        Return a ConditioningScheduler object that provides conditioning tensors for different diffusion steps (currently
+        not fully implemented).
+        """
         positive_conditioning = self.build_conditioning_tensor(positive_prompt)
         negative_conditioning = self.build_conditioning_tensor(negative_prompt)
         [positive_conditioning, negative_conditioning] = self.pad_conditioning_tensors_to_same_length(
             [positive_conditioning, negative_conditioning]
         )
         return StaticConditioningScheduler(positive_conditioning=positive_conditioning,
                                            negative_conditioning=negative_conditioning)
 
     def build_conditioning_tensor(self, text: str) -> torch.Tensor:
+        """
+        Build a conditioning tensor by parsing the text for Compel syntax, constructing a Conjunction, and then
+        building a conditioning tensor from that Conjunction.
+        """
         conjunction = self.parse_prompt_string(text)
         conditioning, _ = self.build_conditioning_tensor_for_conjunction(conjunction)
-        return conditioning
+
+        if self.requires_pooled:
+            pooled = self.conditioning_provider.get_pooled_embeddings([text])
+            return conditioning, pooled
+        else:
+            return conditioning
 
     @torch.no_grad()
     def __call__(self, text: Union[str, List[str]]) -> torch.FloatTensor:
+        """
+        Take a string or a list of strings and build conditioning tensors to match.
+
+        If multiple strings are passed, the resulting tensors will be padded until they have the same length.
+
+        :return: A tensor consisting of conditioning tensors for each of the passed-in strings, concatenated along dim 0.
+        """
         if not isinstance(text, list):
             text = [text]
 
         cond_tensor = []
+        pooled = []
         for text_input in text:
-            cond_tensor.append(self.build_conditioning_tensor(text_input))
+            output = self.build_conditioning_tensor(text_input)
+
+            if self.requires_pooled:
+                cond_tensor.append(output[0])
+                pooled.append(output[1])
+            else:
+                cond_tensor.append(output)
 
         cond_tensor = self.pad_conditioning_tensors_to_same_length(conditionings=cond_tensor)
         cond_tensor = torch.cat(cond_tensor)
 
-        return cond_tensor
+        if self.requires_pooled:
+            pooled = torch.cat(pooled)
+            return cond_tensor, pooled
+        else:
+            return cond_tensor
 
     @classmethod
     def parse_prompt_string(cls, prompt_string: str) -> Conjunction:
+        """
+        Parse the given prompt string and return a structured Conjunction object that represents the prompt it contains.
+        """
         pp = PromptParser()
         conjunction = pp.parse_conjunction(prompt_string)
         return conjunction
 
     def describe_tokenization(self, text: str) -> List[str]:
         """
         For the given text, return a list of strings showing how it will be tokenized.
@@ -106,31 +159,21 @@
         :param text: The text that is to be tokenized.
         :return: A list of strings representing the output of the tokenizer. It's expected that the output list may be
         longer than the number of words in `text` because the tokenizer may split words to multiple tokens. Because of
         this, word boundaries are indicated in the output with `</w>` strings.
         """
         return self.conditioning_provider.tokenizer.tokenize(text)
 
-    def build_conditioning_tensor_for_prompt_object(self, prompt: Union[Blend, FlattenedPrompt],
-                                                    ) -> Tuple[torch.Tensor, dict]:
-        """
-
-        """
-        if type(prompt) is Blend:
-            return self._get_conditioning_for_blend(prompt), {}
-        elif type(prompt) is FlattenedPrompt:
-            if prompt.wants_cross_attention_control:
-                cac_args = self._get_conditioning_for_cross_attention_control(prompt)
-                return cac_args.original_conditioning, { 'cross_attention_control': cac_args }
-            else:
-                return self._get_conditioning_for_flattened_prompt(prompt), {}
-
-        raise ValueError(f"unsupported prompt type: {type(prompt).__name__}")
 
     def build_conditioning_tensor_for_conjunction(self, conjunction: Conjunction) -> Tuple[torch.Tensor, dict]:
+        """
+        Build a conditioning tensor for the given Conjunction object.
+        :return: A tuple of (conditioning tensor, options dict). The contents of the options dict depends on the prompt,
+        at the moment it is only used for returning cross-attention control conditioning data (`.swap()`).
+        """
         if len(conjunction.prompts) > 1 and conjunction.type != 'AND':
             raise ValueError("Only AND conjunctions are supported by build_conditioning_tensor()")
         # concatenate each prompt in the conjunction (typically there will only be 1)
         to_concat = []
         options = {}
         empty_conditioning = None
         for i, p in enumerate(conjunction.prompts):
@@ -142,20 +185,46 @@
                 empty_conditioning = self.build_conditioning_tensor('') if empty_conditioning is None else empty_conditioning
                 [padded_empty_conditioning, _] = self.pad_conditioning_tensors_to_same_length([empty_conditioning, this_conditioning])
                 this_conditioning = padded_empty_conditioning + (this_conditioning - padded_empty_conditioning) * weight
             to_concat.append(this_conditioning)
         return torch.concat(to_concat, dim=1), options
 
 
+    def build_conditioning_tensor_for_prompt_object(self, prompt: Union[Blend, FlattenedPrompt],
+                                                    ) -> Tuple[torch.Tensor, dict]:
+        """
+        Build a conditioning tensor for the given prompt object (either a Blend or a FlattenedPrompt).
+        """
+        if type(prompt) is Blend:
+            return self._get_conditioning_for_blend(prompt), {}
+        elif type(prompt) is FlattenedPrompt:
+            if prompt.wants_cross_attention_control:
+                cac_args = self._get_conditioning_for_cross_attention_control(prompt)
+                return cac_args.original_conditioning, { 'cross_attention_control': cac_args }
+            else:
+                return self._get_conditioning_for_flattened_prompt(prompt), {}
+
+        raise ValueError(f"unsupported prompt type: {type(prompt).__name__}")
+
+
+
     def pad_conditioning_tensors_to_same_length(self, conditionings: List[torch.Tensor],
                                                 ) -> List[torch.Tensor]:
         """
-        If `truncate_long_prompts` was set to False on initialization, conditioning tensors do not have a fixed length.
-        This is a problem when using a negative and a positive prompt to condition the diffusion process. This function
-        pads either c0 or c1 if necessary to ensure they both have the same length, returning the padded c0 and c1.
+        If `truncate_long_prompts` was set to False on initialization, or if your prompt includes a `.and()` operator,
+        conditioning tensors do not have a fixed length. This is a problem when using a negative and a positive prompt
+        to condition the diffusion process. This function pads any of the passed-in tensors, as necessary, to ensure
+        they all have the same length, returning the padded tensors in the same order they are passed.
+
+        Example:
+            ``` python
+            embeds = compel('("a cat playing in the forest", "an impressionist oil painting").and()')
+            negative_embeds = compel("ugly, deformed, distorted")
+            [embeds, negative_embeds] = compel.pad_conditioning_tensors_to_same_length([embeds, negative_embeds])
+            ```
         """
         c0_shape = conditionings[0].shape
         if not all([len(c.shape) == len(c0_shape) for c in conditionings]):
             raise ValueError("Conditioning tensors must all have either 2 dimensions (unbatched) or 3 dimensions (batched)")
 
         if len(c0_shape) == 2:
             # need to be unsqueezed
@@ -163,40 +232,40 @@
             c0_shape = conditionings[0].shape
         if len(c0_shape) != 3:
             raise ValueError(f"All conditioning tensors must have the same number of dimensions (2 or 3)")
 
         if not all([c.shape[0] == c0_shape[0] and c.shape[2] == c0_shape[2] for c in conditionings]):
             raise ValueError(f"All conditioning tensors must have the same batch size ({c0_shape[0]}) and number of embeddings per token ({c0_shape[1]}")
 
-
         max_token_count = max([c.shape[1] for c in conditionings])
         # if necessary, pad shorter tensors out with an emptystring tensor
-        empty_z = torch.cat([self.build_conditioning_tensor("")] * c0_shape[0])
+        emptystring_conditioning = self.build_conditioning_tensor("")
+        if type(emptystring_conditioning) is tuple:
+            # discard pooled
+            emptystring_conditioning = emptystring_conditioning[0]
+        empty_z = torch.cat([emptystring_conditioning] * c0_shape[0])
         for i, c in enumerate(conditionings):
             while c.shape[1] < max_token_count:
                 c = torch.cat([c, empty_z], dim=1)
-            conditionings[i] = c
+                conditionings[i] = c
         return conditionings
 
 
     def _get_conditioning_for_flattened_prompt(self,
                                                prompt: FlattenedPrompt,
                                                should_return_tokens: bool=False
                                                ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         if type(prompt) is not FlattenedPrompt:
             raise ValueError(f"embeddings can only be made from FlattenedPrompts, got {type(prompt).__name__} instead")
         fragments = [x.text for x in prompt.children]
         weights = [x.weight for x in prompt.children]
-        conditioning, tokens = self.conditioning_provider.get_embeddings_for_weighted_prompt_fragments(
+        return self.conditioning_provider.get_embeddings_for_weighted_prompt_fragments(
             text_batch=[fragments], fragment_weights_batch=[weights],
-            should_return_tokens=True, device=self.device)
-        if should_return_tokens:
-            return conditioning, tokens
-        else:
-            return conditioning
+            should_return_tokens=should_return_tokens, device=self.device)
+
 
     def _get_conditioning_for_blend(self, blend: Blend):
         conditionings_to_blend = []
         for i, flattened_prompt in enumerate(blend.prompts):
             this_conditioning = self._get_conditioning_for_flattened_prompt(flattened_prompt)
             conditionings_to_blend.append(this_conditioning)
         conditionings_to_blend = self.pad_conditioning_tensors_to_same_length(conditionings_to_blend)
```

### Comparing `compel-1.2.1/src/compel/conditioning_scheduler.py` & `compel-2.0.0rc1/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.1/src/compel/cross_attention_control.py` & `compel-2.0.0rc1/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.1/src/compel/diffusers_textual_inversion_manager.py` & `compel-2.0.0rc1/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.1/src/compel/embeddings_provider.py` & `compel-2.0.0rc1/src/compel/embeddings_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 import math
 from abc import ABC
 from enum import Enum
-from typing import Callable, Union, Tuple, List, Optional
+from typing import Callable, Union, Optional
 
 import torch
-from transformers import CLIPTokenizer, CLIPTextModel
+from transformers import CLIPTokenizer, CLIPTextModel, CLIPTextModelWithProjection
+from typing import List, Tuple
 
-__all__ = ["EmbeddingsProvider", "DownweightMode"]
+__all__ = ["EmbeddingsProvider", "DownweightMode", "ReturnedEmbeddingsType"]
 
 
 class DownweightMode(Enum):
     REMOVE = 0  # Remove downweighted tokens from the token sequence (shifts all subsequent tokens)
-    MASK = 1,   # Default: Leave tokens in-place but mask them out using attention masking
+    MASK = 1   # Default: Leave tokens in-place but mask them out using attention masking
 
 class BaseTextualInversionManager(ABC):
     def expand_textual_inversion_token_ids_if_necessary(self, token_ids: List[int]) -> List[int]:
         raise NotImplementedError()
 
+class ReturnedEmbeddingsType(Enum):
+    LAST_HIDDEN_STATES_NORMALIZED = 0             # SD1/2 regular
+    PENULTIMATE_HIDDEN_STATES_NORMALIZED = 1      # SD1.5 with "clip skip"
+    PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED = 2  # SDXL
+
 
 class EmbeddingsProvider:
 
     def __init__(self,
                  tokenizer: CLIPTokenizer,
-                 text_encoder: CLIPTextModel,
+                 text_encoder: Union[CLIPTextModel, CLIPTextModelWithProjection], # convert a list of int token ids to a tensor of embeddings
                  textual_inversion_manager: BaseTextualInversionManager = None,
                  dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
                  truncate: bool = True,
                  padding_attention_mask_value: int = 1,
                  downweight_mode: DownweightMode = DownweightMode.MASK,
-                 use_penultimate_clip_layer: bool=False
+                 returned_embeddings_type: ReturnedEmbeddingsType = ReturnedEmbeddingsType.LAST_HIDDEN_STATES_NORMALIZED
                  ):
         """
         `tokenizer`: converts strings to lists of int token ids
         `text_encoder`: convert lists of token ids to embedding tensors
         `textual_inversion_manager`: manage token insertion for textual inversions with vector length >1
         `dtype_for_device_getter`: callback that returns an appropriate dtype for the requested device. if unset, defaults to torch.float32.
         `truncate`: if True, truncate inputs to the maximum length specified by the tokenizer. if False, returns
                     tensors that may be longer than the maximum length (but will always be an integer multiple of maximum length)
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
         `downweight_mode`: if MASK, downweight by blending with a version of the prompt with the downweighted terms masked out.
                     if REMOVE, the blend is against a version of the prompt with the downweighted tokens removed
         `use_penultimate_clip_layer`: Whether to tuse the penultimate hidden state output of the CLIP emcoder (True) or
                     the final hidden state output (False, default).
+        `requires_pooled`:
         """
         self.tokenizer = tokenizer
         self.text_encoder = text_encoder
         self.textual_inversion_manager = textual_inversion_manager
         self.truncate_to_model_max_length = truncate
         self.padding_attention_mask_value = padding_attention_mask_value
         self.downweight_mode = downweight_mode
-        self.use_penultimate_clip_layer = use_penultimate_clip_layer
+        self.returned_embeddings_type = returned_embeddings_type
 
         # by default always use float32
         self.get_dtype_for_device = dtype_for_device_getter
 
 
     @property
     def max_token_count(self) -> int:
@@ -179,15 +186,15 @@
         #print(f"assembled all tokens into tensor of shape {batch_z.shape}")
 
         if should_return_tokens:
             return batch_z, batch_tokens
         else:
             return batch_z
 
-    def get_token_ids(self, texts: List[str], include_start_and_end_markers: bool = True) -> List[List[int]]:
+    def get_token_ids(self, texts: List[str], include_start_and_end_markers: bool = True, padding: str = 'do_not_pad') -> List[List[int]]:
         """
         Convert a list of strings like `["a cat", "a dog", "monkey riding a bicycle"]` into a list of lists of token
         ids like `[[bos, 0, 1, eos], [bos, 0, 2, eos], [bos, 3, 4, 0, 5, eos]]`. bos/eos markers are skipped if
         `include_start_and_end_markers` is `False`. Each list will be restricted to the maximum permitted length
         (typically 75 tokens + eos/bos markers).
 
         :param texts: The strings to convert.
@@ -196,15 +203,15 @@
         :return: A list of lists of token ids corresponding to the input strings.
         """
         # for args documentation of self.tokenizer() see ENCODE_KWARGS_DOCSTRING in tokenization_utils_base.py
         # (part of `transformers` lib)
         token_ids_list = self.tokenizer(
             texts,
             truncation=self.truncate_to_model_max_length,
-            padding='do_not_pad',
+            padding=padding,
             return_tensors=None,  # just give me lists of ints
         )['input_ids']
 
         result = []
         for token_ids in token_ids_list:
             # trim eos/bos
             token_ids = token_ids[1:-1]
@@ -216,14 +223,24 @@
             if include_start_and_end_markers:
                 token_ids = [self.tokenizer.bos_token_id] + token_ids + [self.tokenizer.eos_token_id]
 
             result.append(token_ids)
 
         return result
 
+    def get_pooled_embeddings(self, texts: List[str], attention_mask: Optional[torch.Tensor]=None) -> Optional[torch.Tensor]:
+        token_ids = self.get_token_ids(texts, padding="max_length")
+        token_ids = torch.tensor(token_ids, dtype=torch.long).to(self.text_encoder.device)
+
+        text_encoder_output = self.text_encoder(token_ids, attention_mask, return_dict=True)
+        pooled = text_encoder_output.text_embeds
+
+        return pooled
+
+
     def get_token_ids_and_expand_weights(self, fragments: List[str], weights: List[float], device: str
                                          ) -> (torch.Tensor, torch.Tensor, torch.Tensor):
         '''
         Given a list of text fragments and corresponding weights: tokenize each fragment, append the token sequences
         together and return a padded token sequence starting with the bos marker, ending with the eos marker, and padded
         or truncated as appropriate to `self.max_length`. Also return a list of weights expanded from the passed-in
         weights to match each token.
@@ -301,15 +318,15 @@
     def build_weighted_embedding_tensor(self,
                                         token_ids: torch.Tensor,
                                         per_token_weights: torch.Tensor,
                                         attention_mask: Optional[torch.Tensor] = None,
                                         device: Optional[str] = None) -> torch.Tensor:
         """
         Build a tensor that embeds the passed-in token IDs and applies the given per_token weights
-
+        
         :param token_ids: A tensor of shape `n*[self.max_length]` containing token IDs (ints) where n is some arbitrary
             integer (i.e. n==1 for shorter prompts, or it may be >1 if there are more than max_length tokens in the
             original prompt)
         :param per_token_weights: A tensor containing weights (floats), with the same shape as token_ids
         :param attention_mask: A tensor containing a mask (ints), with the same shape as token_ids, where 1 means use
             the corresponding token and 0 means ignore the corresponding token.
 
@@ -355,32 +372,38 @@
             )
             chunk_start_index += chunk_size
 
         return weighted_z
 
     def _encode_token_ids_to_embeddings(self, token_ids: torch.Tensor,
                                         attention_mask: Optional[torch.Tensor]=None) -> torch.Tensor:
+        needs_hidden_states = (self.returned_embeddings_type == ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NORMALIZED or
+                               self.returned_embeddings_type == ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED)
         text_encoder_output = self.text_encoder(token_ids,
                                                 attention_mask,
-                                                output_hidden_states=self.use_penultimate_clip_layer,
+                                                output_hidden_states=needs_hidden_states,
                                                 return_dict=True)
-        if self.use_penultimate_clip_layer:
-            # needs normalizing
+        if self.returned_embeddings_type is ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED:
+            penultimate_hidden_state = text_encoder_output.hidden_states[-2]
+            return penultimate_hidden_state
+        elif self.returned_embeddings_type is ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NORMALIZED:
             penultimate_hidden_state = text_encoder_output.hidden_states[-2]
             return self.text_encoder.text_model.final_layer_norm(penultimate_hidden_state)
-        else:
+        elif self.returned_embeddings_type is ReturnedEmbeddingsType.LAST_HIDDEN_STATES_NORMALIZED:
             # already normalized
             return text_encoder_output.last_hidden_state
 
+        assert False, f"unrecognized ReturnEmbeddingsType: {self.returned_embeddings_type}"
+
     def _get_token_ranges_for_fragments(self, chunked_and_padded_token_ids: List[int], fragments: List[str]) -> List[Tuple[int, int]]:
         """
         Match token id sequences for the strings in `fragments` with token id sequences in `chunked_and_padded_token_ids`,
-         taking into account any eos and bos markers marking `self.tokenizer.max_model_length` sized chunks.
+         taking into account any eos and bos markers that indicate `self.tokenizer.max_model_length`-sized chunks.
 
-        Returns a list of tuples indicating start and end indices of each fragment's corresponding token id sequence in
+        :return: a list of tuples indicating start and end indices of each fragment's corresponding token id sequence in
          `chunked_and_padded_token_ids`.
         """
         per_fragment_token_ids = self.get_token_ids(fragments, include_start_and_end_markers=False)
         fragment_start = 0
 
         corresponding_indices = []
         for fragment_index, fragment_token_ids in enumerate(per_fragment_token_ids):
@@ -429,7 +452,77 @@
                         f"token sequence mismatch for fragment at index {fragment_index} '{fragments[fragment_index]}':"
                         f"expected {fragment_token_ids}, found {chunked_and_padded_token_ids[fragment_start:fragment_end + 1]}")
 
             corresponding_indices.append((fragment_start, fragment_end))
             fragment_start = fragment_end + 1
 
         return corresponding_indices
+
+
+class EmbeddingsProviderMulti:
+
+    def __init__(self,
+                tokenizers: CLIPTokenizer,
+                text_encoders: Union[CLIPTextModel, CLIPTextModelWithProjection], # convert a list of int token ids to a tensor of embeddings
+                textual_inversion_manager: BaseTextualInversionManager = None,
+                dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
+                truncate: bool = True,
+                padding_attention_mask_value: int = 1,
+                downweight_mode: DownweightMode = DownweightMode.MASK,
+                returned_embeddings_type: Union[List[ReturnedEmbeddingsType], ReturnedEmbeddingsType] = ReturnedEmbeddingsType.LAST_HIDDEN_STATES_NORMALIZED,
+                 requires_pooled_mask: List[bool] = []
+                ):
+
+        returned_embeddings_type = len(text_encoders) * [returned_embeddings_type] if not isinstance(returned_embeddings_type, (list,tuple)) else returned_embeddings_type
+
+        self.embedding_providers = [
+            EmbeddingsProvider(tokenizer, text_encoder, textual_inversion_manager, dtype_for_device_getter, truncate, padding_attention_mask_value, downweight_mode, returned_embeddings_type)
+            for tokenizer, text_encoder, returned_embeddings_type in zip(tokenizers, text_encoders, returned_embeddings_type)
+        ]
+        self.requires_pooled_mask = requires_pooled_mask
+
+    @property
+    def text_encoder(self):
+        return self.embedding_providers[0].text_encoder
+
+    @property
+    def tokenizer(self):
+        return self.embedding_providers[0].tokenizer
+
+    def get_token_ids(self, *args, **kwargs):
+        # get token ids does not use padding. The padding ID is the only ID that can differ between tokenizers
+        # so for simplicity, we just return `get_token_ids` of the first tokenizer
+        return self.embedding_providers[0].get_token_ids(self, *args, **kwargs)
+
+    def get_pooled_embeddings(self, texts: List[str], attention_mask: Optional[torch.Tensor]=None) -> Optional[torch.Tensor]:
+        pooled = [self.embedding_providers[provider_index].get_pooled_embeddings(texts, attention_mask)
+                  for provider_index, requires_pooled in enumerate(self.requires_pooled_mask) if requires_pooled]
+
+        if len(pooled) == 0:
+            return None
+
+        return torch.cat(pooled, dim=-1)
+
+    def get_embeddings_for_weighted_prompt_fragments(self,
+                                                     text_batch: List[List[str]],
+                                                     fragment_weights_batch: List[List[float]],
+                                                     should_return_tokens: bool = False,
+                                                     device='cpu',
+                                 ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
+
+        outputs = [provider.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch, should_return_tokens=should_return_tokens, device=device) for provider in self.embedding_providers]
+
+        text_embeddings_list = []
+        tokens = []
+
+        for output in outputs:
+            text_embeddings_list.append(output[0])
+
+            if should_return_tokens:
+                tokens.append(output[1])
+
+        text_embeddings = torch.cat(text_embeddings_list, dim=-1)
+
+        if should_return_tokens:
+            return text_embeddings, tokens
+        else:
+            return text_embeddings
```

### Comparing `compel-1.2.1/src/compel/prompt_parser.py` & `compel-2.0.0rc1/src/compel/prompt_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,51 +16,14 @@
 
 Useful function exports:
 
 split_weighted_subpromopts()    split subprompts, normalize and weight them
 log_tokenization()              print out colour-coded tokens and warn if truncated
 '''
 
-class Prompt():
-    """
-    Mid-level structure for storing the tree-like result of parsing a prompt. A Prompt may not represent the whole of
-    the singular user-defined "prompt string" (although it can) - for example, if the user specifies a Blend, the objects
-    that are to be blended together are stored individuall as Prompt objects.
-
-    Nesting makes this object not suitable for directly tokenizing; instead call flatten() on the containing Conjunction
-    to produce a FlattenedPrompt.
-    """
-    def __init__(self, parts: list):
-        self.children = []
-        for p in parts:
-            if (type(p) is LoraWeight
-                  or type(p) is Attention
-                  or issubclass(type(p), BaseFragment)
-                  or type(p) is pp.ParseResults):
-                self.children.append(p)
-            else:
-                raise PromptParser.ParsingException(
-                    f"Prompt cannot contain {type(p).__name__} ({p}), only "
-                    f"{[c.__name__ for c in BaseFragment.__subclasses__()]} are allowed"
-                )
-
-    def __repr__(self):
-        return f"Prompt:{self.children}"
-
-    def __eq__(self, other):
-        return (type(other) is Prompt
-                and other.children == self.children)
-
-@dataclass
-class LoraWeight:
-    model: str
-    weight: float
-
-    def __repr__(self):
-        return(f"Lora('{self.model}'@{self.weight})")
 
 class BaseFragment:
     pass
 
 class FlattenedPrompt():
     """
     A Prompt that has been passed through flatten(). Its children can be readily tokenized.
@@ -105,17 +68,129 @@
     def __repr__(self):
         return (f"FlattenedPrompt:{self.children}")
     def __eq__(self, other):
         return (type(other) is FlattenedPrompt
                and other.children == self.children)
 
 
+class Prompt():
+    """
+    Intermediate structure for storing the tree-like result of parsing a prompt. A Prompt may not represent the whole of
+    the singular user-defined "prompt string" (although it can) - for example, if the user specifies a Blend, the objects
+    that are to be blended together are stored individually as Prompt objects.
+
+    Nesting makes this object not suitable for directly tokenizing; instead call `PromptParser.flatten()` on the
+    containing Conjunction to produce a FlattenedPrompt.
+    """
+    def __init__(self, parts: list):
+        self.children = []
+        for p in parts:
+            if (type(p) is LoraWeight
+                  or type(p) is Attention
+                  or issubclass(type(p), BaseFragment)
+                  or type(p) is pp.ParseResults):
+                self.children.append(p)
+            else:
+                raise PromptParser.ParsingException(
+                    f"Prompt cannot contain {type(p).__name__} ({p}), only "
+                    f"{[c.__name__ for c in BaseFragment.__subclasses__()]} are allowed"
+                )
+
+    def __repr__(self):
+        return f"Prompt:{self.children}"
+
+    def __eq__(self, other):
+        return (type(other) is Prompt
+                and other.children == self.children)
+
+@dataclass
+class LoraWeight:
+    """
+    Storage for information about a LoRA, requested using `.withLora(<name>, <weight>)`
+    """
+    model: str
+    weight: float
+
+    def __repr__(self):
+        return(f"Lora('{self.model}'@{self.weight})")
+
+class Blend():
+    """
+    Stores a Blend of multiple Prompts, requested using eg `("prompt 1", "prompt 2").blend(1, 1)`
+
+    To apply, build feature vectors for each of the child Prompts and then perform a weighted blend of the feature
+    vectors to produce a single feature vector that is effectively a lerp between the Prompts.
+    """
+    def __init__(self, prompts: List, weights: List[float], normalize_weights: bool=True):
+        #print("making Blend with prompts", prompts, "and weights", weights)
+        weights = [1.0]*len(prompts) if (weights is None or len(weights)==0) else list(weights)
+        if len(prompts) != len(weights):
+            raise PromptParser.ParsingException(f"while parsing Blend: mismatched prompts/weights counts {prompts}, {weights}")
+        for p in prompts:
+            if type(p) is not Prompt and type(p) is not FlattenedPrompt:
+                raise(PromptParser.ParsingException(f"{type(p)} cannot be added to a Blend, only Prompts or FlattenedPrompts"))
+            for f in p.children:
+                if isinstance(f, CrossAttentionControlSubstitute):
+                    raise(PromptParser.ParsingException(f"while parsing Blend: sorry, you cannot do .swap() as part of a Blend"))
+
+        # upcast all lists to Prompt objects
+        self.prompts = [x if (type(x) is Prompt or type(x) is FlattenedPrompt)
+                         else Prompt(x)
+                        for x in prompts]
+        self.prompts = prompts
+        self.weights = weights
+        self.normalize_weights = normalize_weights
+
+    @property
+    def wants_cross_attention_control(self):
+        # blends cannot cross-attention control
+        return False
+
+    def __repr__(self):
+        return f"Blend:{self.prompts} | weights {' ' if self.normalize_weights else '(non-normalized) '}{self.weights}"
+    def __eq__(self, other):
+        return other.__repr__() == self.__repr__()
+
+
+class Conjunction():
+    """
+    Storage for one or more Prompts, Blends, or FlattenedPrompts, requested using eg `("prompt 1", "prompt 2").and()`.
+
+    Each component should be combined at runtime to produce an output that reflects all of them at the same time. For
+    Stable Diffusion this can be achieved by concatenating the conditioning tensors for each component.
+    """
+    def __init__(self,
+                 prompts: List[Union[Prompt, Blend, FlattenedPrompt]],
+                 weights: List[float] = None,
+                 lora_weights: List[LoraWeight] = None):
+        # force everything to be a Prompt
+        #print("making conjunction with", prompts, "types", [type(p).__name__ for p in prompts])
+        self.prompts = [x if (type(x) is Prompt
+                          or type(x) is Blend
+                          or type(x) is FlattenedPrompt)
+                      else Prompt(x) for x in prompts]
+        self.weights = [1.0]*len(self.prompts) if (weights is None or len(weights)==0) else list(weights)
+        if len(self.weights) != len(self.prompts):
+            raise PromptParser.ParsingException(f"while parsing Conjunction: mismatched parts/weights counts {prompts}, {weights}")
+        self.lora_weights = lora_weights or []
+        self.type = 'AND'
+
+    def __repr__(self):
+        return f"Conjunction:{self.prompts} | type {self.type} | weights {self.weights} | loras {self.lora_weights}"
+    def __eq__(self, other):
+        return type(other) is Conjunction \
+               and other.prompts == self.prompts \
+               and other.weights == self.weights \
+               and other.lora_weights == self.lora_weights
+
+
+
 class Fragment(BaseFragment):
     """
-    A Fragment is a chunk of plain text and an optional weight. The text should be passed as-is to the CLIP tokenizer.
+    A Fragment is a chunk of plain text with an optional weight. The text should be passed as-is to the text encoder.
     """
     def __init__(self, text: str, weight: float=1):
         assert(type(text) is str)
         if '\\"' in text or '\\(' in text or '\\)' in text:
             #print("Fragment converting escaped \( \) \\\" into ( ) \"")
             text = text.replace('\\(', '(').replace('\\)', ')').replace('\\"', '"')
         self.text = text
@@ -129,15 +204,16 @@
             and other.weight == self.weight
 
 class Attention():
     """
     Nestable weight control for fragments. Each object in the children array may in turn be an Attention object;
     weights should be considered to accumulate as the tree is traversed to deeper levels of nesting.
 
-    Do not traverse directly; instead obtain a FlattenedPrompt by calling Flatten() on a top-level Conjunction object.
+    Do not traverse directly. Instead, obtain a FlattenedPrompt by calling `PromptParser.flatten()` on a top-level
+    Conjunction object.
     """
     def __init__(self, weight: float, children: list):
         if type(weight) is not float:
             raise PromptParser.ParsingException(
                 f"Attention weight must be float (got {type(weight).__name__} {weight})")
         self.weight = weight
         if type(children) is not list:
@@ -208,88 +284,25 @@
     def __eq__(self, other):
         return type(other) is CrossAttentionControlSubstitute \
                and other.original == self.original \
                and other.edited == self.edited \
                and other.options == self.options
 
 
+
 class CrossAttentionControlAppend(CrossAttentionControlledFragment):
     def __init__(self, fragment: Fragment):
         self.fragment = fragment
     def __repr__(self):
         return "CrossAttentionControlAppend:",self.fragment
     def __eq__(self, other):
         return type(other) is CrossAttentionControlAppend \
                and other.fragment == self.fragment
 
 
-class Conjunction():
-    """
-    Storage for one or more Prompts or Blends, each of which is to be separately diffused and then the results merged
-    by weighted sum in latent space.
-    """
-    def __init__(self, prompts: List, weights: List[float] = None, lora_weights: List[LoraWeight] = None):
-        # force everything to be a Prompt
-        #print("making conjunction with", prompts, "types", [type(p).__name__ for p in prompts])
-        self.prompts = [x if (type(x) is Prompt
-                          or type(x) is Blend
-                          or type(x) is FlattenedPrompt)
-                      else Prompt(x) for x in prompts]
-        self.weights = [1.0]*len(self.prompts) if (weights is None or len(weights)==0) else list(weights)
-        if len(self.weights) != len(self.prompts):
-            raise PromptParser.ParsingException(f"while parsing Conjunction: mismatched parts/weights counts {prompts}, {weights}")
-        self.lora_weights = lora_weights or []
-        self.type = 'AND'
-
-    def __repr__(self):
-        return f"Conjunction:{self.prompts} | type {self.type} | weights {self.weights} | loras {self.lora_weights}"
-    def __eq__(self, other):
-        return type(other) is Conjunction \
-               and other.prompts == self.prompts \
-               and other.weights == self.weights \
-               and other.lora_weights == self.lora_weights
-
-
-class Blend():
-    """
-    Stores a Blend of multiple Prompts. To apply, build feature vectors for each of the child Prompts and then perform a
-    weighted blend of the feature vectors to produce a single feature vector that is effectively a lerp between the
-    Prompts.
-    """
-    def __init__(self, prompts: List, weights: List[float], normalize_weights: bool=True):
-        #print("making Blend with prompts", prompts, "and weights", weights)
-        weights = [1.0]*len(prompts) if (weights is None or len(weights)==0) else list(weights)
-        if len(prompts) != len(weights):
-            raise PromptParser.ParsingException(f"while parsing Blend: mismatched prompts/weights counts {prompts}, {weights}")
-        for p in prompts:
-            if type(p) is not Prompt and type(p) is not FlattenedPrompt:
-                raise(PromptParser.ParsingException(f"{type(p)} cannot be added to a Blend, only Prompts or FlattenedPrompts"))
-            for f in p.children:
-                if isinstance(f, CrossAttentionControlSubstitute):
-                    raise(PromptParser.ParsingException(f"while parsing Blend: sorry, you cannot do .swap() as part of a Blend"))
-
-        # upcast all lists to Prompt objects
-        self.prompts = [x if (type(x) is Prompt or type(x) is FlattenedPrompt)
-                         else Prompt(x)
-                        for x in prompts]
-        self.prompts = prompts
-        self.weights = weights
-        self.normalize_weights = normalize_weights
-
-    @property
-    def wants_cross_attention_control(self):
-        # blends cannot cross-attention control
-        return False
-
-
-    def __repr__(self):
-        return f"Blend:{self.prompts} | weights {' ' if self.normalize_weights else '(non-normalized) '}{self.weights}"
-    def __eq__(self, other):
-        return other.__repr__() == self.__repr__()
-
 
 class PromptParser():
 
     class ParsingException(Exception):
         pass
 
     class UnrecognizedOperatorException(ParsingException):
@@ -322,17 +335,17 @@
         return self.flatten(root[0], verbose=verbose)
 
 
 
 
     def flatten(self, root: Conjunction, verbose = False) -> Conjunction:
         """
-        Flattening a Conjunction traverses all of the nested tree-like structures in each of its Prompts or Blends,
+        Flatten a Conjunction by traversing all of the nested tree-like structures in each of its Prompts or Blends,
         producing from each of these walks a linear sequence of Fragment or CrossAttentionControlSubstitute objects
-        that can be readily tokenized without the need to walk a complex tree structure.
+        that can be readily tokenized without the need to wrangle a complex tree structure.
 
         :param root: The Conjunction to flatten.
         :return: A Conjunction containing the result of flattening each of the prompts in the passed-in root.
         """
 
         def fuse_fragments(items) -> List:
             # verbose and print("fusing fragments in ", items)
@@ -422,14 +435,22 @@
 
         return Conjunction(flattened_parts, weights, lora_weights=loras)
 
 
 
 
 def build_parser_syntax(attention_plus_base: float, attention_minus_base: float):
+    """
+    Build pyparsing parser to handle prompt syntax.
+
+    Here be dragons. If you make any changes in here it is *strongly* recommended to follow a strict TDD approach:
+    write a new unit test in `test/test_prompt_parser.py` that reflects the change you want to make, and ensure that
+    all unit tests continue to pass with the modificaton you're making.
+    """
+
     def make_operator_object(x):
         #print('making operator for', x)
         target = x[0]
         operator = x[1]
         arguments = x[2]
         if operator == '.attend':
             weight_raw = arguments[0]
```

### Comparing `compel-1.2.1/src/compel.egg-info/PKG-INFO` & `compel-2.0.0rc1/src/compel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.2.1
+Version: 2.0.0rc1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -15,25 +15,29 @@
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embedding tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
-Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
+Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)).
 
 Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
 ### Installation
 
 `pip install compel`
 
+### Documentation
+
+Documentation is [here](doc/).
+
 ### Demo
 
-see [compel-demo.ipynb](compel-demo.ipynb)
+See [compel-demo.ipynb](compel-demo.ipynb)
 
 <a target="_blank" href="https://colab.research.google.com/github/damian0815/compel/blob/main/compel-demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ### Quickstart
 
@@ -82,15 +86,17 @@
 textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
     textual_inversion_manager=textual_inversion_manager)
 ```
 
 ## Memory usage/VRAM leaks
 
-If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
+If you run into memory issues, please make sure you're running compel inside `with torch.no_grad():` blocks. 
+
+If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
 #### 1.2.1 - actually apply `.and()` weights
```

### Comparing `compel-1.2.1/src/compel.egg-info/SOURCES.txt` & `compel-2.0.0rc1/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-1.2.1/test/test_compel.py` & `compel-2.0.0rc1/test/test_compel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from typing import List, Optional
 
 import torch
 
-from src.compel import EmbeddingsProvider
+from src.compel import EmbeddingsProvider, ReturnedEmbeddingsType
 from src.compel.conditioning_scheduler import StaticConditioningScheduler, ConditioningScheduler
 from prompting_test_utils import DummyTokenizer, DummyTransformer, KNOWN_WORDS, KNOWN_WORDS_TOKEN_IDS, NullTransformer
 
 from src.compel.compel import Compel
 
 
 def make_dummy_compel():
@@ -69,14 +69,31 @@
         prompt = " ".join(KNOWN_WORDS[:3])
         conditioning = compel(prompt)
         expected_conditioning = make_test_conditioning(text_encoder, tokenizer, KNOWN_WORDS_TOKEN_IDS[:3])
         self.assertTrue(torch.allclose(expected_conditioning,
                                        conditioning,
                                        atol=1e-6))
 
+    def test_basic_prompt_multi_text_encoder(self):
+        tokenizer_1 = DummyTokenizer()
+        text_encoder_1 = DummyTransformer()
+
+        tokenizer_2 = DummyTokenizer()
+        text_encoder_2 = DummyTransformer()
+
+        compel = Compel(tokenizer=[tokenizer_1, tokenizer_2], text_encoder=[text_encoder_1, text_encoder_2],
+                        returned_embeddings_type = ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED,
+                        requires_pooled=[False, True])
+
+        prompt = " ".join(KNOWN_WORDS[:3])
+        output, pooled = compel(prompt)
+
+        assert output.shape == (1, 77, 2 * 768)
+        assert pooled.shape == (1, 768)
+
 
     def test_basic_negative_prompt(self):
         tokenizer = DummyTokenizer()
         text_encoder = DummyTransformer()
         compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder)
 
         # positive "a b c" negative "c b a" makes it to the Conditioning intact for t=0, t=0.5, t=1
@@ -89,15 +106,16 @@
         self.assert_constant_scheduling_matches_expected(conditioning_scheduler,
                                                          expected_positive_conditioning,
                                                          expected_negative_conditioning)
 
     def test_use_penultimate_layer(self):
         tokenizer = DummyTokenizer()
         text_encoder = DummyTransformer()
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, use_penultimate_clip_layer=True)
+        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder,
+                        returned_embeddings_type=ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NORMALIZED)
 
         # test "a b c" makes it to the Conditioning intact for t=0, t=0.5, t=1
         prompt = " ".join(KNOWN_WORDS[:3])
         conditioning = compel(prompt)
         expected_conditioning = make_test_conditioning(text_encoder, tokenizer,
                                                        KNOWN_WORDS_TOKEN_IDS[:3],
                                                        use_penultimate_clip_layer=True)
```

### Comparing `compel-1.2.1/test/test_embeddings_provider.py` & `compel-2.0.0rc1/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.1/test/test_prompt_parser.py` & `compel-2.0.0rc1/test/test_prompt_parser.py`

 * *Files identical despite different names*

