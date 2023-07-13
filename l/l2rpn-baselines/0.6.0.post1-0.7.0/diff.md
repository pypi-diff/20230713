# Comparing `tmp/l2rpn_baselines-0.6.0.post1.tar.gz` & `tmp/l2rpn_baselines-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2rpn_baselines-0.6.0.post1.tar", last modified: Tue Jul  5 13:25:34 2022, max compression
+gzip compressed data, was "l2rpn_baselines-0.7.0.tar", last modified: Thu Jul 13 12:25:09 2023, max compression
```

## Comparing `l2rpn_baselines-0.6.0.post1.tar` & `l2rpn_baselines-0.7.0.tar`

### file list

```diff
@@ -1,179 +1,178 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.067082 l2rpn_baselines-0.6.0.post1/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      609 2022-01-27 16:36:54.000000 l2rpn_baselines-0.6.0.post1/AUTHORS.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16725 2022-01-27 16:37:10.000000 l2rpn_baselines-0.6.0.post1/LICENSE
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16725 2022-01-27 16:37:10.000000 l2rpn_baselines-0.6.0.post1/LICENSE.md
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       67 2022-01-27 16:37:10.000000 l2rpn_baselines-0.6.0.post1/MANIFEST.in
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2923 2022-07-05 13:25:34.067082 l2rpn_baselines-0.6.0.post1/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1482 2022-01-27 16:37:10.000000 l2rpn_baselines-0.6.0.post1/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.035082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.051082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7899 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24276 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24393 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2711 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/Runner.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      927 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7650 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      710 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7085 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/train.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1446 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      785 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1051 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/deepQSimple.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3000 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/deepQ_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2039 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7048 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/evaluate.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    13151 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      168 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1182 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/doNothing.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     3825 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/eval_donothing.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      192 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/main.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      387 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15296 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2014 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6671 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     5376 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/evaluate.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     3853 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7010 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5411 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     5234 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      398 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15146 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1984 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7463 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     5386 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3277 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     5411 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      338 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1339 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9326 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7262 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3682 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    17875 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      325 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1163 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/duelQSimple.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3259 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/duelQ_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1814 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7444 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/evaluate.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    13127 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.055082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/ExpertAgent/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      259 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/ExpertAgent/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6474 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/ExpertAgent/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    23719 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/ExpertAgent/expertAgent.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4716 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/DDQN_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    26004 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/Geirina.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      962 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4164 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4166 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/generate_action_space.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4359 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/prioritized_memory.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2741 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11803 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/Kaist.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      140 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3976 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/check_your_submission.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8092 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/converter.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3707 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3905 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/models.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3948 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/sublayer.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       34 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11849 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/agent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8009 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/converter.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3970 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/models.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3954 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/sublayer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      763 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/submission.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/utils/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      441 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/utils/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      418 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/utils/zip_dir.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3302 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/utils/zip_for_codalab.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      358 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7327 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1262 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15449 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8656 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6074 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/study.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    17952 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7848 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/Action_reduced_list.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24276 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/ActorCritic_Agent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2630 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/Runner.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      708 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7400 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      710 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/run_grid2viz.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6967 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/train.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1446 2022-01-27 16:38:28.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Multithreading_agent/user_environment_make.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.059082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      706 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      549 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2907 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/make_agent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    53226 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/optimCVXPY.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      699 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4179 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/env_rllib.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8761 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11078 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/rllibagent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10417 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1072 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10730 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13047 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/train.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12448 2022-07-05 13:24:16.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/utils.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13139 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      956 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     3696 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4070 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      293 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6946 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1284 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/sacOld.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13601 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/sacOld_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3033 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/sacOld_NNParam.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    14025 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      321 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     5145 2022-07-05 13:24:16.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3277 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/experienceBuffer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15513 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/sliceRDQN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1570 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10790 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5440 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/slice_util.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     5644 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/train.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1005 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     3957 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/evaluate.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6151 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/template.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     2603 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/train.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      919 2022-07-05 13:24:16.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.063082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1576 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10366 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/baseDeepQ.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2225 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/cli_eval.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1990 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/cli_train.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    51498 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/deepQAgent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8560 2022-07-05 13:24:16.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/gymAgent.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16162 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/gymenv_custom.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2253 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/make_multi_env.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11336 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/nnParam.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2416 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/replayBuffer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1782 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/save_log_gif.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      789 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/str2bool.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2459 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/train_generic.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16056 2022-06-07 15:19:50.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/trainingParam.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      631 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/waring_msgs.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4138 2022-01-27 16:38:29.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/zip_for_codalab.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2022-07-05 13:25:34.051082 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2923 2022-07-05 13:25:33.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6312 2022-07-05 13:25:33.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2022-07-05 13:25:33.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2020-05-11 08:43:56.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/not-zip-safe
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      366 2022-07-05 13:25:33.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       16 2022-07-05 13:25:33.000000 l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2022-07-05 13:25:34.067082 l2rpn_baselines-0.6.0.post1/setup.cfg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2644 2022-07-05 13:24:16.000000 l2rpn_baselines-0.6.0.post1/setup.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       67 2020-07-05 18:33:35.000000 l2rpn_baselines-0.7.0/MANIFEST.in
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2963 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/PKG-INFO
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1496 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/README.md
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.878962 l2rpn_baselines-0.7.0/l2rpn_baselines/
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.906962 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7899 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    24276 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    24393 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2711 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Runner.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      927 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7650 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      710 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7085 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1446 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.910962 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      253 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    20167 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/baseline.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4642 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2520 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.914962 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      785 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1051 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQSimple.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3000 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2039 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7048 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    13151 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.918962 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      168 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1182 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/doNothing.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3825 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/eval_donothing.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      192 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/main.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.930962 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      387 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15296 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2014 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6671 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5376 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3853 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7010 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5411 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5234 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.938962 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      398 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15146 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1984 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7463 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5386 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3277 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5411 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.942962 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      338 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1339 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     9326 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7262 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3682 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    17875 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.950962 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      325 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1163 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQSimple.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3259 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1814 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7444 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    13127 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.950962 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      259 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6474 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    23719 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/expertAgent.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.958962 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4716 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/DDQN_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    26004 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/Geirina.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      962 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4164 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4166 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/generate_action_space.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4359 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/prioritized_memory.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2741 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.970962 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11803 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/Kaist.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      140 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3976 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/check_your_submission.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8092 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/converter.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3707 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3905 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/models.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3948 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/sublayer.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.978962 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       34 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11849 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/agent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8009 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/converter.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3970 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/models.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3954 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/sublayer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      763 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/submission.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.982962 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      441 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      418 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/zip_dir.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3302 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/zip_for_codalab.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.990962 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      358 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7327 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1262 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15449 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8656 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6074 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/study.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    17952 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.994962 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      706 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      549 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2907 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/make_agent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    53226 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/optimCVXPY.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.998962 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      699 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4179 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/env_rllib.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8761 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11078 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/rllibagent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10417 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.006962 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1072 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10730 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13122 2022-11-29 14:09:24.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12448 2022-07-11 09:20:27.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/utils.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.010962 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3995 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/OPF_saveload_investigation.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    17638 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      956 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3696 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4264 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.018962 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      293 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6946 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1284 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13601 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3033 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NNParam.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    14025 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.026962 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      321 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5145 2022-11-29 14:09:20.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3277 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/experienceBuffer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15513 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1570 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10790 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5440 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/slice_util.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5644 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.030962 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1005 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3957 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6151 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/template.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     2603 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.030962 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2010 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/TopoOracleAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      259 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8267 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     9436 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      913 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1576 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10366 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/baseDeepQ.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2225 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_eval.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1990 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    51498 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/deepQAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8560 2023-01-24 08:55:34.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16162 2023-02-03 14:21:58.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymenv_custom.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2253 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/make_multi_env.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11336 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/nnParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2416 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/replayBuffer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1782 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/save_log_gif.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      789 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/str2bool.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2459 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/train_generic.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16056 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/trainingParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      631 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/waring_msgs.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4138 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/zip_for_codalab.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.894962 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2963 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/PKG-INFO
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6275 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/SOURCES.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/dependency_links.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-02-03 09:33:41.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/not-zip-safe
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      401 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/requires.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       16 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/top_level.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       38 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/setup.cfg
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2685 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/setup.py
```

### Comparing `l2rpn_baselines-0.6.0.post1/PKG-INFO` & `l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: l2rpn_baselines
-Version: 0.6.0.post1
+Name: l2rpn-baselines
+Version: 0.7.0
 Summary: L2RPN Baselines a repository to host baselines for l2rpn competitions.
 Home-page: https://github.com/rte-france/L2RPN_Baselines
 Author: Benjamin DONNOT
 Author-email: benjamin.donnot@rte-france.com
 License: MPL
 Description: # L2RPN_Baselines
         Repository hosting reference baselines for the [L2RPN challenge](https://l2rpn.chalearn.org/)
@@ -29,38 +29,38 @@
         
         # Contribute
         
         We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
         
         # Get started with a baseline
         
-        Say you want to know how you compared with the "DoubleDuelingDQN" baseline implementation in this repository (for the
+        Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
         sake of this example).
         
         ## Train it (optional)
         As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
         
         ```python
         import grid2op
-        from l2rpn_baselines.DoubleDuelingDQN import train
-        env = grid2op.make()
+        from l2rpn_baselines.PPO_SB3 import train
+        env = grid2op.make("l2rpn_case14_sandbox")
         res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
         ```
         
         You can have more information about extra argument of the "train" function in the 
         [CONTRIBUTE](/CONTRIBUTE.md) file.
         
         ## Evaluate it
         Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
         
         ```python
         import grid2op
-        from l2rpn_baselines.DoubleDuelingDQN import evaluate
-        env = grid2op.make()
-        res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT.h5", nb_episode=10)
+        from l2rpn_baselines.PPO_SB3 import evaluate
+        env = grid2op.make("l2rpn_case14_sandbox")
+        res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
         ```
         
         You can have more information about extra argument of the "evaluate" function in the 
         [CONTRIBUTE](/CONTRIBUTE.md) file.
         
 Keywords: ML powergrid optmization RL power-systems
 Platform: UNKNOWN
@@ -71,11 +71,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: optional
+Provides-Extra: CurriculumAgent
 Provides-Extra: PPO_RLLIB
 Provides-Extra: PPO_SB3
+Provides-Extra: docs
+Provides-Extra: optional
```

### Comparing `l2rpn_baselines-0.6.0.post1/README.md` & `l2rpn_baselines-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 
 # Contribute
 
 We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
 
 # Get started with a baseline
 
-Say you want to know how you compared with the "DoubleDuelingDQN" baseline implementation in this repository (for the
+Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
 sake of this example).
 
 ## Train it (optional)
 As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
 
 ```python
 import grid2op
-from l2rpn_baselines.DoubleDuelingDQN import train
-env = grid2op.make()
+from l2rpn_baselines.PPO_SB3 import train
+env = grid2op.make("l2rpn_case14_sandbox")
 res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
 ```
 
 You can have more information about extra argument of the "train" function in the 
 [CONTRIBUTE](/CONTRIBUTE.md) file.
 
 ## Evaluate it
 Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
 
 ```python
 import grid2op
-from l2rpn_baselines.DoubleDuelingDQN import evaluate
-env = grid2op.make()
-res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT.h5", nb_episode=10)
+from l2rpn_baselines.PPO_SB3 import evaluate
+env = grid2op.make("l2rpn_case14_sandbox")
+res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
 ```
 
 You can have more information about extra argument of the "evaluate" function in the 
 [CONTRIBUTE](/CONTRIBUTE.md) file.
```

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/Runner.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Runner.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/deepQSimple.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQSimple.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/deepQ_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DeepQSimple/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/doNothing.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/doNothing.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoNothing/eval_donothing.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/eval_donothing.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingDQN/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DoubleDuelingRDQN/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQLeapNet/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/duelQSimple.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQSimple.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/duelQ_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/DuelQSimple/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/ExpertAgent/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/ExpertAgent/expertAgent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/expertAgent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/DDQN_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/DDQN_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/Geirina.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/Geirina.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/generate_action_space.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/generate_action_space.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/prioritized_memory.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/prioritized_memory.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Geirina/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/Kaist.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/Kaist.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/check_your_submission.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/check_your_submission.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/converter.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/converter.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/models.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/models.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/sublayer.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/sublayer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/agent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/agent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/converter.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/converter.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/models.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/models.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/sublayer.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/sublayer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/submission/submission.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/submission.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Kaist/utils/zip_for_codalab.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/zip_for_codalab.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/study.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/study.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/LeapNetEncoded/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/make_agent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/make_agent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/OptimCVXPY/optimCVXPY.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/optimCVXPY.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/env_rllib.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/env_rllib.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/rllibagent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/rllibagent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_RLLIB/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
           name="PPO_SB3",
           iterations=1,
           save_path=None,
           load_path=None,
           net_arch=None,
           logs_dir=None,
           learning_rate=3e-4,
+          checkpoint_callback=None,
           save_every_xxx_steps=None,
           model_policy=MlpPolicy,
           obs_attr_to_keep=copy.deepcopy(default_obs_attr_to_keep),
           obs_space_kwargs=None,
           act_attr_to_keep=copy.deepcopy(default_act_attr_to_keep),
           act_space_kwargs=None,
           policy_kwargs=None,
@@ -252,24 +253,24 @@
                 ("subtract" in obs_space_kwargs and attr_nm in obs_space_kwargs["subtract"]) 
                ):
                 # attribute is scaled elsewhere
                 continue
             env_gym.observation_space.normalize_attr(attr_nm)
     
     # Save a checkpoint every "save_every_xxx_steps" steps
-    checkpoint_callback = None
-    if save_every_xxx_steps is not None:
-        if save_path is None:
-            warnings.warn("save_every_xxx_steps is set, but no path are "
-                          "set to save the model (save_path is None). No model "
-                          "will be saved.")
-        else:
-            checkpoint_callback = CheckpointCallback(save_freq=save_every_xxx_steps,
-                                                     save_path=my_path,
-                                                     name_prefix=name)
+    if checkpoint_callback is None:
+        if save_every_xxx_steps is not None:
+            if save_path is None:
+                warnings.warn("save_every_xxx_steps is set, but no path are "
+                              "set to save the model (save_path is None). No model "
+                              "will be saved.")
+            else:
+                checkpoint_callback = CheckpointCallback(save_freq=save_every_xxx_steps,
+                                                        save_path=my_path,
+                                                        name_prefix=name)
 
     # define the policy
     if load_path is None:
         if policy_kwargs is None:
             policy_kwargs = {}
         if net_arch is not None:
             policy_kwargs["net_arch"] = net_arch
```

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PPO_SB3/utils.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/utils.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,89 @@
-import logging
-
-import numpy as np
-import pandas as pd
-
-import pandapower as pp
-
-
-def find_value_for_pp_bus(grid: pp.pandapowerNet,
-                          voltages_from: np.ndarray,
-                          voltages_to: np.ndarray,
-                          bus: int):
-    # map line extremity voltage readings to the correct pandapower bus
-    bus_vn_kv = grid.bus.loc[bus, "vn_kv"]
-    for idx, line in enumerate(grid.line.itertuples()):
-        if line.from_bus == bus:
-            return voltages_from[idx] / bus_vn_kv
-        elif line.to_bus == bus:
-            return voltages_to[idx] / bus_vn_kv
-    for idx, trafo in enumerate(grid.trafo.itertuples()):
-        if trafo.hv_bus == bus:
-            return voltages_from[len(grid.line) + idx] / bus_vn_kv
-        elif trafo.lv_bus == bus:
-            return voltages_to[len(grid.line) + idx] / bus_vn_kv
-    return None
-
-
-def calc_losses(grid: pp.pandapowerNet):
-    # calculate grid losses
-    return grid.res_gen.p_mw.sum() + grid.res_ext_grid.p_mw.sum() + grid.res_sgen.p_mw.sum() - grid.load.p_mw.sum()
-
-
-def make_zero_idx(elements: pd.DataFrame,
-                  pd_indices,
-                  offset: int = 0):
-    # translate arbitrary pandas indices to 0-based numpy array indices
-    return [elements.index.get_loc(lidx) + offset for lidx in pd_indices]
-
-
-def run_opf(grid: pp.pandapowerNet,
-            min_loss_reduction_mwt: float,
-            acceptable_loading: float,
-            opf_type: str,
-            asset: str = "",
-            logger=logging.getLogger()):
-    loss_before = calc_losses(grid)
-    line_loading_before = grid.res_line.loading_percent.max()
-    trafo_loading_before = (grid.res_trafo.i_hv_ka / grid.trafo.max_i_ka * 100.).max()
-    try:
-        if opf_type == "pypower":
-            pp.runopp(grid)  # pypower OPF
-        elif opf_type == "powermodels":
-            grid.line["in_service"] = True
-            grid.trafo["in_service"] = True
-            pp.runpm_ots(grid, pm_nl_solver="ipopt", pm_model="ACPPowerModel")  # PowerModels.jl OPF
-            grid.line.loc[:, "in_service"] = grid.res_line.loc[:, "in_service"].values.astype(bool)
-            grid.trafo.loc[:, "in_service"] = grid.res_trafo.loc[:, "in_service"].values.astype(bool)
-        generation = np.array(grid.res_gen.p_mw.tolist() + grid.res_ext_grid.p_mw.tolist())
-        losses_avoided = loss_before - calc_losses(grid)
-        line_loading_after = grid.res_line.loading_percent.max()
-        trafo_loading_after = (grid.res_trafo.i_hv_ka / grid.trafo.max_i_ka * 100.).max()
-        use_opf_results = False
-        # three conditions for using the OPF results:
-        # 1. transformer was overloaded before and is now less overloaded
-        # 2. line was overloaded before and is now less overloaded
-        # 3. losses are minimized at least by "min_loss_reduction_mwt" while all loadings are acceptably low
-        if trafo_loading_before > acceptable_loading and trafo_loading_after < trafo_loading_before:
-            use_opf_results = True
-        if line_loading_before > acceptable_loading and line_loading_after < line_loading_before:
-            use_opf_results = True
-        if losses_avoided > min_loss_reduction_mwt and line_loading_after < acceptable_loading and trafo_loading_after < acceptable_loading:
-            use_opf_results = True
-        if use_opf_results:
-            logger.info(f"Losses avoided: {losses_avoided:.3f} MW (max. loading: {line_loading_after:.1f}% [{line_loading_after - line_loading_before:.1f}%] "
-                        f"/ Trafo: {trafo_loading_after:.1f}% [{trafo_loading_after - trafo_loading_before:.1f}%])")
-            return generation, grid.line.in_service, grid.trafo.in_service, True
-        return np.zeros(len(grid.gen)), grid.line.in_service, grid.trafo.in_service, False
-    except pp.optimal_powerflow.OPFNotConverged:
-        asset_str = f"if asset #{asset} is out of service" if len(asset) else ""
-        logger.info(f"OPF failed {asset_str}")
-        return np.zeros(len(grid.gen)), grid.line.in_service, grid.trafo.in_service, False
+import logging
+
+import numpy as np
+import pandas as pd
+
+import pandapower as pp
+
+
+def find_value_for_pp_bus(grid: pp.pandapowerNet,
+                          voltages_from: np.ndarray,
+                          voltages_to: np.ndarray,
+                          bus: int):
+    # map line extremity voltage readings to the correct pandapower bus
+    bus_vn_kv = grid.bus.loc[bus, "vn_kv"]
+    for idx, line in enumerate(grid.line.itertuples()):
+        if line.from_bus == bus:
+            return voltages_from[idx] / bus_vn_kv
+        elif line.to_bus == bus:
+            
+            return voltages_to[idx] / bus_vn_kv
+    for idx, trafo in enumerate(grid.trafo.itertuples()):
+        if trafo.hv_bus == bus:
+            
+            return voltages_from[len(grid.line) + idx] / bus_vn_kv
+        elif trafo.lv_bus == bus:
+            
+            return voltages_to[len(grid.line) + idx] / bus_vn_kv
+    return None
+
+
+def calc_losses(grid: pp.pandapowerNet):
+    # calculate grid losses
+    return grid.res_gen.p_mw.sum() + grid.res_ext_grid.p_mw.sum() + grid.res_sgen.p_mw.sum() - grid.load.p_mw.sum()
+
+
+def make_zero_idx(elements: pd.DataFrame,
+                  pd_indices,
+                  offset: int = 0):
+    # translate arbitrary pandas indices to 0-based numpy array indices
+    return [elements.index.get_loc(lidx) + offset for lidx in pd_indices]
+
+
+def run_opf(grid: pp.pandapowerNet,
+            min_loss_reduction_mwt: float,
+            acceptable_loading: float,
+            opf_type: str,
+            asset: str = "",
+            logger=logging.getLogger()):
+    loss_before = calc_losses(grid)
+    line_loading_before = grid.res_line.loading_percent.max()
+    trafo_loading_before = grid.res_trafo.loading_percent.max()
+    try:
+        if opf_type == "pypower":
+        
+            grid.ext_grid["min_p_mw"][0] = -100
+            grid.ext_grid["max_p_mw"][0] = 200
+        
+            pp.runopp(grid)  # pypower OPF
+        elif opf_type == "powermodels":
+            grid.line["in_service"] = True
+            grid.trafo["in_service"] = True
+            pp.runpm_ots(grid, pm_nl_solver="ipopt", pm_model="ACPPowerModel")  # PowerModels.jl OPF
+            grid.line.loc[:, "in_service"] = grid.res_line.loc[:, "in_service"].values.astype(bool)
+            grid.trafo.loc[:, "in_service"] = grid.res_trafo.loc[:, "in_service"].values.astype(bool)
+        generation = np.array(grid.res_gen.p_mw.tolist() + grid.res_ext_grid.p_mw.tolist())
+        losses_avoided = loss_before - calc_losses(grid)
+        line_loading_after = grid.res_line.loading_percent.max()
+        trafo_loading_after = grid.res_trafo.loading_percent.max()
+        use_opf_results = False
+
+        # three conditions for using the OPF results:
+        # 1. transformer was overloaded before and is now less overloaded
+        # 2. line was overloaded before and is now less overloaded
+        # 3. losses are minimized at least by "min_loss_reduction_mwt" while all loadings are acceptably low
+        if trafo_loading_before > acceptable_loading and trafo_loading_after < trafo_loading_before: 
+            use_opf_results = True
+        if line_loading_before > acceptable_loading and line_loading_after < line_loading_before:
+            use_opf_results = True
+        if losses_avoided > min_loss_reduction_mwt and line_loading_after < acceptable_loading and trafo_loading_after < acceptable_loading:
+            use_opf_results = True
+        if use_opf_results:
+           logger.info(f"Losses avoided: {losses_avoided:.3f} MW (max. loading: {line_loading_after:.1f}% [{line_loading_after - line_loading_before:.1f}%] "
+                       f"/ Trafo: {trafo_loading_after:.1f}% [{trafo_loading_after - trafo_loading_before:.1f}%])")
+           return generation, grid.line.in_service, grid.trafo.in_service, True
+        return np.zeros(len(grid.gen)), grid.line.in_service, grid.trafo.in_service, False
+    except pp.optimal_powerflow.OPFNotConverged:
+        asset_str = f"if asset #{asset} is out of service" if len(asset) else ""
+        logger.info(f"OPF failed {asset_str}")
+        return np.zeros(len(grid.gen)), grid.line.in_service, grid.trafo.in_service, False
```

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/sacOld.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/sacOld_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/sacOld_NNParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SACOld/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/experienceBuffer.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/experienceBuffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/sliceRDQN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/slice_util.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/slice_util.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/SliceRDQN/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/evaluate.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/template.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/template.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/Template/train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
-__version__ = "0.6.0.post1"
+__version__ = "0.7.0"
 
 all_baselines_li = [
     "Template",
     "DoNothing",
     "ExpertAgent",
     "PPO_RLLIB",
     "PPO_SB3",
```

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/__init__.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/baseDeepQ.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/baseDeepQ.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/cli_eval.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_eval.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/cli_train.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/deepQAgent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/deepQAgent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/gymAgent.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymAgent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/gymenv_custom.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymenv_custom.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/make_multi_env.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/make_multi_env.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/nnParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/nnParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/replayBuffer.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/replayBuffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/save_log_gif.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/save_log_gif.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/str2bool.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/str2bool.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/train_generic.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/train_generic.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/trainingParam.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/trainingParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/waring_msgs.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/waring_msgs.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines/utils/zip_for_codalab.py` & `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/zip_for_codalab.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/PKG-INFO` & `l2rpn_baselines-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: l2rpn-baselines
-Version: 0.6.0.post1
+Name: l2rpn_baselines
+Version: 0.7.0
 Summary: L2RPN Baselines a repository to host baselines for l2rpn competitions.
 Home-page: https://github.com/rte-france/L2RPN_Baselines
 Author: Benjamin DONNOT
 Author-email: benjamin.donnot@rte-france.com
 License: MPL
 Description: # L2RPN_Baselines
         Repository hosting reference baselines for the [L2RPN challenge](https://l2rpn.chalearn.org/)
@@ -29,38 +29,38 @@
         
         # Contribute
         
         We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
         
         # Get started with a baseline
         
-        Say you want to know how you compared with the "DoubleDuelingDQN" baseline implementation in this repository (for the
+        Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
         sake of this example).
         
         ## Train it (optional)
         As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
         
         ```python
         import grid2op
-        from l2rpn_baselines.DoubleDuelingDQN import train
-        env = grid2op.make()
+        from l2rpn_baselines.PPO_SB3 import train
+        env = grid2op.make("l2rpn_case14_sandbox")
         res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
         ```
         
         You can have more information about extra argument of the "train" function in the 
         [CONTRIBUTE](/CONTRIBUTE.md) file.
         
         ## Evaluate it
         Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
         
         ```python
         import grid2op
-        from l2rpn_baselines.DoubleDuelingDQN import evaluate
-        env = grid2op.make()
-        res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT.h5", nb_episode=10)
+        from l2rpn_baselines.PPO_SB3 import evaluate
+        env = grid2op.make("l2rpn_case14_sandbox")
+        res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
         ```
         
         You can have more information about extra argument of the "evaluate" function in the 
         [CONTRIBUTE](/CONTRIBUTE.md) file.
         
 Keywords: ML powergrid optmization RL power-systems
 Platform: UNKNOWN
@@ -71,11 +71,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: optional
+Provides-Extra: CurriculumAgent
 Provides-Extra: PPO_RLLIB
 Provides-Extra: PPO_SB3
+Provides-Extra: docs
+Provides-Extra: optional
```

### Comparing `l2rpn_baselines-0.6.0.post1/l2rpn_baselines.egg-info/SOURCES.txt` & `l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-AUTHORS.txt
-LICENSE
-LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 l2rpn_baselines/__init__.py
 l2rpn_baselines.egg-info/PKG-INFO
 l2rpn_baselines.egg-info/SOURCES.txt
 l2rpn_baselines.egg-info/dependency_links.txt
@@ -16,14 +13,18 @@
 l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py
 l2rpn_baselines/AsynchronousActorCritic/Runner.py
 l2rpn_baselines/AsynchronousActorCritic/__init__.py
 l2rpn_baselines/AsynchronousActorCritic/evaluate.py
 l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py
 l2rpn_baselines/AsynchronousActorCritic/train.py
 l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py
+l2rpn_baselines/CurriculumAgent/__init__.py
+l2rpn_baselines/CurriculumAgent/baseline.py
+l2rpn_baselines/CurriculumAgent/evaluate.py
+l2rpn_baselines/CurriculumAgent/train.py
 l2rpn_baselines/DeepQSimple/__init__.py
 l2rpn_baselines/DeepQSimple/deepQSimple.py
 l2rpn_baselines/DeepQSimple/deepQ_NN.py
 l2rpn_baselines/DeepQSimple/deepQ_NNParam.py
 l2rpn_baselines/DeepQSimple/evaluate.py
 l2rpn_baselines/DeepQSimple/train.py
 l2rpn_baselines/DoNothing/__init__.py
@@ -87,35 +88,28 @@
 l2rpn_baselines/LeapNetEncoded/__init__.py
 l2rpn_baselines/LeapNetEncoded/evaluate.py
 l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py
 l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py
 l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py
 l2rpn_baselines/LeapNetEncoded/study.py
 l2rpn_baselines/LeapNetEncoded/train.py
-l2rpn_baselines/Multithreading_agent/Action_reduced_list.py
-l2rpn_baselines/Multithreading_agent/ActorCritic_Agent.py
-l2rpn_baselines/Multithreading_agent/Runner.py
-l2rpn_baselines/Multithreading_agent/__init__.py
-l2rpn_baselines/Multithreading_agent/evaluate.py
-l2rpn_baselines/Multithreading_agent/run_grid2viz.py
-l2rpn_baselines/Multithreading_agent/train.py
-l2rpn_baselines/Multithreading_agent/user_environment_make.py
 l2rpn_baselines/OptimCVXPY/__init__.py
 l2rpn_baselines/OptimCVXPY/evaluate.py
 l2rpn_baselines/OptimCVXPY/make_agent.py
 l2rpn_baselines/OptimCVXPY/optimCVXPY.py
 l2rpn_baselines/PPO_RLLIB/__init__.py
 l2rpn_baselines/PPO_RLLIB/env_rllib.py
 l2rpn_baselines/PPO_RLLIB/evaluate.py
 l2rpn_baselines/PPO_RLLIB/rllibagent.py
 l2rpn_baselines/PPO_RLLIB/train.py
 l2rpn_baselines/PPO_SB3/__init__.py
 l2rpn_baselines/PPO_SB3/evaluate.py
 l2rpn_baselines/PPO_SB3/train.py
 l2rpn_baselines/PPO_SB3/utils.py
+l2rpn_baselines/PandapowerOPFAgent/OPF_saveload_investigation.py
 l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py
 l2rpn_baselines/PandapowerOPFAgent/__init__.py
 l2rpn_baselines/PandapowerOPFAgent/evaluate.py
 l2rpn_baselines/PandapowerOPFAgent/pp_functions.py
 l2rpn_baselines/SACOld/__init__.py
 l2rpn_baselines/SACOld/evaluate.py
 l2rpn_baselines/SACOld/sacOld.py
@@ -130,14 +124,18 @@
 l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py
 l2rpn_baselines/SliceRDQN/slice_util.py
 l2rpn_baselines/SliceRDQN/train.py
 l2rpn_baselines/Template/__init__.py
 l2rpn_baselines/Template/evaluate.py
 l2rpn_baselines/Template/template.py
 l2rpn_baselines/Template/train.py
+l2rpn_baselines/TopoOracleAgent/TopoOracleAgent.py
+l2rpn_baselines/TopoOracleAgent/__init__.py
+l2rpn_baselines/TopoOracleAgent/evaluate.py
+l2rpn_baselines/TopoOracleAgent/train.py
 l2rpn_baselines/utils/__init__.py
 l2rpn_baselines/utils/baseDeepQ.py
 l2rpn_baselines/utils/cli_eval.py
 l2rpn_baselines/utils/cli_train.py
 l2rpn_baselines/utils/deepQAgent.py
 l2rpn_baselines/utils/gymAgent.py
 l2rpn_baselines/utils/gymenv_custom.py
```

### Comparing `l2rpn_baselines-0.6.0.post1/setup.py` & `l2rpn_baselines-0.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
 import setuptools
 from setuptools import setup
-__version__ = "0.6.0.post1"
+__version__ = "0.7.0"
 
 
 pkgs = {
     "required": [
         "grid2op",
         "statsmodels>=0.11.1",
         "scipy>=1.4.1",
@@ -33,15 +33,16 @@
                      "Keras>=2.3.1",
                      "torch>=1.4.0",
                      "scikit-learn>=0.22.2",
                      ],
         "PPO_RLLIB": ["ray[rllib]",
                       "jsonpickle",
                       "lightsim2grid"],
-        "PPO_SB3": ["stable_baselines3", "lightsim2grid"]
+        "PPO_SB3": ["stable_baselines3", "lightsim2grid"],
+        "CurriculumAgent":["curriculumagent"]
     }
 }
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

