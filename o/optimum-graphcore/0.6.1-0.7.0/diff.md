# Comparing `tmp/optimum-graphcore-0.6.1.tar.gz` & `tmp/optimum-graphcore-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-graphcore-0.6.1.tar", last modified: Thu May 25 15:28:44 2023, max compression
+gzip compressed data, was "optimum-graphcore-0.7.0.tar", last modified: Thu Jul 13 12:42:16 2023, max compression
```

## Comparing `optimum-graphcore-0.6.1.tar` & `optimum-graphcore-0.7.0.tar`

### file list

```diff
@@ -1,123 +1,126 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     8905 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.713887 optimum-graphcore-0.6.1/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2680 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/data/
--rw-rw-r--   0 michael   (1000) michael   (1000)      885 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/data/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5927 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/data/data_collator.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/
--rw-rw-r--   0 michael   (1000) michael   (1000)      204 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)      211 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 michael   (1000) michael   (1000)      311 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4641 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      227 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17507 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1732 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/generation/
--rw-rw-r--   0 michael   (1000) michael   (1000)      709 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13526 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/attention_mixin.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6733 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/logits_process.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    20117 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/on_device_generation.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    86113 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/generation/utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    39210 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/ipu_configuration.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5749 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/modelcard.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    30935 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/modeling_utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/models/
--rw-rw-r--   0 michael   (1000) michael   (1000)      897 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.717887 optimum-graphcore-0.6.1/optimum/graphcore/models/bart/
--rw-rw-r--   0 michael   (1000) michael   (1000)      883 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bart/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    49792 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bart/modeling_bart.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1032 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6831 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/bert_fused_attention.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22148 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/bert/modeling_bert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/
--rw-rw-r--   0 michael   (1000) michael   (1000)      849 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2801 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/modeling_convnext.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1016 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/optimized_convnextlayer.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/
--rw-rw-r--   0 michael   (1000) michael   (1000)      978 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22415 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/modeling_deberta.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1035 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15150 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/modeling_distilbert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      924 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15345 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1606 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1918 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10205 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_attention.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3334 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_convolution.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2929 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_ffn.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    35160 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/modeling_groupbert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/
--rw-rw-r--   0 michael   (1000) michael   (1000)      848 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6667 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/ipu_layer_drop.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8003 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/modeling_hubert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/
--rw-rw-r--   0 michael   (1000) michael   (1000)      843 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6199 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/modeling_lxmert.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/
--rw-rw-r--   0 michael   (1000) michael   (1000)      841 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27199 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/modeling_mt5.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1017 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    14463 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/modeling_roberta.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/t5/
--rw-rw-r--   0 michael   (1000) michael   (1000)      839 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/t5/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    21486 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/t5/modeling_t5.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/vit/
--rw-rw-r--   0 michael   (1000) michael   (1000)      839 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/vit/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2156 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/vit/modeling_vit.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      866 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4396 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7587 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    24383 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/
--rw-rw-r--   0 michael   (1000) michael   (1000)      972 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2193 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/feature_extraction_whisper.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    21496 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/modeling_whisper.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1226 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/processing_whisper.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)    20004 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1208 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/fill_mask.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3060 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/text2text_generation.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3233 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/token_classification.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3890 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/pipelines/zero_shot_classification.py
--rw-rw-r--   0 michael   (1000) michael   (1000)   107693 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer_pt_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12049 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer_seq2seq.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2266 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/trainer_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    47190 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/optimum/graphcore/training_args.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2879 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/optimum/graphcore/training_args_seq2seq.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum/graphcore/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1128 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/optimum/graphcore/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-05-25 15:19:12.000000 optimum-graphcore-0.6.1/optimum/graphcore/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.721887 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     4214 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 12:57:36.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      248 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-05-25 15:28:44.000000 optimum-graphcore-0.6.1/optimum_graphcore.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)      674 2023-04-05 12:52:34.000000 optimum-graphcore-0.6.1/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      811 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2236 2023-05-25 15:19:28.000000 optimum-graphcore-0.6.1/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-25 15:28:44.725887 optimum-graphcore-0.6.1/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    22929 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3338 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/tests/test_examples_match_transformers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    25361 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_ipu_configuration.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1809 2023-02-15 10:20:19.000000 optimum-graphcore-0.6.1/tests/test_modeling_common.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5702 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_modeling_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12759 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_pipelined_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    61891 2023-05-25 15:19:02.000000 optimum-graphcore-0.6.1/tests/test_trainer.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8905 2023-05-25 15:19:02.000000 optimum-graphcore-0.7.0/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.409396 optimum-graphcore-0.7.0/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2776 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/data/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      885 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/data/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5974 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/data/data_collator.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      808 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      815 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      915 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5563 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      831 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      852 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      852 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    19051 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2335 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/safety_checker.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/generation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      740 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17488 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/attention_mixin.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10938 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/logits_process.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20324 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/on_device_generation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    94451 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/generation/utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    38450 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/ipu_configuration.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5749 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/modelcard.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    33652 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/modeling_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      954 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/bart/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      940 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bart/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    50037 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bart/modeling_bart.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1089 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6853 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/bert_fused_attention.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22296 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/bert/modeling_bert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      906 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2801 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/modeling_convnext.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1711 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/optimized_convnextlayer.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1035 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22415 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/modeling_deberta.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1092 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15150 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/modeling_distilbert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      981 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15345 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/modeling_gpt2.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2342 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/optimized_gpt2_attn.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.413396 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1915 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10189 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_attention.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3297 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_convolution.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2892 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_ffn.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35135 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/modeling_groupbert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      905 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6676 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/ipu_layer_drop.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8092 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/modeling_hubert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      900 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6262 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/modeling_lxmert.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      898 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27287 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/modeling_mt5.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1074 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14589 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/modeling_roberta.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      921 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      777 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/configuration_t5.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25981 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/t5/modeling_t5.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/vit/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      896 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/vit/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2217 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/vit/modeling_vit.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      923 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4484 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7591 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    24472 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1029 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2256 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/feature_extraction_whisper.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    28245 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/modeling_whisper.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1226 2023-05-25 15:19:02.000000 optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/processing_whisper.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20752 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5609 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/automatic_speech_recognition.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1873 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/fill_mask.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3696 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/text2text_generation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1908 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/token_classification.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4471 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/pipelines/zero_shot_classification.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)   107720 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer_pt_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17320 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer_seq2seq.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2331 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/trainer_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    46931 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/training_args.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4528 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/optimum/graphcore/training_args_seq2seq.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum/graphcore/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1128 2023-02-15 10:20:19.000000 optimum-graphcore-0.7.0/optimum/graphcore/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      697 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/optimum/graphcore/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9947 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4352 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-05 12:57:36.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      285 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-07-13 12:42:16.000000 optimum-graphcore-0.7.0/optimum_graphcore.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1098 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      112 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3021 2023-07-13 12:41:40.000000 optimum-graphcore-0.7.0/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-13 12:42:16.417395 optimum-graphcore-0.7.0/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    23442 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3395 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25297 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_ipu_configuration.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     1808 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_modeling_common.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6691 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_modeling_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13055 2023-07-13 12:41:16.000000 optimum-graphcore-0.7.0/tests/test_pipelined_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    61608 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_trainer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5653 2023-07-13 12:41:07.000000 optimum-graphcore-0.7.0/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-graphcore-0.6.1/LICENSE` & `optimum-graphcore-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/MANIFEST.in` & `optimum-graphcore-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/PKG-INFO` & `optimum-graphcore-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-graphcore
-Version: 0.6.1
+Version: 0.7.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://huggingface.co/hardware
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,training,ipu
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `optimum-graphcore-0.6.1/README.md` & `optimum-graphcore-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 #  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -47,15 +48,18 @@
 from .models.roberta import (
     PipelinedRobertaForMaskedLM,
     PipelinedRobertaForMultipleChoice,
     PipelinedRobertaForQuestionAnswering,
     PipelinedRobertaForSequenceClassification,
     PipelinedRobertaForTokenClassification,
 )
-from .models.t5 import PipelinedT5ForConditionalGeneration
+from .models.t5 import (
+    PipelinedT5ForConditionalGeneration,
+    PipelinedT5EncoderModel,
+)
 from .models.vit import PipelinedViTForImageClassification
 from .models.wav2vec2 import PipelinedWav2Vec2ForPreTraining
 from .pipelines import IPUFillMaskPipeline, IPUTokenClassificationPipeline, pipeline
 from .trainer import IPUTrainer, IPUTrainerState
 from .trainer_seq2seq import IPUSeq2SeqTrainer
 from .training_args import IPUTrainingArguments
 from .training_args_seq2seq import IPUSeq2SeqTrainingArguments
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/data/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/data/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/data/data_collator.py` & `optimum-graphcore-0.7.0/optimum/graphcore/data/data_collator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from functools import wraps
-from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from torch import Tensor
-
 from transformers.data import DataCollatorForLanguageModeling
 from transformers.data.data_collator import DataCollator
 from transformers.tokenization_utils_base import BatchEncoding
 
 
 def pad_on_batch_axis(batch_size: int) -> Callable[[DataCollator], DataCollator]:
     """
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py` & `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/ipu_configs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,32 @@
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from typing import Any, Dict
+
 from optimum.utils import logging
 
 from ....training_args import ALLOWED_N_IPU
 
 
 logger = logging.get_logger(__name__)
 
 
+# Deprecated.
 INFERENCE_ENGINES_TO_MODEL_NAMES = {
     "stable-diffusion-v1": "CompVis/stable-diffusion-v1-4",  # this is a guess
     "stable-diffusion-v1-5": "runwayml/stable-diffusion-v1-5",
     "stable-diffusion-512-v2-0": "stabilityai/stable-diffusion-2-base",
     "stable-diffusion-768-v2-0": "stabilityai/stable-diffusion-2",
     "stable-diffusion-512-v2-1": "stabilityai/stable-diffusion-2-1-base",
     "stable-diffusion-768-v2-1": "stabilityai/stable-diffusion-2-1",
@@ -59,51 +76,57 @@
         "attn_matrix_target_mem_mb": 45,
     },
     "vae": None,  # not supported yet
     "safety_checker": {"ipus_per_replica": 1, "matmul_proportion": 0.6},
 }
 
 
+# Deprecated.
 INFERENCE_ENGINES_TO_IPU_CONFIGS = {
     "stable-diffusion-v1": STABLE_DIFFUSION_V1_512_IPU_CONFIG,  # this is a guess
     "stable-diffusion-v1-5": STABLE_DIFFUSION_V1_512_IPU_CONFIG,
     "stable-diffusion-512-v2-0": STABLE_DIFFUSION_V2_512_IPU_CONFIG,
     "stable-diffusion-768-v2-0": STABLE_DIFFUSION_V2_768_IPU_CONFIG,
     "stable-diffusion-512-v2-1": STABLE_DIFFUSION_V2_512_IPU_CONFIG,
     "stable-diffusion-768-v2-1": STABLE_DIFFUSION_V2_768_IPU_CONFIG,
     "stable-inpainting-v1-0": STABLE_DIFFUSION_V1_512_IPU_CONFIG,
     "stable-inpainting-512-v2-0": STABLE_DIFFUSION_V2_512_IPU_CONFIG,
 }
 
 
 def get_default_ipu_configs(
-    engine: str = "stable-diffusion-512-v2-0",
-    height: int = 512,
-    width: int = 512,
+    unet_config: Dict[str, Any],
+    n_ipu: int = 4,
     num_prompts: int = 1,
     num_images_per_prompt: int = 1,
-    n_ipu: int = 4,
     **common_kwargs,
 ):
-    if engine not in INFERENCE_ENGINES_TO_MODEL_NAMES:
-        raise ValueError(f"{engine} should be one of {', '.join(INFERENCE_ENGINES_TO_MODEL_NAMES)}")
     if n_ipu not in ALLOWED_N_IPU:
         raise ValueError(
             f"{n_ipu=} is not a valid value for a Pod type, supported Pod types: {', '.join(ALLOWED_N_IPU)}"
         )
 
-    default_image_dim = 768 if "768" in engine else 512
-    if default_image_dim == 768 and height < default_image_dim and width < default_image_dim:
+    # Infer base checkpoint model size for instantiating default IPU configs.
+    cross_attention_dim = unet_config.cross_attention_dim
+    sample_size = unet_config.sample_size
+    model_ipu_configs = None
+    if cross_attention_dim == 768:
+        model_ipu_configs = STABLE_DIFFUSION_V1_512_IPU_CONFIG
+    elif cross_attention_dim == 1024:
+        if sample_size == 64:
+            model_ipu_configs = STABLE_DIFFUSION_V2_512_IPU_CONFIG
+        elif sample_size == 96:
+            model_ipu_configs = STABLE_DIFFUSION_V2_768_IPU_CONFIG
+    if model_ipu_configs is None:
         logger.warn(
-            "Generating an image smaller than 768x768 with a checkpoint fine-tuned for 768x768 "
-            "can lead to images of poor quality."
+            f"UNet config has a combination of `{cross_attention_dim=}` and `{sample_size=}` which we do not "
+            "have known configs for (SD1 = (768, 64), SD2 512x512 = (1024, 64), SD2 768 x 768 = (1024, 96). "
+            "Defaulting to the SD1 config."
         )
 
-    model_ipu_configs = INFERENCE_ENGINES_TO_IPU_CONFIGS[engine]
-
     unet_ipu_config = model_ipu_configs["unet"]
     text_encoder_ipu_config = model_ipu_configs["text_encoder"] if n_ipu > 4 else None
     vae_ipu_config = model_ipu_configs["vae"] if n_ipu > 4 else None
     safety_checker_ipu_config = model_ipu_configs["safety_checker"] if n_ipu > 4 else None
 
     # Set the micro batch size at 1 for now.
     common_kwargs["inference_device_iterations"] = num_prompts * num_images_per_prompt
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py` & `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 from typing import Optional, Tuple, Union
 
-import torch
-
 import poptorch
+import torch
 from diffusers import AutoencoderKL, StableDiffusionPipeline, UNet2DConditionModel
 from diffusers.models.autoencoder_kl import AutoencoderKLOutput
 from diffusers.models.cross_attention import CrossAttention
 from diffusers.models.unet_2d_condition import UNet2DConditionOutput
 from diffusers.models.vae import DecoderOutput, DiagonalGaussianDistribution
-from optimum.utils import logging
 from transformers import CLIPTextModel
 from transformers.modeling_outputs import BaseModelOutputWithPooling
 from transformers.models.clip.modeling_clip import CLIPTextTransformer
 
+from optimum.utils import logging
+
 from ....ipu_configuration import IPUConfig
 from ....modeling_utils import PipelineMixin
+from .ipu_configs import get_default_ipu_configs
 from .safety_checker import IPUStableDiffusionSafetyChecker
 
 
 logger = logging.get_logger(__name__)
 
 
 class IPUSlicedAttnProcessor:
@@ -59,15 +60,14 @@
 
     def __call__(self, attn: CrossAttention, hidden_states, encoder_hidden_states=None, attention_mask=None):
         batch_size, sequence_length, _ = hidden_states.shape
 
         attention_mask = attn.prepare_attention_mask(attention_mask, sequence_length)
 
         query = attn.to_q(hidden_states)
-        dim = query.shape[-1]
         query = attn.head_to_batch_dim(query)
 
         encoder_hidden_states = encoder_hidden_states if encoder_hidden_states is not None else hidden_states
         key = attn.to_k(encoder_hidden_states)
         value = attn.to_v(encoder_hidden_states)
         key = attn.head_to_batch_dim(key)
         value = attn.head_to_batch_dim(value)
@@ -107,15 +107,15 @@
         return hidden_states
 
 
 class IPUCLIPTextModel(CLIPTextModel, PipelineMixin):
     def parallelize(self):
         super().parallelize()
 
-        def _build_causal_attention_mask(self, bsz, seq_len, dtype):
+        def _build_causal_attention_mask(self, bsz, seq_len, dtype, device=None):
             # lazily create causal attention mask, with full attention between the vision tokens
             # pytorch uses additive attention mask; fill with -inf
             # IPU MOD
             # mask = torch.empty(bsz, seq_len, seq_len, dtype=dtype)
             # mask.fill_(torch.tensor(torch.finfo(dtype).min))
             mask = torch.ones((bsz, seq_len, seq_len), dtype=dtype) * torch.finfo(dtype).min
             mask.triu_(1)  # zero out the lower diagonal
@@ -257,29 +257,59 @@
         text_encoder,
         tokenizer,
         unet,
         scheduler,
         safety_checker,
         feature_extractor,
         requires_safety_checker=True,
+        n_ipu=4,
+        num_prompts=1,
+        num_images_per_prompt=1,
         unet_ipu_config=None,
         text_encoder_ipu_config=None,
         vae_ipu_config=None,
         safety_checker_ipu_config=None,
+        common_ipu_config_kwargs=None,
     ):
-        common_ipu_config = {
+        default_common_ipu_config_kwargs = {
             "enable_half_partials": True,
             "executable_cache_dir": "./exe_cache",
             "inference_device_iterations": 1,
             "inference_replication_factor": 1,
         }
 
+        if common_ipu_config_kwargs is not None:
+            if not isinstance(common_ipu_config_kwargs, dict):
+                raise TypeError(
+                    f"`common_ipu_config_kwargs` must be a dict, received {type(common_ipu_config_kwargs)}."
+                )
+            common_ipu_config_kwargs = {**default_common_ipu_config_kwargs, **common_ipu_config_kwargs}
+        else:
+            common_ipu_config_kwargs = default_common_ipu_config_kwargs
+
+        (
+            default_unet_ipu_config,
+            default_text_encoder_ipu_config,
+            default_vae_ipu_config,
+            default_safety_checker_ipu_config,
+        ) = get_default_ipu_configs(
+            unet.config,
+            n_ipu=n_ipu,
+            num_prompts=num_prompts,
+            num_images_per_prompt=num_images_per_prompt,
+            **common_ipu_config_kwargs,
+        )
+        unet_ipu_config = unet_ipu_config or default_unet_ipu_config
+        if n_ipu > 4:
+            text_encoder_ipu_config = text_encoder_ipu_config or default_text_encoder_ipu_config
+            vae_ipu_config = vae_ipu_config or default_vae_ipu_config
+            safety_checker_ipu_config = safety_checker_ipu_config or default_safety_checker_ipu_config
+
         def _get_poplar_executor(model, ipu_model_class, ipu_config):
-            model_ipu_config = {**common_ipu_config, **ipu_config}
-            model_ipu_config = IPUConfig.from_dict(model_ipu_config)
+            model_ipu_config = IPUConfig.from_dict(ipu_config)
 
             model_ipu = copy.deepcopy(model).half()
             model_ipu.__class__ = ipu_model_class
             model_ipu.ipu_config = model_ipu_config
             model_ipu.parallelize()
             override_module_eps(model_ipu)
 
@@ -358,17 +388,16 @@
         else:
             logger.info("Running safety_checker on CPU.")
             safety_checker = maybe_cast_module_to_float(safety_checker)
 
         if unet_ipu_config is not None:
             logger.info("Running UNet on IPU.")
 
-            attn_matrix_target_mem_mb = unet_ipu_config["attn_matrix_target_mem_mb"]
+            attn_matrix_target_mem_mb = unet_ipu_config.pop("attn_matrix_target_mem_mb")
 
-            unet_ipu_config = {**common_ipu_config, **unet_ipu_config}
             unet_ipu_config = IPUConfig.from_dict(unet_ipu_config)
 
             unet_ipu = copy.deepcopy(unet)
             unet_ipu.__class__ = IPUUNet2DConditionModel
             unet_ipu.ipu_config = unet_ipu_config
             unet_ipu.parallelize(attn_matrix_target_mem_mb=attn_matrix_target_mem_mb)
             override_module_eps(unet_ipu)
@@ -393,26 +422,34 @@
             requires_safety_checker=requires_safety_checker,
         )
 
     @classmethod
     def from_pretrained(
         cls,
         pretrained_model_name_or_path,
+        n_ipu=4,
+        num_prompts=1,
+        num_images_per_prompt=1,
         unet_ipu_config=None,
         text_encoder_ipu_config=None,
         vae_ipu_config=None,
         safety_checker_ipu_config=None,
+        common_ipu_config_kwargs=None,
         **kwargs,
     ):
         return super().from_pretrained(
             pretrained_model_name_or_path,
+            n_ipu=n_ipu,
+            num_prompts=num_prompts,
+            num_images_per_prompt=num_images_per_prompt,
             unet_ipu_config=unet_ipu_config,
             text_encoder_ipu_config=text_encoder_ipu_config,
             vae_ipu_config=vae_ipu_config,
             safety_checker_ipu_config=safety_checker_ipu_config,
+            common_ipu_config_kwargs=common_ipu_config_kwargs,
             **kwargs,
         )
 
     def set_attention_slice(self, slice_size: Optional[int]):
         # Another side effect of letting this go through is that CrossAttention could set
         # a different processor than what we intended, so do the simple thing for now.
         logger.warn(
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/generation/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/generation/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .attention_mixin import IPUAttentionMixin
-from .utils import IPUGenerationMixin, supports_kv_cache
+from .utils import IPUGenerationMixin, assert_poptorch_supports_cond, supports_kv_cache
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/generation/on_device_generation.py` & `optimum-graphcore-0.7.0/optimum/graphcore/generation/on_device_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from typing import Optional, Union
 
-import torch
-
 import poptorch
-from optimum.utils import logging
+import torch
 from transformers.generation.utils import LogitsProcessorList
 from transformers.modeling_outputs import ModelOutput
 
+from optimum.utils import logging
+
 
 logger = logging.get_logger(__name__)
 
 
 LARGE_NEGATIVE_CONST = -1e9
 
 
@@ -211,109 +211,110 @@
 
         # Since we are constrained to keeping buffers in float, including ones holding tokens which are ints,
         # we do most of the processing as int and cast just before writing.
         sequences = self.sequences.int()
         running_sequences = input_ids_mask * padded_input_ids + (1 - input_ids_mask) * self.running_sequences.int()
         is_finished = self.is_finished.int()
 
+        # 0. Check for termination of previous step
+        not_max_length_yet = absolute_step < self.max_length
+
+        worst_finished_score = torch.where(
+            torch.any(is_finished, axis=1),
+            torch.amin(self.log_probs, axis=1),
+            torch.ones(self.batch_size) * LARGE_NEGATIVE_CONST,
+        )
+        if self.early_stopping == "never" and self.length_penalty > 0.0:
+            best_running_score = self.running_log_probs[:, 0] / (self.max_length**self.length_penalty)
+        else:
+            best_running_score = self.running_log_probs[:, 0] / (absolute_step**self.length_penalty)
+        improvement_still_possible = torch.any(best_running_score > worst_finished_score)
+
+        still_open_beam = ~(torch.all(is_finished) & (self.early_stopping is True))
+
+        continue_search = not_max_length_yet & still_open_beam & improvement_still_possible
+
+        # 1. Return best beam for each batch and beam indices from previous step
+        # Account for the edge-case where there are no finished sequences for a
+        # particular batch item. If so, return running sequences for that batch item.
+        none_finished = torch.any(is_finished, axis=1)
+        return_sequences = torch.where(none_finished[:, None, None], sequences, running_sequences)
+        return_sequences = return_sequences[:, 0]
+
+        # 2. Get logits
         model_input_ids = torch.index_select(running_sequences, 2, absolute_step - 1)
         model_input_ids = self._flatten_beam_dim(model_input_ids, self.num_beams)
 
         logits = self.model(decoder_input_ids=model_input_ids, **kwargs)
         if hasattr(logits, "logits"):
             logits = logits.logits
         logits = logits.squeeze(1).float()
 
-        # 2. Compute log probs
+        # 3. Compute log probs
         vocab_size = logits.shape[-1]
         log_probs = torch.nn.functional.log_softmax(logits, dim=-1)
         log_probs = self.logits_processor(running_sequences, log_probs, absolute_step=absolute_step)
         log_probs = self._unflatten_beam_dim(log_probs, self.num_beams)
         log_probs = log_probs + self.running_log_probs.unsqueeze(-1)
         log_probs = log_probs.view(self.batch_size, self.num_beams * vocab_size)
 
-        # 3. Retrieve top-2*K
+        # 4. Retrieve top-2*K
         beams_to_keep = 2 * self.num_beams
         topk_log_probs, topk_indices = torch.topk(log_probs, k=beams_to_keep)
         topk_beam_indices = torch.div(topk_indices, vocab_size).int()
         topk_running_sequences = self._gather_beams(
             running_sequences, topk_beam_indices, self.batch_size, self.num_beams, beams_to_keep
         )
         topk_ids = topk_indices % vocab_size
-        topk_ids = topk_ids.unsqueeze(-1).int()
-
-        topk_sequences = poptorch.dynamic_update(topk_running_sequences, topk_ids, 2, absolute_step, 1)
+        topk_sequences = poptorch.dynamic_update(
+            topk_running_sequences, topk_ids.unsqueeze(-1).int(), 2, absolute_step, 1
+        )
 
-        # 4. Check which sequences have ended
-        did_topk_just_finish = torch.index_select(topk_sequences, 2, absolute_step).squeeze(2) == self.eos_token_id
+        # 5. Check which sequences have ended
+        did_topk_just_finish = topk_ids == self.eos_token_id
         running_topk_log_probs = topk_log_probs + did_topk_just_finish * LARGE_NEGATIVE_CONST
 
-        # 5. Get running sequences scores for next
+        # 6. Get running sequences scores for next
         next_topk_indices = torch.topk(running_topk_log_probs, k=self.num_beams)[1]
 
         next_running_sequences = self._gather_beams(
             topk_sequences, next_topk_indices, self.batch_size, beams_to_keep, self.num_beams
         )
         next_running_log_probs = self._gather_beams(
             running_topk_log_probs, next_topk_indices, self.batch_size, beams_to_keep, self.num_beams
         )
 
-        # 6. Process topk logits
+        # 7. Process topk logits
         topk_log_probs = topk_log_probs / (absolute_step**self.length_penalty)
-        beams_in_batch_are_full = self.is_finished.all(axis=-1, keepdims=True).repeat(
-            1, did_topk_just_finish.shape[-1]
-        ) & (self.early_stopping is True)
+        beams_in_batch_are_full = is_finished.all(axis=-1, keepdims=True).repeat(1, did_topk_just_finish.shape[-1]) & (
+            self.early_stopping is True
+        )
         add_penalty = ~did_topk_just_finish | beams_in_batch_are_full
         topk_log_probs += add_penalty * LARGE_NEGATIVE_CONST
 
-        # 7. Get scores, sequences, is sentence finished for next.
+        # 8. Get scores, sequences, is sentence finished for next.
         merged_sequences = torch.cat([sequences, topk_sequences], axis=1)
         merged_log_probs = torch.cat([self.log_probs, topk_log_probs], axis=1)
         merged_is_finished = torch.cat([is_finished, did_topk_just_finish], axis=1)
         topk_merged_indices = torch.topk(merged_log_probs, k=self.num_beams)[1]
         next_sequences = self._gather_beams(
             merged_sequences, topk_merged_indices, self.batch_size, 3 * self.num_beams, self.num_beams
         )
         next_log_probs = self._gather_beams(
             merged_log_probs, topk_merged_indices, self.batch_size, 3 * self.num_beams, self.num_beams
         )
         next_is_finished = self._gather_beams(
             merged_is_finished, topk_merged_indices, self.batch_size, 3 * self.num_beams, self.num_beams
         )
 
-        # 8. Determine the top k beam indices from the original set of all beams.
+        # 9. Determine the top k beam indices from the original set of all beams.
         next_running_indices = self._gather_beams(
             topk_beam_indices, next_topk_indices, self.batch_size, 2 * self.num_beams, self.num_beams
         )
 
-        # 9. Check for termination.
-        not_max_length_yet = absolute_step < self.max_length
-
-        worst_finished_score = torch.where(
-            torch.any(next_is_finished, axis=1),
-            torch.amin(self.log_probs, axis=1),
-            torch.ones(self.batch_size) * LARGE_NEGATIVE_CONST,
-        )
-        if self.early_stopping == "never" and self.length_penalty > 0.0:
-            best_running_score = self.running_log_probs[:, 0] / (self.max_length**self.length_penalty)
-        else:
-            best_running_score = self.running_log_probs[:, 0] / (absolute_step**self.length_penalty)
-        improvement_still_possible = torch.any(best_running_score > worst_finished_score)
-
-        still_open_beam = ~(torch.all(next_is_finished) & (self.early_stopping is True))
-
-        continue_search = not_max_length_yet & still_open_beam & improvement_still_possible
-
-        # 10. Return best beam for each batch and beam indices.
-        # Account for the edge-case where there are no finished sequences for a
-        # particular batch item. If so, return running sequences for that batch item.
-        none_finished = torch.any(next_is_finished, axis=1)
-        sequences = torch.where(none_finished[:, None, None], next_sequences, next_running_sequences)
-        return_sequences = sequences[:, 0]
-
         flat_batch_indices = torch.arange(self.batch_size * self.num_beams) // self.num_beams
         flat_batch_indices = flat_batch_indices * self.num_beams
         beam_indices = self._flatten_beam_dim(next_running_indices, self.num_beams)
         beam_indices = beam_indices + flat_batch_indices
 
         self.sequences.copy_(next_sequences.float())
         self.running_sequences.copy_(next_running_sequences.float())
@@ -364,14 +365,19 @@
         early_stopping: Optional[bool] = False,
     ):
         super().__init__()
 
         if not use_cache:
             raise NotImplementedError("On device generation assumes `use_cache=True`.")
 
+        if isinstance(eos_token_id, list):
+            if len(eos_token_id) > 1:
+                raise ValueError("Multiple EOS tokens are not yet supported for on-device generation.")
+            eos_token_id = eos_token_id[0]
+
         self.max_length = max_length
         self.context_length = 1
 
         if num_beams == 1:
             self.generation_strategy = OnDeviceGreedySearch(
                 model,
                 batch_size=batch_size,
@@ -404,15 +410,15 @@
         input_ids_key = "decoder_input_ids"
         input_ids = kwargs.pop(input_ids_key, None)
         if input_ids is None:
             input_ids_key = "input_ids"
             input_ids = kwargs.pop(input_ids_key, None)
             if input_ids is None:
                 raise ValueError(
-                    f"The on device generation model was called with kwargs that are missing both `decoder_input_ids` "
+                    "The on device generation model was called with kwargs that are missing both `decoder_input_ids` "
                     "and `input_ids`. Please provide one of these as inputs (default is `decoder_input_ids`)."
                 )
         if input_ids.shape[-1] > 1:
             raise ValueError("Context length (input_ids.shape[-1]) > 1 is not supported yet.")
 
         if generation_step := kwargs.pop("generation_step", None) is not None:
             self._generation_step.copy_(generation_step)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/generation/utils.py` & `optimum-graphcore-0.7.0/optimum/graphcore/generation/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #  Copyright 2022 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,21 +14,19 @@
 #  limitations under the License.
 
 import contextlib
 import copy
 import json
 import os
 import warnings
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+import poptorch
 import torch
 from torch import nn
-
-import poptorch
-from optimum.utils import logging
 from transformers.generation.stopping_criteria import validate_stopping_criteria
 from transformers.generation.utils import (
     BeamSampleDecoderOnlyOutput,
     BeamSampleEncoderDecoderOutput,
     BeamSampleOutput,
     BeamScorer,
     BeamSearchDecoderOnlyOutput,
@@ -40,36 +39,45 @@
     LogitsProcessorList,
     SampleDecoderOnlyOutput,
     SampleEncoderDecoderOutput,
     SampleOutput,
     StoppingCriteriaList,
 )
 from transformers.modeling_outputs import BaseModelOutput, ModelOutput
-from transformers.pytorch_utils import torch_int_div
 from transformers.utils.versions import require_version
 
+from optimum.utils import logging
+
 from .logits_process import IPULogitsProcessors
 from .on_device_generation import (
-    OnDeviceBeamSearch,
     OnDeviceGenerationModel,
     OnDeviceGenerationModelOutput,
-    OnDeviceGreedySearch,
 )
 
 
 logger = logging.get_logger(__name__)
 
 MODELS_SUPPORTING_KV_CACHE = set()
 
 
 def supports_kv_cache(pipelined_cls):
     MODELS_SUPPORTING_KV_CACHE.add(pipelined_cls)
     return pipelined_cls
 
 
+def assert_poptorch_supports_cond(context: Optional[str] = None):
+    context = context or ""
+    require_version("poptorch>=3.3", "Require poptorch>=3.3 for `poptorch.cond`. " + context)
+    if not hasattr(poptorch, "cond"):
+        raise AttributeError(
+            "`poptorch.cond` appears to be missing, perhaps you are using a candidate release "
+            "which does not support it yet? " + context
+        )
+
+
 @contextlib.contextmanager
 def graph_profile_dir_append(append: str):
     if poplar_engine_options_original := os.getenv("POPLAR_ENGINE_OPTIONS"):
         poplar_engine_options_modified = json.loads(poplar_engine_options_original)
         if autoreport_directory := poplar_engine_options_modified.get("autoReport.directory"):
             poplar_engine_options_modified["autoReport.directory"] = autoreport_directory + append
             os.environ["POPLAR_ENGINE_OPTIONS"] = json.dumps(poplar_engine_options_modified)
@@ -174,24 +182,32 @@
 class IPUGenerationMixin(GenerationMixin):
 
     """
     Enable optimization for encoder-decoder text generation where the encoder outputs
     are cached on the Decoder device using buffers.
     """
 
-    use_encoder_output_buffer = False
+    _use_cond_encoder = False
+    _use_encoder_output_buffer = False
+    kv_cache_enabled = False
 
     @property
     def encoder_output_buffer_enabled(self) -> bool:
-        return self.config.is_encoder_decoder and self.use_encoder_output_buffer
+        return self.config.is_encoder_decoder and self._use_encoder_output_buffer and not self._use_cond_encoder
+
+    @property
+    def cond_encoder_enabled(self) -> bool:
+        return self.config.is_encoder_decoder and self._use_cond_encoder
 
     def _pad_tensors_to_max_len(self, tensor: torch.Tensor, max_length: int, pad_token_id: int) -> torch.Tensor:
         return nn.functional.pad(tensor, (0, max_length - tensor.shape[1]), "constant", pad_token_id)
 
     def _ensure_generation_step_progression(self, generation_step):
+        if not self.kv_cache_enabled:
+            return
         if not hasattr(self, "_previous_generation_step"):
             self._previous_generation_step = generation_step
             return
         if generation_step <= self._previous_generation_step and generation_step != 0:
             raise ValueError("`generation_step` must increase, or begin from 0.")
         self._previous_generation_step = generation_step
 
@@ -216,41 +232,47 @@
                 decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
                 decoder_options = decoder_ipu_config.to_options(for_inference=True)
 
                 if self.encoder_output_buffer_enabled:
                     require_version(
                         "poptorch>=3.3", "Updatable encoder output buffer optimization only available in poptorch>=3.3"
                     )
-                    named_buffers = {"encoder_last_hidden_state": kwargs["encoder_outputs"]["last_hidden_state"]}
-                    if kwargs.get("attention_mask") is not None:
-                        named_buffers["encoder_attention_mask"] = kwargs["attention_mask"].half()
+                    if decoder_ipu_config.inference_replication_factor > 1:
+                        raise ValueError("Replication is not supported when `use_encoder_output_buffer=True`.")
+
+                    named_buffers = {}
+                    encoder_last_hidden_state = kwargs.pop("encoder_outputs")["last_hidden_state"]
+                    if encoder_last_hidden_state is not None:
+                        named_buffers["encoder_last_hidden_state"] = encoder_last_hidden_state
+                    attention_mask = kwargs.pop("attention_mask", None)
+                    if attention_mask is not None:
+                        named_buffers["encoder_attention_mask"] = attention_mask.half()
+                    if not named_buffers:
+                        raise ValueError(
+                            "Found `encoder_output_buffer_enabled=True`, but encoder outputs missing when calling the model."
+                        )
                     decoder_wrapper.register_encoder_output_buffers(named_buffers)
                     decoder_options.updatableNamedBuffers(list(named_buffers.keys()))
+                if self.cond_encoder_enabled and decoder_ipu_config.inference_replication_factor > 1:
+                    decoder_options.broadcastBuffers(False)
 
                 self.poptorch_decoder = poptorch.inferenceModel(decoder_wrapper, decoder_options)
-
-        if self.encoder_output_buffer_enabled:
-            kwargs.pop("encoder_outputs", None)
-            kwargs.pop("attention_mask", None)
+        elif self.encoder_output_buffer_enabled:
+            encoder_last_hidden_state = kwargs.pop("encoder_outputs")["last_hidden_state"]
+            attention_mask = kwargs.pop("attention_mask", None)
+            if generation_step == 0:
+                self.poptorch_decoder.encoder_last_hidden_state.copy_(encoder_last_hidden_state)
+                if attention_mask is not None:
+                    self.poptorch_decoder.encoder_attention_mask.copy_(attention_mask.half())
+                self.poptorch_decoder.copyNamedBuffersToDevice()
 
         # This will trigger a compile first time it's ran
         with graph_profile_dir_append("/decoder" if self.config.is_encoder_decoder else ""):
             return self.poptorch_decoder(*args, t=t, **kwargs)
 
-    def _update_model_buffers_if_needed(self, model_kwargs):
-        """
-        If decoder model then we cache the encoder values inside pytorch buffers to reduce the IO cost
-        """
-        if not (self.encoder_output_buffer_enabled and hasattr(self, "poptorch_decoder")):
-            return
-        self.poptorch_decoder.encoder_last_hidden_state.copy_(model_kwargs["encoder_outputs"]["last_hidden_state"])
-        if model_kwargs.get("attention_mask") is not None:
-            self.poptorch_decoder.encoder_attention_mask.copy_(model_kwargs["attention_mask"].half())
-        self.poptorch_decoder.copyNamedBuffersToDevice()
-
     def _prepare_encoder_decoder_kwargs_for_generation(
         self, inputs_tensor: torch.Tensor, model_kwargs, model_input_name: Optional[str] = None
     ) -> Dict[str, Any]:
         # 1. get encoder
         encoder = self.get_encoder()
 
         # 2. prepare encoder args and encoder kwargs from model kwargs
@@ -262,61 +284,146 @@
         }
 
         # 3. make sure that encoder returns `ModelOutput`
         model_input_name = model_input_name if model_input_name is not None else self.main_input_name
         encoder_kwargs["return_dict"] = True
         encoder_kwargs[model_input_name] = inputs_tensor
 
+        if self.cond_encoder_enabled:
+            # The encoder and decoder are being run on the same IPU.
+            # We make a simplifying assumption and only provide the inputs to the encoder.
+            model_kwargs[model_input_name] = inputs_tensor
+            # For minimal changes to the generation path, we put dummy encoder outputs here
+            # and drop them before calling the model.
+            model_kwargs["encoder_outputs"] = BaseModelOutput(
+                last_hidden_state=torch.zeros(inputs_tensor.shape[0], 1, dtype=encoder.dtype)
+            )
+            return model_kwargs
+
         if not hasattr(self, "poptorch_encoder"):
             # Use split encoder ipu_config for encoder/decoder models
             if os.getenv("DEBUG_RUN_ENCODER_ON_CPU", False):
                 self.poptorch_encoder = encoder.eval()
             else:
                 self.poptorch_encoder = poptorch.inferenceModel(
                     encoder.eval(), self.encoder_ipu_config.to_options(for_inference=True)
                 )
         with graph_profile_dir_append("/encoder"):
             model_kwargs["encoder_outputs"]: ModelOutput = self.poptorch_encoder(**encoder_kwargs)
 
         return model_kwargs
 
+    @staticmethod
+    def _expand_inputs_for_generation(
+        expand_size: int = 1,
+        is_encoder_decoder: bool = False,
+        input_ids: Optional[torch.LongTensor] = None,
+        **model_kwargs,
+    ) -> Tuple[torch.LongTensor, Dict[str, Any]]:
+        # Change: if we are running the encoder and decoder on the same IPU, `model_kwargs`
+        # will contain `input_features`. We do not want these to be expanded by e.g. num_beams.
+        input_features = model_kwargs.pop("input_features", None)
+        input_ids, model_kwargs = GenerationMixin._expand_inputs_for_generation(
+            expand_size=expand_size, is_encoder_decoder=is_encoder_decoder, input_ids=input_ids, **model_kwargs
+        )
+        if input_features is not None:
+            model_kwargs["input_features"] = input_features
+        return input_ids, model_kwargs
+
     def detachFromDevice(self):
         if hasattr(self, "poptorch_encoder"):
             self.poptorch_encoder.detachFromDevice()
         if hasattr(self, "poptorch_decoder"):
             self.poptorch_decoder.detachFromDevice()
 
+    def destroy(self):
+        if hasattr(self, "poptorch_encoder"):
+            self.poptorch_encoder.destroy()
+            delattr(self, "poptorch_encoder")
+        if hasattr(self, "poptorch_decoder"):
+            self.poptorch_decoder.destroy()
+            delattr(self, "poptorch_decoder")
+
     def _get_generation_step_tensor(self, generation_step, ascending=False):
         # Returns a 1 dimensional tensor of the form [device_iterations * replication factor]
         # with all elements equal to generation_step.
         # This ensures the dimensions are as expected by any parallelism options.
         decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
         per_replica = (
             torch.arange(decoder_ipu_config.inference_device_iterations) + generation_step
             if ascending
             else torch.ones(decoder_ipu_config.inference_device_iterations) * generation_step
         )
-        return per_replica.repeat(decoder_ipu_config.inference_replication_factor)
+        return per_replica.repeat_interleave(decoder_ipu_config.inference_replication_factor)
 
-    def _maybe_ensure_kv_cache_supported(self, use_cache):
-        if not use_cache or hasattr(self, "_poptorch_decoder"):
-            return
+    def _populate_parallelize_kwargs_with_generation_config(self, **kwargs):
+        if self.generation_config is None:
+            return kwargs
+
+        for kwarg in ["num_beams", "max_length"]:
+            if kwarg not in kwargs:
+                kwarg_value = getattr(self.generation_config, kwarg)
+                kwargs[kwarg] = kwarg_value
+                logger.info(f"Setting parallelize kwarg `{kwarg}` to value in generation_config ({kwarg_value}).")
+
+        return kwargs
+
+    def _validate_kv_cache(self, use_cache, num_beams=1, max_length=128):
+        first_call = not hasattr(self, "_poptorch_decoder")
 
         if use_cache and self.__class__ not in MODELS_SUPPORTING_KV_CACHE:
-            raise ValueError(
-                f"{self.__class__} does not support KV caching. Pipelined models can be "
-                "decorated using `supports_kv_cache` once they support static KV caching."
-            )
+            if first_call:
+                logger.warn(
+                    f"{self.__class__} does not support KV caching, but `use_cache=True`. "
+                    "Overriding to `use_cache=False`. If your believe your pipelined model "
+                    "supports static KV caching, please decorate it using `supports_kv_cache`."
+                )
+            use_cache = False
+
+        if not use_cache or not first_call:
+            return use_cache
 
         model_has_kv_cache_initialized = any(getattr(m, "kv_cache_initialized", False) for m in self.modules())
         if use_cache and not model_has_kv_cache_initialized:
             raise ValueError(
                 f"{self.__class__.__name__} supports KV caching and `use_cache=True`, but no KV caches have been initialized. "
                 f"Please pass `use_cache=True` to the `parallelize` method of {self.__class__.__name__}."
             )
+        self.kv_cache_enabled = use_cache and model_has_kv_cache_initialized
+
+        if not self.kv_cache_enabled:
+            return use_cache
+
+        module_with_cache = next(m for m in self.modules() if getattr(m, "kv_cache_initialized", False))
+        cache_shape = module_with_cache._k_cache.shape
+        cache_num_beams = module_with_cache._num_beams
+        cache_max_length = cache_shape[2]
+
+        generic_kwarg_msg = (
+            "KV caches are created with `kwargs` that are directly provided to `parallelize`, or where such "
+            "kwargs are missing, we optionally retrieve values from the `model.generation_config`. "
+            "On the other hand, `model.generate()` will determine generation kwargs in the priority of "
+            "`kwargs` > `kwargs['generation_config']` > `model.generation_config`. "
+            "Mismatches between the two flows can be reconciled by ensuring that the kwargs provided to `parallelize` "
+            "match the `kwargs` and / or `kwargs['generation_config']` passed to `model.generate()`."
+        )
+        if cache_num_beams != num_beams:
+            raise ValueError(
+                f"KV caches were created with num_beams={cache_num_beams}, but `model.generate()` is being called "
+                f"with {num_beams=}."
+                f"\n{generic_kwarg_msg}"
+            )
+        if cache_max_length != max_length:
+            raise ValueError(
+                f"KV caches were created with max_length={cache_max_length}, but `model.generate()` is being called "
+                f"with {max_length=}."
+                f"\n{generic_kwarg_msg}"
+            )
+
+        return use_cache
 
     def change_lm_head_to_indexed_input_linear(self, restore: bool):
         """Changes the LM head with the faster _IndexedInputLinear layer.
 
         Args:
             restore: whether to restore the LM head to the original version or not.
         """
@@ -331,15 +438,15 @@
     def greedy_search(
         self,
         input_ids: torch.LongTensor,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
-        eos_token_id: Optional[int] = None,
+        eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         **model_kwargs,
     ) -> Union[GreedySearchOutput, torch.LongTensor]:
         r"""
@@ -358,16 +465,16 @@
                 used to tell if the generation loop should stop.
 
             max_length (`int`, *optional*, defaults to 20):
                 **DEPRECATED**. Use `logits_processor` or `stopping_criteria` directly to cap the number of generated
                 tokens. The maximum length of the sequence to be generated.
             pad_token_id (`int`, *optional*):
                 The id of the *padding* token.
-            eos_token_id (`int`, *optional*):
-                The id of the *end-of-sequence* token.
+            eos_token_id (`Union[int, List[int]]`, *optional*):
+                The id of the *end-of-sequence* token. Optionally, use a list to set multiple *end-of-sequence* tokens.
             output_attentions (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the attentions tensors of all attention layers. See `attentions` under
                 returned tensors for more details.
             output_hidden_states (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
@@ -429,23 +536,30 @@
                 "`max_length` is deprecated in this function, use"
                 " `stopping_criteria=StoppingCriteriaList([MaxLengthCriteria(max_length=max_length)])` instead.",
                 UserWarning,
             )
             stopping_criteria = validate_stopping_criteria(stopping_criteria, max_length)
         else:
             max_length = stopping_criteria.max_length
-        pad_token_id = pad_token_id if pad_token_id is not None else self.config.pad_token_id
-        eos_token_id = eos_token_id if eos_token_id is not None else self.config.eos_token_id
-        output_scores = output_scores if output_scores is not None else self.config.output_scores
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        pad_token_id = pad_token_id if pad_token_id is not None else self.generation_config.pad_token_id
+        eos_token_id = eos_token_id if eos_token_id is not None else self.generation_config.eos_token_id
+        if isinstance(eos_token_id, int):
+            eos_token_id = [eos_token_id]
+        eos_token_id_tensor = torch.tensor(eos_token_id).to(input_ids.device) if eos_token_id is not None else None
+        output_scores = output_scores if output_scores is not None else self.generation_config.output_scores
+        output_attentions = (
+            output_attentions if output_attentions is not None else self.generation_config.output_attentions
+        )
         output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+            output_hidden_states if output_hidden_states is not None else self.generation_config.output_hidden_states
         )
         return_dict_in_generate = (
-            return_dict_in_generate if return_dict_in_generate is not None else self.config.return_dict_in_generate
+            return_dict_in_generate
+            if return_dict_in_generate is not None
+            else self.generation_config.return_dict_in_generate
         )
 
         # init attention / hidden states / scores tuples
         scores = () if (return_dict_in_generate and output_scores) else None
         decoder_attentions = () if (return_dict_in_generate and output_attentions) else None
         cross_attentions = () if (return_dict_in_generate and output_attentions) else None
         decoder_hidden_states = () if (return_dict_in_generate and output_hidden_states) else None
@@ -454,17 +568,15 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         use_cache = model_kwargs.get("use_cache", False)
-        self._maybe_ensure_kv_cache_supported(use_cache)
-
-        self._update_model_buffers_if_needed(model_kwargs)
+        use_cache = self._validate_kv_cache(use_cache, num_beams=1, max_length=max_length)
 
         # Change: intercept to optionally run the entire generation loop on device
         if self.on_device_generation_steps > 0:
             return self._on_device_greedy_search(
                 input_ids,
                 logits_processor=logits_processor,
                 stopping_criteria=stopping_criteria,
@@ -547,16 +659,18 @@
             input_ids = torch.cat([input_ids, next_tokens[:, None]], dim=-1)
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
             cur_len = cur_len + 1
 
             # if eos_token was found in one sentence, set sentence to finished
-            if eos_token_id is not None:
-                unfinished_sequences = unfinished_sequences.mul((next_tokens != eos_token_id).long())
+            if eos_token_id_tensor is not None:
+                unfinished_sequences = unfinished_sequences.mul(
+                    next_tokens.tile(eos_token_id_tensor.shape[0], 1).ne(eos_token_id_tensor.unsqueeze(1)).prod(dim=0)
+                )
 
             # stop when each sentence is finished, or if we exceed the maximum length
             if unfinished_sequences.max() == 0 or stopping_criteria(input_ids, scores):
                 # Change: remove synced_gpu code
                 break
         # End of while True
 
@@ -585,15 +699,15 @@
         self,
         input_ids: torch.LongTensor,
         beam_scorer: BeamScorer,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
-        eos_token_id: Optional[int] = None,
+        eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         **model_kwargs,
     ) -> Union[BeamSearchOutput, torch.LongTensor]:
         r"""
@@ -614,16 +728,16 @@
                 An instance of [`StoppingCriteriaList`]. List of instances of class derived from [`StoppingCriteria`]
                 used to tell if the generation loop should stop.
             max_length (`int`, *optional*, defaults to 20):
                 **DEPRECATED**. Use `logits_processor` or `stopping_criteria` directly to cap the number of generated
                 tokens. The maximum length of the sequence to be generated.
             pad_token_id (`int`, *optional*):
                 The id of the *padding* token.
-            eos_token_id (`int`, *optional*):
-                The id of the *end-of-sequence* token.
+            eos_token_id (`Union[int, List[int]]`, *optional*):
+                The id of the *end-of-sequence* token. Optionally, use a list to set multiple *end-of-sequence* tokens.
             output_attentions (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the attentions tensors of all attention layers. See `attentions` under
                 returned tensors for more details.
             output_hidden_states (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
@@ -703,23 +817,29 @@
                 UserWarning,
             )
             stopping_criteria = validate_stopping_criteria(stopping_criteria, max_length)
         else:
             max_length = stopping_criteria.max_length
         if len(stopping_criteria) == 0:
             warnings.warn("You don't have defined any stopping_criteria, this will likely loop forever", UserWarning)
-        pad_token_id = pad_token_id if pad_token_id is not None else self.config.pad_token_id
-        eos_token_id = eos_token_id if eos_token_id is not None else self.config.eos_token_id
-        output_scores = output_scores if output_scores is not None else self.config.output_scores
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        pad_token_id = pad_token_id if pad_token_id is not None else self.generation_config.pad_token_id
+        eos_token_id = eos_token_id if eos_token_id is not None else self.generation_config.eos_token_id
+        if isinstance(eos_token_id, int):
+            eos_token_id = [eos_token_id]
+        output_scores = output_scores if output_scores is not None else self.generation_config.output_scores
+        output_attentions = (
+            output_attentions if output_attentions is not None else self.generation_config.output_attentions
+        )
         output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+            output_hidden_states if output_hidden_states is not None else self.generation_config.output_hidden_states
         )
         return_dict_in_generate = (
-            return_dict_in_generate if return_dict_in_generate is not None else self.config.return_dict_in_generate
+            return_dict_in_generate
+            if return_dict_in_generate is not None
+            else self.generation_config.return_dict_in_generate
         )
 
         batch_size = len(beam_scorer._beam_hyps)
         num_beams = beam_scorer.num_beams
 
         batch_beam_size, cur_len = input_ids.shape
 
@@ -741,17 +861,15 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         use_cache = model_kwargs.get("use_cache", False)
-        self._maybe_ensure_kv_cache_supported(use_cache)
-
-        self._update_model_buffers_if_needed(model_kwargs)
+        use_cache = self._validate_kv_cache(use_cache, num_beams=num_beams, max_length=max_length)
 
         # Change: intercept to optionally run the entire generation loop on device
         if self.on_device_generation_steps > 0:
             return self._on_device_beam_search(
                 input_ids,
                 beam_scorer=beam_scorer,
                 logits_processor=logits_processor,
@@ -830,15 +948,15 @@
             vocab_size = next_token_scores.shape[-1]
             next_token_scores = next_token_scores.view(batch_size, num_beams * vocab_size)
 
             next_token_scores, next_tokens = torch.topk(
                 next_token_scores, 2 * num_beams, dim=1, largest=True, sorted=True
             )
 
-            next_indices = torch_int_div(next_tokens, vocab_size)
+            next_indices = torch.div(next_tokens, vocab_size, rounding_mode="floor")
             next_tokens = next_tokens % vocab_size
 
             # stateless
             beam_outputs = beam_scorer.process(
                 input_ids,
                 next_token_scores,
                 next_tokens,
@@ -853,16 +971,16 @@
             beam_idx = beam_outputs["next_beam_indices"]
 
             input_ids = torch.cat([input_ids[beam_idx, :], beam_next_tokens.unsqueeze(-1)], dim=-1)
 
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
-            if model_kwargs["past"] is not None:
-                model_kwargs["past"] = self._reorder_cache(model_kwargs["past"], beam_idx)
+            if model_kwargs["past_key_values"] is not None:
+                model_kwargs["past_key_values"] = self._reorder_cache(model_kwargs["past_key_values"], beam_idx)
             # Change: add beam_idx to model_kwargs so KV caching can be made aware of it on device
             model_kwargs["beam_idx"] = beam_idx
 
             if return_dict_in_generate and output_scores:
                 beam_indices = tuple((beam_indices[beam_idx[i]] + (beam_idx[i],) for i in range(len(beam_indices))))
 
             # increase cur_len
@@ -914,15 +1032,15 @@
         self,
         input_ids: torch.LongTensor,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         logits_warper: Optional[LogitsProcessorList] = None,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
-        eos_token_id: Optional[int] = None,
+        eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         **model_kwargs,
     ) -> Union[SampleOutput, torch.LongTensor]:
         r"""
@@ -944,16 +1062,16 @@
                 to warp the prediction score distribution of the language modeling head applied before multinomial
                 sampling at each generation step.
             max_length (`int`, *optional*, defaults to 20):
                 **DEPRECATED**. Use `logits_processor` or `stopping_criteria` directly to cap the number of generated
                 tokens. The maximum length of the sequence to be generated.
             pad_token_id (`int`, *optional*):
                 The id of the *padding* token.
-            eos_token_id (`int`, *optional*):
-                The id of the *end-of-sequence* token.
+            eos_token_id (`Union[int, List[int]]`, *optional*):
+                The id of the *end-of-sequence* token. Optionally, use a list to set multiple *end-of-sequence* tokens.
             output_attentions (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the attentions tensors of all attention layers. See `attentions` under
                 returned tensors for more details.
             output_hidden_states (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
@@ -1029,24 +1147,33 @@
         if max_length is not None:
             warnings.warn(
                 "`max_length` is deprecated in this function, use"
                 " `stopping_criteria=StoppingCriteriaList(MaxLengthCriteria(max_length=max_length))` instead.",
                 UserWarning,
             )
             stopping_criteria = validate_stopping_criteria(stopping_criteria, max_length)
+        else:
+            max_length = stopping_criteria.max_length
         logits_warper = logits_warper if logits_warper is not None else LogitsProcessorList()
-        pad_token_id = pad_token_id if pad_token_id is not None else self.config.pad_token_id
-        eos_token_id = eos_token_id if eos_token_id is not None else self.config.eos_token_id
-        output_scores = output_scores if output_scores is not None else self.config.output_scores
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        pad_token_id = pad_token_id if pad_token_id is not None else self.generation_config.pad_token_id
+        eos_token_id = eos_token_id if eos_token_id is not None else self.generation_config.eos_token_id
+        if isinstance(eos_token_id, int):
+            eos_token_id = [eos_token_id]
+        eos_token_id_tensor = torch.tensor(eos_token_id).to(input_ids.device) if eos_token_id is not None else None
+        output_scores = output_scores if output_scores is not None else self.generation_config.output_scores
+        output_attentions = (
+            output_attentions if output_attentions is not None else self.generation_config.output_attentions
+        )
         output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+            output_hidden_states if output_hidden_states is not None else self.generation_config.output_hidden_states
         )
         return_dict_in_generate = (
-            return_dict_in_generate if return_dict_in_generate is not None else self.config.return_dict_in_generate
+            return_dict_in_generate
+            if return_dict_in_generate is not None
+            else self.generation_config.return_dict_in_generate
         )
 
         # init attention / hidden states / scores tuples
         scores = () if (return_dict_in_generate and output_scores) else None
         decoder_attentions = () if (return_dict_in_generate and output_attentions) else None
         cross_attentions = () if (return_dict_in_generate and output_attentions) else None
         decoder_hidden_states = () if (return_dict_in_generate and output_hidden_states) else None
@@ -1055,17 +1182,15 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         use_cache = model_kwargs.get("use_cache", False)
-        self._maybe_ensure_kv_cache_supported(use_cache)
-
-        self._update_model_buffers_if_needed(model_kwargs)
+        use_cache = self._validate_kv_cache(use_cache, num_beams=1, max_length=max_length)
 
         # Change: intercept to optionally run the entire generation loop on device
         if self.on_device_generation_steps > 0:
             return self._on_device_sample()
 
         # keep track of which sequences are already finished
         unfinished_sequences = input_ids.new(input_ids.shape[0]).fill_(1)
@@ -1143,16 +1268,18 @@
             input_ids = torch.cat([input_ids, next_tokens[:, None]], dim=-1)
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
             cur_len = cur_len + 1
 
             # if eos_token was found in one sentence, set sentence to finished
-            if eos_token_id is not None:
-                unfinished_sequences = unfinished_sequences.mul((next_tokens != eos_token_id).long())
+            if eos_token_id_tensor is not None:
+                unfinished_sequences = unfinished_sequences.mul(
+                    next_tokens.tile(eos_token_id_tensor.shape[0], 1).ne(eos_token_id_tensor.unsqueeze(1)).prod(dim=0)
+                )
 
             # stop when each sentence is finished, or if we exceed the maximum length
             if unfinished_sequences.max() == 0 or stopping_criteria(input_ids, scores):
                 break
 
         if return_dict_in_generate:
             if self.config.is_encoder_decoder:
@@ -1180,15 +1307,15 @@
         input_ids: torch.LongTensor,
         beam_scorer: BeamScorer,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         logits_warper: Optional[LogitsProcessorList] = None,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
-        eos_token_id: Optional[int] = None,
+        eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         **model_kwargs,
     ) -> Union[BeamSampleOutput, torch.LongTensor]:
         r"""
@@ -1213,16 +1340,16 @@
                 to warp the prediction score distribution of the language modeling head applied before multinomial
                 sampling at each generation step.
             max_length (`int`, *optional*, defaults to 20):
                 **DEPRECATED**. Use `logits_processor` or `stopping_criteria` directly to cap the number of generated
                 tokens. The maximum length of the sequence to be generated.
             pad_token_id (`int`, *optional*):
                 The id of the *padding* token.
-            eos_token_id (`int`, *optional*):
-                The id of the *end-of-sequence* token.
+            eos_token_id (`Union[int, List[int]]`, *optional*):
+                The id of the *end-of-sequence* token. Optionally, use a list to set multiple *end-of-sequence* tokens.
             output_attentions (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the attentions tensors of all attention layers. See `attentions` under
                 returned tensors for more details.
             output_hidden_states (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
@@ -1306,23 +1433,29 @@
         if max_length is not None:
             warnings.warn(
                 "`max_length` is deprecated in this function, use"
                 " `stopping_criteria=StoppingCriteriaList(MaxLengthCriteria(max_length=max_length))` instead.",
                 UserWarning,
             )
             stopping_criteria = validate_stopping_criteria(stopping_criteria, max_length)
-        pad_token_id = pad_token_id if pad_token_id is not None else self.config.pad_token_id
-        eos_token_id = eos_token_id if eos_token_id is not None else self.config.eos_token_id
-        output_scores = output_scores if output_scores is not None else self.config.output_scores
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        else:
+            max_length = stopping_criteria.max_length
+        pad_token_id = pad_token_id if pad_token_id is not None else self.generation_config.pad_token_id
+        eos_token_id = eos_token_id if eos_token_id is not None else self.generation_config.eos_token_id
+        output_scores = output_scores if output_scores is not None else self.generation_config.output_scores
+        output_attentions = (
+            output_attentions if output_attentions is not None else self.generation_config.output_attentions
+        )
         output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+            output_hidden_states if output_hidden_states is not None else self.generation_config.output_hidden_states
         )
         return_dict_in_generate = (
-            return_dict_in_generate if return_dict_in_generate is not None else self.config.return_dict_in_generate
+            return_dict_in_generate
+            if return_dict_in_generate is not None
+            else self.generation_config.return_dict_in_generate
         )
 
         batch_size = len(beam_scorer._beam_hyps)
         num_beams = beam_scorer.num_beams
 
         batch_beam_size, cur_len = input_ids.shape
 
@@ -1339,17 +1472,15 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         use_cache = model_kwargs.get("use_cache", False)
-        self._maybe_ensure_kv_cache_supported(use_cache)
-
-        self._update_model_buffers_if_needed(model_kwargs)
+        use_cache = self._validate_kv_cache(use_cache, num_beams=num_beams, max_length=max_length)
 
         # Change: intercept to optionally run the entire generation loop on device
         if self.on_device_generation_steps > 0:
             return self._on_device_beam_sample()
 
         beam_scores = torch.zeros((batch_size, num_beams), dtype=torch.float, device=input_ids.device)
         beam_scores = beam_scores.view((batch_size * num_beams,))
@@ -1423,15 +1554,15 @@
 
             next_tokens = torch.multinomial(probs, num_samples=2 * num_beams)
             next_token_scores = torch.gather(next_token_scores, -1, next_tokens)
 
             next_token_scores, _indices = torch.sort(next_token_scores, descending=True, dim=1)
             next_tokens = torch.gather(next_tokens, -1, _indices)
 
-            next_indices = torch_int_div(next_tokens, vocab_size)
+            next_indices = torch.div(next_tokens, vocab_size, rounding_mode="floor")
             next_tokens = next_tokens % vocab_size
 
             # stateless
             beam_outputs = beam_scorer.process(
                 input_ids,
                 next_token_scores,
                 next_tokens,
@@ -1445,16 +1576,16 @@
             beam_idx = beam_outputs["next_beam_indices"]
 
             input_ids = torch.cat([input_ids[beam_idx, :], beam_next_tokens.unsqueeze(-1)], dim=-1)
 
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
-            if model_kwargs["past"] is not None:
-                model_kwargs["past"] = self._reorder_cache(model_kwargs["past"], beam_idx)
+            if model_kwargs["past_key_values"] is not None:
+                model_kwargs["past_key_values"] = self._reorder_cache(model_kwargs["past_key_values"], beam_idx)
             # Change: add beam_idx to model_kwargs so KV caching can be made aware of it on device
             model_kwargs["beam_idx"] = beam_idx
 
             if return_dict_in_generate and output_scores:
                 beam_indices = tuple((beam_indices[beam_idx[i]] + (beam_idx[i],) for i in range(len(beam_indices))))
 
             # increase cur_len
@@ -1553,15 +1684,17 @@
                 # These inputs will copied onto device via buffers, so we don't need to duplicate them.
                 adapted_model_inputs[k] = v
                 continue
             if k == "beam_idx":
                 # With on-device generation, beam_idx at each step is handled through buffers.
                 continue
 
-            if torch.is_tensor(v):
+            if k == "input_features" and self.cond_encoder_enabled:
+                v = v.repeat(on_device_generation_steps, *(1 for _ in range(v.ndim - 1)))
+            elif torch.is_tensor(v):
                 if v.shape[0] != batch_size:
                     raise ValueError(f"Unexpected size in dim 0 for {k}, expected {batch_size}.")
                 v = v.repeat(on_device_generation_steps, *(1 for _ in range(v.ndim - 1)))
             elif k == "encoder_outputs":
                 v_type = type(v)
                 if not isinstance(v, BaseModelOutput):
                     raise ValueError(
@@ -1608,17 +1741,19 @@
         if (max_length - context_length) % self.on_device_generation_steps != 0:
             logger.info(
                 "`max_length - context_length` does not evenly divide `on_device_generation_steps` "
                 f"({max_length - context_length} vs {self.on_device_generation_steps}). Generation will be done "
                 f"{self.on_device_generation_steps} tokens at a time and stop short of `max_length` so as not to exceed it."
             )
 
-        if self.ipu_config.inference_device_iterations != 1:
+        decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
+        if decoder_ipu_config.inference_device_iterations not in (1, self.on_device_generation_steps):
             raise ValueError(
-                "On device generation expects `inference_device_iterations=1`, "
+                "On device generation expects `inference_device_iterations=1` or "
+                "`inference_device_iterations=on_device_generation_steps`, "
                 f"received {self.ipu_config.inference_device_iterations}. "
                 "For on device generation, `inference_device_iterations` will be set to "
                 f"`on_device_generation_steps={self.on_device_generation_steps}`."
             )
         if hasattr(self, "decoder_ipu_config"):
             self.decoder_ipu_config.inference_device_iterations = self.on_device_generation_steps
         else:
@@ -1634,44 +1769,51 @@
         model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
         # A model-agnostic version of above mainly to duplicate inputs for device iterations.
         model_inputs = self._prepare_inputs_for_on_device_generation(
             model_inputs, self.on_device_generation_steps, batch_size
         )
 
-        on_device_generation_model_ctr = lambda inst: OnDeviceGenerationModel(
-            inst,
-            batch_size=batch_size,
-            max_length=max_length,
-            pad_token_id=pad_token_id,
-            eos_token_id=eos_token_id,
-            logits_processor=logits_processor,
-            num_beams=1,
-            use_cache=True,
-        )
+        per_replica_batch_size = batch_size // decoder_ipu_config.inference_replication_factor
+
+        def on_device_generation_model_ctr(inst):
+            return OnDeviceGenerationModel(
+                inst,
+                batch_size=per_replica_batch_size,
+                max_length=max_length,
+                pad_token_id=pad_token_id,
+                eos_token_id=eos_token_id,
+                logits_processor=logits_processor,
+                num_beams=1,
+                use_cache=True,
+            )
 
         generation_step = 0
         while True:
             output = self._call_generate(
                 generation_step=generation_step,  # NB: equal to `cur_len - 1` since context_length=1
                 on_device_generation_model_ctr=on_device_generation_model_ctr,
                 **model_inputs,
                 return_dict=True,
                 output_attentions=False,
                 output_hidden_states=False,
             )
             next_tokens = output.generated_tokens.view(self.on_device_generation_steps, batch_size).T
+            done = torch.all(
+                output.done.view(self.on_device_generation_steps, decoder_ipu_config.inference_replication_factor),
+                dim=-1,
+            )
 
             # update generated ids, model inputs, and length for next step
             input_ids = torch.cat([input_ids, next_tokens], dim=-1)
 
             generation_step += self.on_device_generation_steps
 
             # stop when each sentence is finished, or if we exceed the maximum length
-            if torch.any(output.done) or stopping_criteria(input_ids, ()):
+            if torch.any(done) or stopping_criteria(input_ids, ()):
                 break
 
         return input_ids
 
     def _on_device_beam_search(
         self,
         input_ids: torch.Tensor,
@@ -1701,17 +1843,19 @@
         if (max_length - context_length) % self.on_device_generation_steps != 0:
             logger.info(
                 "`max_length - context_length` does not evenly divide `on_device_generation_steps` "
                 f"({max_length - context_length} vs {self.on_device_generation_steps}). Generation will be done "
                 f"{self.on_device_generation_steps} tokens at a time and stop short of `max_length` so as not to exceed it."
             )
 
-        if self.ipu_config.inference_device_iterations != 1:
+        decoder_ipu_config = getattr(self, "decoder_ipu_config", self.ipu_config)
+        if decoder_ipu_config.inference_device_iterations not in (1, self.on_device_generation_steps):
             raise ValueError(
-                "On device generation expects `inference_device_iterations=1`, "
+                "On device generation expects `inference_device_iterations=1` or "
+                "`inference_device_iterations=on_device_generation_steps`, "
                 f"received {self.ipu_config.inference_device_iterations}. "
                 "For on device generation, `inference_device_iterations` will be set to "
                 f"`on_device_generation_steps={self.on_device_generation_steps}`."
             )
         if hasattr(self, "decoder_ipu_config"):
             self.decoder_ipu_config.inference_device_iterations = self.on_device_generation_steps
         else:
@@ -1727,47 +1871,54 @@
         model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
         # A model-agnostic version of above mainly to duplicate inputs for device iterations.
         model_inputs = self._prepare_inputs_for_on_device_generation(
             model_inputs, self.on_device_generation_steps, batch_beam_size
         )
 
-        on_device_generation_model_ctr = lambda inst: OnDeviceGenerationModel(
-            inst,
-            batch_size=batch_size,
-            max_length=max_length,
-            pad_token_id=pad_token_id,
-            eos_token_id=eos_token_id,
-            logits_processor=logits_processor,
-            num_beams=num_beams,
-            use_cache=True,
-            length_penalty=beam_scorer.length_penalty,
-            early_stopping=beam_scorer.do_early_stopping,
-        )
+        per_replica_batch_size = batch_size // decoder_ipu_config.inference_replication_factor
+
+        def on_device_generation_model_ctr(inst):
+            return OnDeviceGenerationModel(
+                inst,
+                batch_size=per_replica_batch_size,
+                max_length=max_length,
+                pad_token_id=pad_token_id,
+                eos_token_id=eos_token_id,
+                logits_processor=logits_processor,
+                num_beams=num_beams,
+                use_cache=True,
+                length_penalty=beam_scorer.length_penalty,
+                early_stopping=beam_scorer.do_early_stopping,
+            )
 
         generation_step = 0
         while True:
             output = self._call_generate(
                 generation_step=generation_step,  # NB: equal to `cur_len - 1` since context_length=1
                 on_device_generation_model_ctr=on_device_generation_model_ctr,
                 **model_inputs,
                 return_dict=True,
                 output_attentions=False,
                 output_hidden_states=False,
             )
+            done = torch.all(
+                output.done.view(self.on_device_generation_steps, decoder_ipu_config.inference_replication_factor),
+                dim=-1,
+            )
 
             generation_step += self.on_device_generation_steps
 
-            first_done = torch.argmax(output.done.int())
+            first_done = torch.argmax(done.int())
 
             input_ids = output.generated_tokens[
                 first_done * batch_size : (first_done + 1) * batch_size, : context_length + generation_step
             ].to(input_ids.dtype)
 
-            if torch.any(output.done) or stopping_criteria(input_ids, ()):
+            if torch.any(done) or stopping_criteria(input_ids, ()):
                 break
 
         return input_ids
 
     def _on_device_sample(self):
         raise NotImplementedError("On device sampling is not supported.")
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/ipu_configuration.py` & `optimum-graphcore-0.7.0/optimum/graphcore/ipu_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 #  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,24 +16,24 @@
 
 import copy
 import json
 import warnings
 from collections import defaultdict
 from functools import partial
 from tempfile import NamedTemporaryFile
-from typing import Any, Dict, List, Optional, Sequence, Set, Type, Union, get_type_hints
-
-import torch
+from typing import Any, Dict, List, Optional, Sequence, Union, get_type_hints
 
 import popart
 import poptorch
+import torch
 import typeguard
+from poptorch import Options, OutputMode
+
 from optimum.configuration_utils import BaseConfig
 from optimum.utils import logging
-from poptorch import Options, OutputMode
 
 
 # For container types check all items for type correctness
 # rather than just the first element
 typeguard._config.global_config.collection_check_strategy = typeguard.config.collection_check_strategy.ALL_ITEMS
 logger = logging.get_logger(__name__)
 
@@ -347,40 +348,17 @@
         fallback_matmul_proportion = self.matmul_proportion
         if isinstance(self.matmul_proportion, list) and len(self.matmul_proportion) != self.inference_ipus_per_replica:
             fallback_matmul_proportion = 0.2
         self.inference_matmul_proportion = (
             inference_matmul_proportion if inference_matmul_proportion else fallback_matmul_proportion
         )
 
-        def check_and_set_replication_factor(attr_name, attr, default=False):
+        def check_and_set_replication_factor(attr_name, attr):
             if isinstance(attr, int):
                 setattr(self, attr_name, attr)
-            elif isinstance(attr, dict):
-                base_message = (
-                    f"Dictionary values for `{attr_name}`"
-                    " have been deprecated. Provide values of type `int` instead."
-                )
-
-                if "default" not in attr:
-                    raise ValueError(
-                        base_message + f" Attempted to use the `default`"
-                        f" replication factor in `{attr_name}={attr}"
-                        " however no such key exists."
-                    )
-
-                try:
-                    setattr(self, attr_name, attr.get("default"))
-                except TypeError as e:
-                    raise TypeError(
-                        base_message + f" Attempted to set"
-                        f" `{attr_name}` using the `default` key of `{attr_name}`"
-                        " but a TypeError was raised. Check the error traceback for more information."
-                    ) from e
-
-                warnings.warn(base_message, FutureWarning, stacklevel=2)
             else:
                 raise ValueError(f"{attr_name} must be of type `int`. You provided: {attr_name}={attr}, {type(attr)}.")
 
         check_and_set_replication_factor("replication_factor", replication_factor)
         check_and_set_replication_factor("inference_replication_factor", inference_replication_factor)
 
         # Non-transformer layers initialisation
@@ -390,20 +368,20 @@
         self.inference_serialized_embedding_splits_per_ipu = inference_serialized_embedding_splits_per_ipu
 
         self.projection_serialization_factor = projection_serialization_factor
         self.inference_projection_serialization_factor = inference_projection_serialization_factor
         self.serialized_projection_splits_per_ipu = serialized_projection_splits_per_ipu
         self.inference_serialized_projection_splits_per_ipu = inference_serialized_projection_splits_per_ipu
 
-        if "sharded_execution_for_inference" in kwargs:
+        if kwargs.pop("sharded_execution_for_inference", None):
             warnings.warn(
                 'The "sharded_execution_for_inference" parameter is deprecated, sharded execution is always used during inference'
             )
 
-        if "enable_half_first_order_momentum" in kwargs:
+        if kwargs.pop("enable_half_first_order_momentum", None):
             warnings.warn('The "enable_half_first_order_momentum" parameter is deprecated')
 
         self.gradient_accumulation_steps = gradient_accumulation_steps
         self.device_iterations = device_iterations
         self.inference_device_iterations = inference_device_iterations
         self.optimizer_state_offchip = optimizer_state_offchip
         self.replicated_tensor_sharding = replicated_tensor_sharding
@@ -413,14 +391,20 @@
         self.embedding_serialization_factor = embedding_serialization_factor
         self.recompute_checkpoint_every_layer = recompute_checkpoint_every_layer
         self.output_mode = output_mode
 
         # TODO: remove this if unnecessary.
         self.execute_encoder_on_cpu_for_generation = kwargs.pop("execute_encoder_on_cpu_for_generation", False)
 
+        # Raise error if user has provided unknown & unused kwarg
+        if unknown_kwargs := (set(kwargs) - set(BaseConfig().to_dict())):
+            raise IncompatibleIPUConfigError(
+                "IPUConfig received unknown arguments:\n" + "\n".join([f"  {k}={kwargs[k]}" for k in unknown_kwargs])
+            )
+
         self._validate_ipu_config()
 
     @property
     def mode(self) -> str:
         return self._mode
 
     @mode.setter
@@ -552,15 +536,15 @@
                         f" should use the same number of IPUs as {ipus_per_replica_mode_str}={self._ipus_per_replica}."
                     )
 
         self.mode = old_mode
         return self
 
     def _to_options(self, for_inference: bool = False, compile_only: bool = False) -> poptorch.Options:
-        if not compile_only and poptorch.ipuHardwareVersion() != 2:
+        if not compile_only and poptorch.ipuHardwareVersion() not in (2, 21):
             raise RuntimeError("This requires an IPU Mk2 system to run.")
 
         if self.execute_encoder_on_cpu_for_generation:
             raise NotImplementedError("execute_encoder_on_cpu_for_generation is not supported yet.")
 
         old_mode = self.mode
         self.eval() if for_inference else self.train()
@@ -618,21 +602,18 @@
             # Use Pipelined Execution
             opts.setExecutionStrategy(poptorch.PipelinedExecution(poptorch.AutoStage.AutoIncrement))
 
         # Compile offline (no IPUs required)
         if compile_only:
             opts.useOfflineIpuTarget()
 
-        matmul_proportion = copy.deepcopy(
-            self.inference_matmul_proportion if for_inference else self.matmul_proportion
-        )
-        ipus_per_replica = self.inference_ipus_per_replica if for_inference else self.ipus_per_replica
-        if isinstance(self.matmul_proportion, float):
-            matmul_proportion = [self.matmul_proportion] * ipus_per_replica
-        mem_prop = {f"IPU{i}": matmul_proportion[i] for i in range(ipus_per_replica)}
+        matmul_proportion = copy.deepcopy(self._matmul_proportion)
+        if isinstance(matmul_proportion, float):
+            matmul_proportion = [matmul_proportion] * self._ipus_per_replica
+        mem_prop = {f"IPU{i}": matmul_proportion[i] for i in range(self._ipus_per_replica)}
         opts.setAvailableMemoryProportion(mem_prop)
 
         # Enable caching the compiled executable to disk
         if self.executable_cache_dir and self.executable_cache_dir != "disabled":
             opts.enableExecutableCaching(self.executable_cache_dir)
 
         opts._Popart.set("saveInitializersToFile", NamedTemporaryFile().name)
@@ -696,14 +677,17 @@
             `Dict[str, Any]`: Dictionary of all the attributes that make up this configuration instance.
         """
         output = super().to_dict()
 
         # Remove type hints as they are not serializable
         output.pop("_attribute_type_hints", None)
 
+        # Remove mode as it's not relevant for a dict
+        output.pop("_mode", None)
+
         return output
 
     def batch_size_factor(self, for_inference: bool = False) -> int:
         """
         Computes the factor to apply to the micro batch size to calculate the combined batch size.
 
         Args:
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/modelcard.py` & `optimum-graphcore-0.7.0/optimum/graphcore/modelcard.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/modeling_utils.py` & `optimum-graphcore-0.7.0/optimum/graphcore/modeling_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,24 +11,23 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from __future__ import annotations
 
 import copy
-from inspect import signature
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn.functional as F
 from torch import nn
+from transformers import PreTrainedModel
 
-import poptorch
 from optimum.utils import logging
-from transformers import PreTrainedModel
 
 from .ipu_configuration import IncompatibleIPUConfigError, IPUConfig
 
 
 logger = logging.get_logger(__name__)
 
 
@@ -86,15 +86,17 @@
             ipu_config ([`IPUConfig`]):
                 The `IPUConfig` instance of the pipelined model.
 
         Returns:
             The pipelined version of the model.
         """
         config = copy.deepcopy(model.config)
+        generation_config = copy.deepcopy(model.generation_config)
         pipelined_model = cls(config)
+        pipelined_model.generation_config = generation_config
         pipelined_model.load_state_dict(model.state_dict())
         pipelined_model.ipu_config = copy.deepcopy(ipu_config)
         pipelined_model.training = model.training
         return pipelined_model
 
     @classmethod
     def from_pretrained_transformers(cls, model_name_or_path: str, ipu_config: IPUConfig, *model_args, **kwargs):
@@ -323,15 +325,15 @@
     # Split layers_per_ipu between the given num layers
     layers_per_ipu = _expand_layers_per_ipu_wildcard(ipu_config, num_encoder_layers + num_decoder_layers)
     cumsum = [sum(layers_per_ipu[: i + 1]) for i in range(len(layers_per_ipu))]
     try:
         cut = [i + 1 for i, c in enumerate(cumsum) if c == num_encoder_layers]
         # Choose the cut index that's the highest power of 2
         cut = max([num for num in cut if num & (num - 1) == 0])
-    except:
+    except Exception:
         raise IncompatibleIPUConfigError(
             f"Unable to find a valid split of ipu_config.{layers_per_ipu_mode_str}\n"
             "Arguments: \n"
             f"\tipu_config.{layers_per_ipu_mode_str}={ipu_config._layers_per_ipu}\n"
             f"\tnum_encoder_layers={num_encoder_layers}\n"
             f"\tnum_decoder_layers={num_decoder_layers}\n"
             "Possible causes: \n"
@@ -464,20 +466,25 @@
 
         # Num embeddings should be divisible by the serialization factor
         assert self.num_embeddings % self.serialization_factor == 0
         self.split_size = self.num_embeddings // self.serialization_factor
 
         freeze = not embedding.weight.requires_grad
         self.padding_idx = embedding.padding_idx
+        boundaries = torch.linspace(
+            self.split_size - 1, self.num_embeddings - 1, self.serialization_factor, dtype=torch.int
+        )
         self.split_embeddings = nn.ModuleList(
             [
                 nn.Embedding.from_pretrained(
                     embedding.weight[i * self.split_size : (i + 1) * self.split_size, :].detach(),
                     freeze=freeze,
-                    padding_idx=embedding.padding_idx if i == 0 else None,
+                    padding_idx=self.padding_idx - i * self.split_size
+                    if self.padding_idx and i == torch.bucketize(self.padding_idx, boundaries).item()
+                    else None,
                 )
                 for i in range(self.serialization_factor)
             ]
         )
 
     @classmethod
     def from_model(cls, embedding: nn.Embedding, serialization_factor: int) -> SerializedEmbedding:
@@ -601,75 +608,121 @@
     is split along the reducing dimension `nn.Linear.in_features` in equal parts.
     The forward call aggregates the partial sums obtained from each linear layer.
 
     Args:
         linear: A `nn.Linear` to wrap
         serialization_factor: The number of partitions of the linear layer. This must
             be a factor of linear.in_features
+        serialization_mode: The dimension of the matmul to serialize on.
+            For matrix A (m by n) multiplied by matrix B (n by p):
+            * ReducingDim: Split across the reducing dimension (n).
+            * OutputChannels: Split across the output channels (dimension p).
     """
 
     def __init__(
         self,
         linear: torch.nn.Linear,
         serialization_factor: int,
+        serialization_mode=poptorch.MatMulSerializationMode.OutputChannels,
     ) -> None:
         super().__init__()
 
         self.in_features = linear.in_features
         self.out_features = linear.out_features
-        if self.in_features % serialization_factor != 0:
-            raise ValueError(f"{linear.in_features=} must be divisible by {serialization_factor=}")
-
-        self.split_size = self.in_features // serialization_factor
+        self.serialization_mode = serialization_mode
         self.split_linear_layers = torch.nn.ModuleList()
-        for i in range(0, self.in_features, self.split_size):
-            split_linear = torch.nn.Linear(self.split_size, self.out_features, bias=False, dtype=linear.weight.dtype)
-            # initialise linear layer using a section of `linear` weight,
-            with torch.no_grad():
-                split_linear.weight.copy_(linear.weight[:, i : i + self.split_size].detach())
-            self.split_linear_layers.append(split_linear)
+
+        if serialization_mode is poptorch.MatMulSerializationMode.OutputChannels:
+            if self.out_features % serialization_factor != 0:
+                raise ValueError(f"{linear.out_features=} must be divisible by {serialization_factor=}")
+
+            self.split_size = self.out_features // serialization_factor
+            for i in range(0, self.out_features, self.split_size):
+                split_linear = torch.nn.Linear(
+                    self.in_features, self.split_size, bias=False, dtype=linear.weight.dtype
+                )
+                with torch.no_grad():
+                    split_linear.weight.copy_(linear.weight[i : i + self.split_size, :].detach())
+                self.split_linear_layers.append(split_linear)
+
+        elif serialization_mode is poptorch.MatMulSerializationMode.ReducingDim:
+            if self.in_features % serialization_factor != 0:
+                raise ValueError(f"{linear.in_features=} must be divisible by {serialization_factor=}")
+
+            self.split_size = self.in_features // serialization_factor
+            for i in range(0, self.in_features, self.split_size):
+                split_linear = torch.nn.Linear(
+                    self.split_size, self.out_features, bias=False, dtype=linear.weight.dtype
+                )
+                with torch.no_grad():
+                    split_linear.weight.copy_(linear.weight[:, i : i + self.split_size].detach())
+                self.split_linear_layers.append(split_linear)
+
+        else:
+            raise ValueError(
+                f"`SplitProjection` `serialization_mode` can only be {poptorch.MatMulSerializationMode.OutputChannels} or {poptorch.MatMulSerializationMode.ReducingDim}."
+                f" You provided: {serialization_mode=}"
+            )
 
         self.bias = None
         if linear.bias is not None:
             self.bias = torch.nn.Parameter(torch.zeros_like(linear.bias))
             with torch.no_grad():
                 self.bias.copy_(linear.bias.detach())
 
     def forward(self, x):
-        # each linear layer processes a partition of the input
-        out = None
-        for i, split_linear_layer in enumerate(self.split_linear_layers):
-            h = split_linear_layer(x[..., i * self.split_size : (i + 1) * self.split_size])
-            if out is None:
-                out = h
-            else:
-                out += h
+        if self.serialization_mode is poptorch.MatMulSerializationMode.OutputChannels:
+            out = []
+            for i, split_linear_layer in enumerate(self.split_linear_layers):
+                out.append(split_linear_layer(x))
+            out = torch.concat(out, -1)
+
+        elif self.serialization_mode is poptorch.MatMulSerializationMode.ReducingDim:
+            out = self.split_linear_layers[0](x[..., 0 : self.split_size])
+            for i, split_linear_layer in enumerate(self.split_linear_layers[1:]):
+                out += split_linear_layer(x[..., i * self.split_size : (i + 1) * self.split_size])
+
         if self.bias is not None:
             out += self.bias
+
         return out
 
     @classmethod
-    def from_model(cls, linear: torch.nn.Linear, serialization_factor: int) -> SplitProjection:
-        return cls(linear, serialization_factor)
+    def from_model(
+        cls,
+        linear: torch.nn.Linear,
+        serialization_factor: int,
+        serialization_mode=poptorch.MatMulSerializationMode.OutputChannels,
+    ) -> SplitProjection:
+        return cls(linear, serialization_factor, serialization_mode)
 
     def to_model(self) -> nn.Linear:
         """
         Merge the sub linear layers into one
 
         Returns:
             `nn.Linear` layer
         """
         dtype = self.split_linear_layers[0].weight.dtype
         layer = nn.Linear(self.in_features, self.out_features, bias=self.bias is not None)
         if dtype == torch.float16:
             layer = layer.half()
-        with torch.no_grad():
-            layer.weight.copy_(torch.hstack([l.weight.detach() for l in self.split_linear_layers]))
-            if self.bias is not None:
+
+        if self.serialization_mode is poptorch.MatMulSerializationMode.OutputChannels:
+            with torch.no_grad():
+                layer.weight.copy_(torch.vstack([l.weight.detach() for l in self.split_linear_layers]))
+
+        elif self.serialization_mode is poptorch.MatMulSerializationMode.ReducingDim:
+            with torch.no_grad():
+                layer.weight.copy_(torch.hstack([l.weight.detach() for l in self.split_linear_layers]))
+
+        if self.bias is not None:
+            with torch.no_grad():
                 layer.bias.copy_(self.bias)
+
         return layer
 
     def parallelize(self, splits_per_ipu: List[int]):
         for ipu_id, splits in enumerate(splits_per_ipu):
             if splits:
                 from_split = sum(splits_per_ipu[:ipu_id])
                 to_split = from_split + splits - 1
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/bart/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_bart import PipelinedBartForConditionalGeneration, PipelinedBartForSequenceClassification
+from .feature_extraction_whisper import WhisperFeatureExtractorTorch
+from .modeling_whisper import PipelinedWhisperForConditionalGeneration
+from .processing_whisper import WhisperProcessorTorch
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/bart/modeling_bart.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/bart/modeling_bart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,19 +13,17 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import copy
 import random
 from typing import List, Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
-
-import poptorch
-from optimum.utils import logging
 from transformers import BartForConditionalGeneration, BartForSequenceClassification, BartModel
 from transformers.modeling_outputs import (
     BaseModelOutput,
     BaseModelOutputWithPastAndCrossAttentions,
     Seq2SeqLMOutput,
     Seq2SeqModelOutput,
     Seq2SeqSequenceClassifierOutput,
@@ -34,14 +33,16 @@
     BartDecoder,
     BartEncoder,
     BartEncoderLayer,
     BartLearnedPositionalEmbedding,
     shift_tokens_right,
 )
 
+from optimum.utils import logging
+
 from ...generation import IPUAttentionMixin, IPUGenerationMixin, supports_kv_cache
 from ...modeling_utils import (
     PipelineMixin,
     SerializedLinear,
     SharedEmbedding,
     get_layer_ipu,
     recomputation_checkpoint,
@@ -102,15 +103,14 @@
         layer_head_mask: Optional[torch.Tensor] = None,
         output_attentions: bool = False,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
         """Input shape: Batch x Time x Channel"""
 
         # if key_value_states are provided this layer is used as a cross-attention layer
         # for the decoder
-        is_cross_attention = key_value_states is not None
 
         bsz, tgt_len, _ = hidden_states.size()
 
         # get query proj
         query_states = self.q_proj(hidden_states) * self.scaling
         if key_value_states is not None:
             # cross attention
@@ -139,16 +139,16 @@
             # all previous decoder key/value_states. Further calls to uni-directional self-attention
             # can concat previous decoder key/value_states to current projected key/value_states (third "elif" case)
             # if encoder bi-directional self-attention `past_key_value` is always `None`
             past_key_value = (key_states, value_states)
 
         proj_shape = (bsz * self.num_heads, -1, self.head_dim)
         query_states = self._shape(query_states, tgt_len, bsz).view(*proj_shape)
-        key_states = key_states.view(*proj_shape)
-        value_states = value_states.view(*proj_shape)
+        key_states = key_states.reshape(*proj_shape)
+        value_states = value_states.reshape(*proj_shape)
 
         src_len = key_states.size(1)
         attn_weights = torch.bmm(query_states, key_states.transpose(1, 2))
 
         if attn_weights.size() != (bsz * self.num_heads, tgt_len, src_len):
             raise ValueError(
                 f"Attention weights should be of size {(bsz * self.num_heads, tgt_len, src_len)}, but is {attn_weights.size()}"
@@ -180,15 +180,15 @@
 
         attn_probs = nn.functional.dropout(attn_weights, p=self.dropout, training=self.training)
 
         attn_output = torch.bmm(attn_probs, value_states)
 
         if attn_output.size() != (bsz * self.num_heads, tgt_len, self.head_dim):
             raise ValueError(
-                f"`attn_output` should be of size {(bsz, self.num_heads, tgt_len, self.head_dim)}, but is {attn_output.size()}"
+                f"`attn_output` should be of size {(bsz * self.num_heads, tgt_len, self.head_dim)}, but is {attn_output.size()}"
             )
 
         attn_output = attn_output.view(bsz, self.num_heads, tgt_len, self.head_dim)
         attn_output = attn_output.transpose(1, 2)
 
         # Use the `embed_dim` from the config (stored in the class) rather than `hidden_state` because `attn_output` can be
         # partitioned aross GPUs when using tensor-parallelism.
@@ -768,28 +768,31 @@
         Recommended usage:
         ```
         model = PipelinedBartForConditionalGeneration(config).parallelize().half()
         ```
         """
         super().parallelize()
 
+        if use_cache:
+            kwargs = self._populate_parallelize_kwargs_with_generation_config(**kwargs)
+
         logger.info("-------------------- Device Allocation --------------------")
         logger.info("Embedding  --> IPU 0")
 
         if self.ipu_config.embedding_serialization_factor > 1:
             self.lm_head = SerializedLinear.from_model(self.lm_head, self.ipu_config.embedding_serialization_factor)
             self.tie_weights()
 
         self.model.__class__ = _BartModelWithSharedEmbedding
         self.model.encoder_and_decoder_embeddings_computation(use_shared_embedding=True)
         self.model.change_bart_encoder_and_decoder_classes(restore=False)
         self.model.change_bart_attention_class(restore=False, use_cache=use_cache and for_generation, **kwargs)
         self.model.change_decoder_positional_embedding(restore=False)
         self.change_lm_head_to_indexed_input_linear(restore=not (for_generation and not use_cache))
-        self.use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
+        self._use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
         self.set_on_device_generation_steps(kwargs.get("on_device_generation_steps", 0))
 
         self.model.shared = poptorch.BeginBlock(self.model.shared, "Embedding", ipu_id=0)
         self.model.encoder.embed_positions = poptorch.BeginBlock(
             self.model.encoder.embed_positions, "Embedding", ipu_id=0
         )
         self.model.encoder.layernorm_embedding = poptorch.BeginBlock(
@@ -855,28 +858,35 @@
         if isinstance(self.lm_head, SerializedLinear):
             self.lm_head = self.lm_head.to_model()
             self.tie_weights()
 
         return self
 
     def prepare_inputs_for_generation(
-        self, decoder_input_ids, past=None, use_cache=None, encoder_outputs=None, attention_mask=None, **kwargs
+        self,
+        decoder_input_ids,
+        past_key_values=None,
+        use_cache=None,
+        encoder_outputs=None,
+        attention_mask=None,
+        decoder_attention_mask=None,
+        **kwargs,
     ):
-        # We don't use `past` for KV caching, and rely on `use_cache` instead.
+        # We don't use `past_key_values` for KV caching, and rely on `use_cache` instead.
         beam_idx = None
         if use_cache:
             decoder_input_ids = decoder_input_ids[:, -1:]
             beam_idx = kwargs.get("beam_idx", torch.arange(decoder_input_ids.shape[0], dtype=torch.long))
 
         return {
             "encoder_outputs": encoder_outputs,
             "past_key_values": None,
             "attention_mask": attention_mask,
             "decoder_input_ids": decoder_input_ids,
-            "decoder_attention_mask": None,
+            "decoder_attention_mask": decoder_attention_mask,
             "beam_idx": beam_idx,
         }
 
     def forward(
         self,
         input_ids: torch.LongTensor = None,
         attention_mask: Optional[torch.Tensor] = None,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/bert/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/bert/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/bert/bert_fused_attention.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/bert/bert_fused_attention.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 # limitations under the License.
 
 import math
 from typing import Tuple
 
 import torch
 import torch.nn as nn
-
 from transformers.models.bert.modeling_bert import BertSelfAttention
 
 
 class BertFusedSelfAttention(BertSelfAttention):
     def fused_qkv(self, hidden_state: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         weights = (self.query.weight, self.key.weight, self.value.weight)
         combined_weight = torch.cat(weights, dim=0)
         combined_result = hidden_state @ torch.transpose(combined_weight, -2, -1)
         biases = (self.query.bias, self.key.bias, self.value.bias)
-        if all(map(lambda b: b is not None, biases)):
+        if all((b is not None for b in biases)):
             combined_bias = torch.cat(biases, dim=0)
             combined_result += combined_bias
-        elif any(map(lambda b: b is not None, biases)):
+        elif any((b is not None for b in biases)):
             raise RuntimeError(
                 "Some attention layers had biases but not all. This is not supported. "
                 "Please enable biases on all Query, Key and Value or none. "
                 f"query.bias = {biases[0] is not None}, "
                 f"key.bias = {biases[1] is not None}, "
                 f"value.bias = {biases[2] is not None}"
             )
@@ -80,17 +79,17 @@
             # if encoder bi-directional self-attention `past_key_value` is always `None`
             past_key_value = (key_layer, value_layer)
 
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
 
         if self.position_embedding_type == "relative_key" or self.position_embedding_type == "relative_key_query":
-            seq_length = hidden_states.size()[1]
-            position_ids_l = torch.arange(seq_length, dtype=torch.long, device=hidden_states.device).view(-1, 1)
-            position_ids_r = torch.arange(seq_length, dtype=torch.long, device=hidden_states.device).view(1, -1)
+            query_length, key_length = query_layer.shape[2], key_layer.shape[2]
+            position_ids_l = torch.arange(query_length, dtype=torch.long, device=hidden_states.device).view(-1, 1)
+            position_ids_r = torch.arange(key_length, dtype=torch.long, device=hidden_states.device).view(1, -1)
             distance = position_ids_l - position_ids_r
             positional_embedding = self.distance_embedding(distance + self.max_position_embeddings - 1)
             positional_embedding = positional_embedding.to(dtype=query_layer.dtype)  # fp16 compatibility
 
             if self.position_embedding_type == "relative_key":
                 relative_position_scores = torch.einsum("bhld,lrd->bhlr", query_layer, positional_embedding)
                 attention_scores = attention_scores + relative_position_scores
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/bert/modeling_bert.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/bert/modeling_bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2018 The Google AI Language Team Authors and The HuggingFace Inc. team.
+# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
 # Copyright (c) 2021 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -10,32 +12,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
-import poptorch
-from optimum.utils import logging
 from scipy.stats import truncnorm
 from transformers import (
     BertForMaskedLM,
     BertForMultipleChoice,
     BertForPreTraining,
     BertForQuestionAnswering,
     BertForSequenceClassification,
     BertForTokenClassification,
 )
 from transformers.modeling_outputs import MaskedLMOutput, QuestionAnsweringModelOutput
 from transformers.models.bert.modeling_bert import BertForPreTrainingOutput, BertSelfAttention
 
+from optimum.utils import logging
+
 from ...modeling_utils import (
     OnehotGather,
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     outline_attribute,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/convnext/modeling_convnext.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/convnext/modeling_convnext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import poptorch
-from optimum.utils import logging
 from transformers.models.convnext.modeling_convnext import ConvNextForImageClassification, ConvNextLayer
 
+from optimum.utils import logging
+
 from ...modeling_utils import PipelineMixin, get_layer_ipu, register
 from .optimized_convnextlayer import OptimizedConvNextLayer
 
 
 logger = logging.get_logger(__name__)
 
 
@@ -30,15 +31,15 @@
 
         # Use optimized ConvNextLayer
         for stage in self.convnext.encoder.stages:
             for layer in stage.layers:
                 layer.__class__ = OptimizedConvNextLayer
 
         logger.info("---------- Device Allocation -----------")
-        logger.info(f"Embedding  --> IPU 0")
+        logger.info("Embedding  --> IPU 0")
         self.convnext.embeddings = poptorch.BeginBlock(self.convnext.embeddings, "Embedding", ipu_id=0)
 
         num_encoder_layers = sum([len(stage.layers) for stage in self.convnext.encoder.stages])
         layer_ipu = get_layer_ipu(self.ipu_config, num_encoder_layers)
         global_layer_idx = 0
         for stage_idx, stage in enumerate(self.convnext.encoder.stages):
             for layer_idx, layer in enumerate(stage.layers):
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_deberta import (
-    PipelinedDebertaForMaskedLM,
-    PipelinedDebertaForQuestionAnswering,
-    PipelinedDebertaForSequenceClassification,
-    PipelinedDebertaForTokenClassification,
+from .modeling_distilbert import (
+    PipelinedDistilBertForMaskedLM,
+    PipelinedDistilBertForMultipleChoice,
+    PipelinedDistilBertForQuestionAnswering,
+    PipelinedDistilBertForSequenceClassification,
+    PipelinedDistilBertForTokenClassification,
 )
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/deberta/modeling_deberta.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/modeling_deberta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,34 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
-import poptorch
-from optimum.utils import logging
 from transformers import (
     DebertaForMaskedLM,
     DebertaForQuestionAnswering,
     DebertaForSequenceClassification,
     DebertaForTokenClassification,
 )
 from transformers.modeling_outputs import MaskedLMOutput, QuestionAnsweringModelOutput
 from transformers.models.deberta.modeling_deberta import (
     DebertaEncoder,
     DisentangledSelfAttention,
     StableDropout,
     build_relative_position,
 )
 
+from optimum.utils import logging
+
 from ...modeling_utils import (
     OnehotGather,
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     outline_attribute,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_distilbert import (
-    PipelinedDistilBertForMaskedLM,
-    PipelinedDistilBertForMultipleChoice,
-    PipelinedDistilBertForQuestionAnswering,
-    PipelinedDistilBertForSequenceClassification,
-    PipelinedDistilBertForTokenClassification,
+from .modeling_roberta import (
+    PipelinedRobertaForMaskedLM,
+    PipelinedRobertaForMultipleChoice,
+    PipelinedRobertaForQuestionAnswering,
+    PipelinedRobertaForSequenceClassification,
+    PipelinedRobertaForTokenClassification,
 )
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/distilbert/modeling_distilbert.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/distilbert/modeling_distilbert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,30 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
-import poptorch
-from optimum.utils import logging
 from transformers import (
     DistilBertForMaskedLM,
     DistilBertForMultipleChoice,
     DistilBertForQuestionAnswering,
     DistilBertForSequenceClassification,
     DistilBertForTokenClassification,
 )
 from transformers.modeling_outputs import MaskedLMOutput, QuestionAnsweringModelOutput
 from transformers.models.distilbert.modeling_distilbert import MultiHeadSelfAttention
 
+from optimum.utils import logging
+
 from ...modeling_utils import (
     OnehotGather,
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     recomputation_checkpoint,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_gpt2 import (
-    PipelinedGPT2ForSequenceClassification,
-    PipelinedGPT2ForTokenClassification,
-    PipelinedGPT2LMHeadModel,
-)
+from .modeling_wav2vec2 import PipelinedWav2Vec2ForCTC, PipelinedWav2Vec2ForPreTraining
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/gpt2/modeling_gpt2.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/modeling_gpt2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
-
-import poptorch
-from optimum.utils import logging
 from transformers import GPT2ForSequenceClassification, GPT2ForTokenClassification, GPT2LMHeadModel
 from transformers.modeling_outputs import CausalLMOutputWithCrossAttentions, SequenceClassifierOutputWithPast
 from transformers.models.gpt2.modeling_gpt2 import GPT2Attention
 
+from optimum.utils import logging
+
 from ...generation import IPUGenerationMixin
 from ...modeling_utils import (
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     outline_attribute,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
-# Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_attention.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # RANDOM CHANGE
 
 import math
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 
 import torch
 import torch.nn as nn
-
-from optimum.utils import logging
 from transformers.modeling_utils import find_pruneable_heads_and_indices, prune_linear_layer
 from transformers.models.bert.modeling_bert import BertSelfAttention
 
+from optimum.utils import logging
+
 
 logger = logging.get_logger(__name__)
 
 
 class GroupBertFusedSelfAttention(BertSelfAttention):
     def fused_qkv(self, hidden_state: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         weights = (self.query.weight, self.key.weight, self.value.weight)
         combined_weight = torch.cat(weights, dim=0)
         combined_result = hidden_state @ torch.transpose(combined_weight, -2, -1)
         biases = (self.query.bias, self.key.bias, self.value.bias)
-        if all(map(lambda b: b is not None, biases)):
+        if all((b is not None for b in biases)):
             combined_bias = torch.cat(biases, dim=0)
             combined_result += combined_bias
-        elif any(map(lambda b: b is not None, biases)):
+        elif any((b is not None for b in biases)):
             raise RuntimeError(
                 "Some attention layers had biases but not all. This is not supported. "
                 "Please enable biases on all Query, Key and Value or none. "
                 f"query.bias = {biases[0] is not None}, "
                 f"key.bias = {biases[1] is not None}, "
                 f"value.bias = {biases[2] is not None}"
             )
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_convolution.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # RANDOM CHANGE
 
-import math
-from typing import Tuple
 
 import torch
 import torch.nn as nn
 
 from optimum.utils import logging
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/groupbert_ffn.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/groupbert_ffn.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # RANDOM CHANGE
 
-import math
-from typing import Tuple
 
 import torch
 import torch.nn as nn
+from transformers.activations import ACT2FN
 
 from optimum.utils import logging
-from transformers.activations import ACT2FN
 
 
 logger = logging.get_logger(__name__)
 
 
 class GroupBertIntermediate(nn.Module):
     """
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/groupbert/modeling_groupbert.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/groupbert/modeling_groupbert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-# /usr/bin/python3
-# Copyright (c) 2021 Graphcore Ltd. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
-import poptorch
-from optimum.utils import logging
 from scipy.stats import truncnorm
 from transformers import (
     BertConfig,
     BertForMaskedLM,
     BertForMultipleChoice,
     BertForPreTraining,
     BertForQuestionAnswering,
@@ -35,14 +32,16 @@
     BaseModelOutputWithPastAndCrossAttentions,
     MaskedLMOutput,
     QuestionAnsweringModelOutput,
 )
 from transformers.modeling_utils import apply_chunking_to_forward
 from transformers.models.bert.modeling_bert import BertForPreTrainingOutput, BertModel
 
+from optimum.utils import logging
+
 from ...modeling_utils import (
     OnehotGather,
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     outline_attribute,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/ipu_layer_drop.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/ipu_layer_drop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2021 The Fairseq Authors and the HuggingFace Inc. team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,16 +16,14 @@
 
 """
 These are the same blocks as in the original implementation in transformers,
 but with a traceable implementation of LayerDrop.
 """
 
 import torch
-from torch.nn import functional as F
-
 from transformers.modeling_outputs import BaseModelOutput
 from transformers.models.hubert.modeling_hubert import HubertEncoder, HubertEncoderStableLayerNorm
 
 
 class IPUHubertEncoder(HubertEncoder):
     def forward(
         self,
@@ -58,15 +57,15 @@
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_outputs = layer(hidden_states, attention_mask=attention_mask, output_attentions=output_attentions)
 
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
             # Modify LayerDrop so it can be statically compiled without eager mode
             if self.config.layerdrop > 0.0:
-                dropout_probability = torch.rand(tuple(), device=hidden_states.device)
+                dropout_probability = torch.rand((), device=hidden_states.device)
                 skip_the_layer = (
                     torch.tensor(self.training, device=hidden_states.device)
                     & (dropout_probability < self.config.layerdrop)
                 ).to(dtype=hidden_states.dtype)
                 hidden_states = hidden_states * skip_the_layer + layer_outputs[0] * (1 - skip_the_layer)
             else:
                 hidden_states = layer_outputs[0]
@@ -121,15 +120,15 @@
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_outputs = layer(hidden_states, attention_mask=attention_mask, output_attentions=output_attentions)
 
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
             # Modify LayerDrop so it can be statically compiled without eager mode
             if self.config.layerdrop > 0.0:
-                dropout_probability = torch.rand(tuple(), device=hidden_states.device)
+                dropout_probability = torch.rand((), device=hidden_states.device)
                 skip_the_layer = (
                     torch.tensor(self.training, device=hidden_states.device)
                     & (dropout_probability < self.config.layerdrop)
                 ).to(dtype=hidden_states.dtype)
                 hidden_states = hidden_states * skip_the_layer + layer_outputs[0] * (1 - skip_the_layer)
             else:
                 hidden_states = layer_outputs[0]
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/hubert/modeling_hubert.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/hubert/modeling_hubert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2021 The Fairseq Authors and the HuggingFace Inc. team. All rights reserved.
 # Copyright (c) 2021 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -10,22 +11,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
-import torch
-
 import poptorch
-from optimum.utils import logging
+import torch
 from transformers import HubertForCTC, HubertForSequenceClassification
 from transformers.modeling_outputs import CausalLMOutput
 from transformers.models.hubert.modeling_hubert import HubertEncoder, HubertEncoderStableLayerNorm
 
+from optimum.utils import logging
+
 from ...modeling_utils import PipelineMixin, get_layer_ipu, recomputation_checkpoint, register
 from .ipu_layer_drop import IPUHubertEncoder, IPUHubertEncoderStableLayerNorm
 
 
 logger = logging.get_logger(__name__)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/t5/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_lxmert import PipelinedLxmertForQuestionAnswering
+from .modeling_t5 import PipelinedT5ForConditionalGeneration, PipelinedT5EncoderModel
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/lxmert/modeling_lxmert.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/modeling_lxmert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2018 Hao Tan, Mohit Bansal, and the HuggingFace team
 # Copyright (c) 2021 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -10,22 +11,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn.functional as F
-
-import poptorch
-from optimum.utils import logging
 from transformers import LxmertForQuestionAnswering
 from transformers.models.lxmert.modeling_lxmert import LxmertForQuestionAnsweringOutput
 
+from optimum.utils import logging
+
 from ...modeling_utils import PipelineMixin, recomputation_checkpoint, register
 
 
 logger = logging.get_logger(__name__)
 
 
 @register(LxmertForQuestionAnswering)
@@ -68,18 +69,18 @@
         for index, layer in enumerate(self.lxmert.encoder.x_layers):
             if self.ipu_config.recompute_checkpoint_every_layer:
                 h = recomputation_checkpoint(layer)
                 self._hooks.append(h)
             self.lxmert.encoder.x_layers[index] = poptorch.BeginBlock(layer, f"Cross modality layer{index}", ipu_id=3)
             logger.info(f"Cross modality layer {index:<2} --> IPU 3")
 
-        logger.info(f"Pooler                  --> IPU 3")
+        logger.info("Pooler                  --> IPU 3")
         self.lxmert.pooler = poptorch.BeginBlock(self.lxmert.pooler, "Pooler", ipu_id=3)
 
-        logger.info(f"Head                    --> IPU 3")
+        logger.info("Head                    --> IPU 3")
         self.answer_head = poptorch.BeginBlock(self.answer_head, "Head", ipu_id=3)
         logger.info("-----------------------------------------------------------")
         return self
 
     def forward(
         self,
         input_ids: Optional[torch.LongTensor] = None,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/mt5/modeling_mt5.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/mt5/modeling_mt5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+#  Copyright 2020 Mesh TensorFlow authors, T5 Authors and HuggingFace Inc. team.
+#  Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,24 +12,24 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import warnings
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
 from torch import Tensor
-
-import poptorch
-from optimum.utils import logging
 from transformers import MT5ForConditionalGeneration
 from transformers.activations import NewGELUActivation
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
-from transformers.models.t5.modeling_t5 import __HEAD_MASK_WARNING_MSG, T5Block, T5Stack
+from transformers.models.mt5.modeling_mt5 import __HEAD_MASK_WARNING_MSG, MT5Block, MT5Stack
+
+from optimum.utils import logging
 
 from ...generation import IPUGenerationMixin
 from ...modeling_utils import (
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     SharedEmbedding,
@@ -63,15 +64,15 @@
         safe_input = torch.where(safe, input, 0.0)
         gelu = super().forward(safe_input)
         relu = nn.functional.relu(input)
         return torch.where(safe, gelu, relu)
 
 
 # Copied from optimum.graphcore.models.t5.modeling_t5.CustomT5Block with t5->mt5 and T5->MT5
-class CustomMT5Block(T5Block):
+class CustomMT5Block(MT5Block):
     def forward(
         self,
         hidden_states,
         attention_mask=None,
         position_bias=None,
         encoder_hidden_states=None,
         encoder_attention_mask=None,
@@ -169,15 +170,15 @@
         else:
             outputs = outputs + attention_outputs
 
         return outputs  # hidden-states, present_key_value_states, (self-attention position bias), (self-attention weights), (cross-attention position bias), (cross-attention weights)
 
 
 # Copied from optimum.graphcore.models.t5.modeling_t5.CustomT5Stack with t5->mt5 and T5->MT5
-class CustomMT5Stack(T5Stack):
+class CustomMT5Stack(MT5Stack):
     def invert_attention_mask(self, *args, **kwargs) -> Tensor:
         return super().invert_attention_mask(*args, **kwargs) * 0.75
 
     def get_extended_attention_mask(self, *args, **kwargs) -> Tensor:
         return super().get_extended_attention_mask(*args, **kwargs) * 0.75
 
 
@@ -420,28 +421,28 @@
         if self.lm_head.__class__ == SerializedLinear:
             self.lm_head = self.lm_head.to_model()
             if self.config.tie_word_embeddings:
                 self.tie_weights()
         elif self.lm_head.__class__ == SplitProjection:
             self.lm_head = self.lm_head.to_model()
 
-        self.encoder.__class__ = T5Stack
-        self.decoder.__class__ = T5Stack
+        self.encoder.__class__ = MT5Stack
+        self.decoder.__class__ = MT5Stack
 
         for block in self.encoder.block:
-            block.__class__ = T5Block
+            block.__class__ = MT5Block
             block.layer[0].dropout = block.layer[0].dropout.module
             with torch.no_grad():
                 block.layer[1].DenseReluDense.wo.weight *= block.layer[1].dropout.scale
             block.layer[1].dropout = block.layer[1].dropout.module
             if self.config.dense_act_fn == "gelu_new":
                 block.layer[1].DenseReluDense.act = NewGELUActivation()
 
         for block in self.decoder.block:
-            block.__class__ = T5Block
+            block.__class__ = MT5Block
             if self.config.dense_act_fn == "gelu_new":
                 block.layer[2].DenseReluDense.act = NewGELUActivation()
 
         return self
 
     # Copied from optimum.graphcore.models.t5.modeling_t5.PipelinedT5ForConditionalGenerationCustomT5Stack.forward
     def forward(
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/deberta/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_roberta import (
-    PipelinedRobertaForMaskedLM,
-    PipelinedRobertaForMultipleChoice,
-    PipelinedRobertaForQuestionAnswering,
-    PipelinedRobertaForSequenceClassification,
-    PipelinedRobertaForTokenClassification,
+from .modeling_deberta import (
+    PipelinedDebertaForMaskedLM,
+    PipelinedDebertaForQuestionAnswering,
+    PipelinedDebertaForSequenceClassification,
+    PipelinedDebertaForTokenClassification,
 )
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/roberta/modeling_roberta.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/roberta/modeling_roberta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2018 The Google AI Language Team Authors and The HuggingFace Inc. team.
+# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
 # Copyright (c) 2021 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -10,29 +12,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
-import torch.nn as nn
 from torch.nn import CrossEntropyLoss
-
-import poptorch
-from optimum.utils import logging
 from transformers import (
     RobertaForMaskedLM,
     RobertaForMultipleChoice,
     RobertaForQuestionAnswering,
     RobertaForSequenceClassification,
     RobertaForTokenClassification,
 )
 from transformers.modeling_outputs import MaskedLMOutput, QuestionAnsweringModelOutput
 
+from optimum.utils import logging
+
 from ...modeling_utils import (
     OnehotGather,
     PipelineMixin,
     SerializedEmbedding,
     SerializedLinear,
     get_layer_ipu,
     outline_attribute,
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/t5/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/gpt2/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_t5 import PipelinedT5ForConditionalGeneration
+from .modeling_gpt2 import (
+    PipelinedGPT2ForSequenceClassification,
+    PipelinedGPT2ForTokenClassification,
+    PipelinedGPT2LMHeadModel,
+)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/t5/modeling_t5.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/t5/modeling_t5.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #  Copyright 2022 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,24 +12,24 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import warnings
 from typing import Optional, Tuple, Union
 
+import poptorch
 import torch
 import torch.nn as nn
 from torch import Tensor
-
-import poptorch
-from optimum.utils import logging
 from transformers import T5ForConditionalGeneration
 from transformers.activations import NewGELUActivation
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
-from transformers.models.t5.modeling_t5 import __HEAD_MASK_WARNING_MSG, T5Block, T5Stack
+from transformers.models.t5.modeling_t5 import __HEAD_MASK_WARNING_MSG, T5Block, T5EncoderModel, T5Stack
+
+from optimum.utils import logging
 
 from ...generation import IPUGenerationMixin
 from ...modeling_utils import (
     PipelineMixin,
     SerializedLinear,
     SharedEmbedding,
     get_layer_ipu,
@@ -468,7 +469,101 @@
             decoder_hidden_states=decoder_outputs.hidden_states,
             decoder_attentions=decoder_outputs.attentions,
             cross_attentions=decoder_outputs.cross_attentions,
             encoder_last_hidden_state=encoder_outputs.last_hidden_state,
             encoder_hidden_states=encoder_outputs.hidden_states,
             encoder_attentions=encoder_outputs.attentions,
         )
+
+
+@register(T5EncoderModel)
+class PipelinedT5EncoderModel(T5EncoderModel, PipelineMixin):
+    def parallelize(self):
+        """
+        Transform the model to run in an IPU pipeline.
+        - Adds pipeline stages to the model
+        - Adds recomputation checkpoints
+
+        Recommended usage:
+        ```
+        model = PipelinedT5EncoderModel(config).parallelize().half()
+        ```
+        """
+        PipelineMixin.parallelize(self)
+
+        logger.info("-------------------- Device Allocation --------------------")
+        logger.info("Embedding  --> IPU 0")
+
+        self.shared = poptorch.BeginBlock(self.shared, "Embedding", ipu_id=0)
+
+        # Use a custom T5Stack implementation because sharing the position bias causes OOM error
+        self.encoder.__class__ = CustomT5Stack
+
+        # Upcast input embeddings so that the residuals remain in FP32. This
+        # cast is reversed where necessary by the T5LayerNorm layers in:
+        # - first layer of T5LayerSelfAttention
+        # - first layer of T5LayerFF
+        # - final_layer_norm
+        # Which, conveniently, are all the places that this needs to happen.
+        # Therefore, so we just need to upcast immediately before the residual
+        # adds in T5LayerSelfAttention and T5LayerFF. This is handled in the
+        # for loop below.
+        self.encoder.embed_tokens = UpCastWrapper(self.encoder.embed_tokens)
+
+        # Use a custom T5Block implementation that removes a dynamic if blocks that can't be statically traced
+        for block in self.encoder.block:
+            block.__class__ = CustomT5Block
+            # Dropout happens immediately before the residual add. Inserting a
+            # cast in T5LayerSelfAttention and T5LayerFF keeps the residual
+            # structure in FP32
+            block.layer[0].dropout = UpCastWrapper(block.layer[0].dropout)
+            # Scale down the weights for the T5LayerFF down-projection and
+            # then scale its output back up again after it is cast to FP32
+            scale = 8.0
+            with torch.no_grad():
+                block.layer[1].DenseReluDense.wo.weight /= scale
+            block.layer[1].dropout = UpCastWrapper(block.layer[1].dropout, scale)
+            # Prevent overflow in NewGELUActivation
+            if self.config.dense_act_fn == "gelu_new":
+                # TODO: Work-around bug with torch.nn.GELU(approximate="tanh"). Replace
+                # this with block.layer[1].DenseReluDense.act = torch.nn.GELU(approximate="tanh")
+                # when bug is fixed
+                block.layer[1].DenseReluDense.act = CustomGELU()
+
+        num_encoder_layers = len(self.encoder.block)
+        number_of_layers = num_encoder_layers
+        encoder_layer_ipu = get_layer_ipu(self.ipu_config, number_of_layers)
+
+        for index, (layer, ipu) in enumerate(zip(self.encoder.block, encoder_layer_ipu)):
+            if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_layers - 1:
+                self._hooks.append(recomputation_checkpoint(layer))
+            self.encoder.block[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
+            logger.info(f"Encoder {index:<2} --> IPU {ipu}")
+
+        self.encoder.final_layer_norm = poptorch.BeginBlock(
+            self.encoder.final_layer_norm, "Encoder Stack Final LayerNorm", ipu_id=ipu
+        )
+
+        return self
+
+    def deparallelize(self):
+        """
+        Undo the changes to the model done by `parallelize`.
+        You should call this before doing `save_pretrained` so that the `model.state_dict` is
+        fully compatible with `transformers.T5ForConditionalGeneration`.
+        """
+        # T5ForConditionalGeneration has a deparallelize method, so make sure that the PipelineMixin one is used here.
+        PipelineMixin.deparallelize(self)
+
+        self.encoder.__class__ = T5Stack
+        self.encoder.embed_tokens = self.encoder.embed_tokens.module
+
+        for block in self.encoder.block:
+            block.__class__ = T5Block
+            block.layer[0].dropout = block.layer[0].dropout.module
+            with torch.no_grad():
+                block.layer[1].DenseReluDense.wo.weight *= block.layer[1].dropout.scale
+            block.layer[1].dropout = block.layer[1].dropout.module
+            if self.config.dense_act_fn == "gelu_new":
+                block.layer[1].DenseReluDense.act = NewGELUActivation()
+
+        return self
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/vit/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/vit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/vit/modeling_vit.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/vit/modeling_vit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2021 The HuggingFace Team. All rights reserved.
 # Copyright (c) 2021 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -10,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import poptorch
 import transformers
+
 from optimum.utils import logging
 
 from ...modeling_utils import PipelineMixin, get_layer_ipu, recomputation_checkpoint, register
 
 
 logger = logging.get_logger(__name__)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# flake8: noqa
-# There's no way to ignore "F401 '...' imported but unused" warnings in this
-# module, but to preserve other warnings. So, don't check this module at all.
-
-# Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .modeling_wav2vec2 import PipelinedWav2Vec2ForCTC, PipelinedWav2Vec2ForPreTraining
+from diffusers import StableDiffusionPipeline
+
+from .pipeline_stable_diffusion_mixin import IPUStableDiffusionPipelineMixin
+
+
+class IPUStableDiffusionPipeline(IPUStableDiffusionPipelineMixin, StableDiffusionPipeline):
+    pass
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2021 The Fairseq Authors and the HuggingFace Inc. team. All rights reserved.
 # Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -23,15 +24,14 @@
   with a matrix multiplication (einsum), to allow for a more efficient memory
   usage on IPU.
 """
 
 import warnings
 
 import torch
-
 from transformers.models.wav2vec2.modeling_wav2vec2 import Wav2Vec2GumbelVectorQuantizer
 
 
 def _ipu_gumbel_softmax(logits, tau=1, hard=False, eps=1e-10, dim=-1):
     if eps != 1e-10:
         warnings.warn("`eps` parameter is deprecated and has no effect.")
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/ipu_layer_drop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2021 The Fairseq Authors and the HuggingFace Inc. team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,16 +16,14 @@
 
 """
 These are the same blocks as in the original implementation in transformers,
 but with a traceable implementation of LayerDrop.
 """
 
 import torch
-from torch.nn import functional as F
-
 from transformers.modeling_outputs import BaseModelOutput
 from transformers.models.wav2vec2.modeling_wav2vec2 import (
     Wav2Vec2Adapter,
     Wav2Vec2Encoder,
     Wav2Vec2EncoderStableLayerNorm,
 )
 
@@ -62,15 +61,15 @@
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_outputs = layer(hidden_states, attention_mask=attention_mask, output_attentions=output_attentions)
 
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
             # Modify LayerDrop so it can be statically compiled without eager mode
             if self.config.layerdrop > 0.0:
-                dropout_probability = torch.rand(tuple(), device=hidden_states.device)
+                dropout_probability = torch.rand((), device=hidden_states.device)
                 skip_the_layer = (
                     torch.tensor(self.training, device=hidden_states.device)
                     & (dropout_probability < self.config.layerdrop)
                 ).to(dtype=hidden_states.dtype)
                 hidden_states = hidden_states * skip_the_layer + layer_outputs[0] * (1 - skip_the_layer)
             else:
                 hidden_states = layer_outputs[0]
@@ -125,15 +124,15 @@
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_outputs = layer(hidden_states, attention_mask=attention_mask, output_attentions=output_attentions)
 
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
             # Modify LayerDrop so it can be statically compiled without eager mode
             if self.config.layerdrop > 0.0:
-                dropout_probability = torch.rand(tuple(), device=hidden_states.device)
+                dropout_probability = torch.rand((), device=hidden_states.device)
                 skip_the_layer = (
                     torch.tensor(self.training, device=hidden_states.device)
                     & (dropout_probability < self.config.layerdrop)
                 ).to(dtype=hidden_states.dtype)
                 hidden_states = hidden_states * skip_the_layer + layer_outputs[0] * (1 - skip_the_layer)
             else:
                 hidden_states = layer_outputs[0]
@@ -165,15 +164,15 @@
             hidden_states = self.proj(hidden_states)
             hidden_states = self.proj_layer_norm(hidden_states)
 
         hidden_states = hidden_states.transpose(1, 2)
 
         for layer in self.layers:
             layer_output = layer(hidden_states)
-            layerdrop_prob = torch.rand(tuple(), device=hidden_states.device)
+            layerdrop_prob = torch.rand((), device=hidden_states.device)
             use_the_layer = ~(
                 torch.tensor(self.training, device=hidden_states.device) | (layerdrop_prob > self.layerdrop)
             )
             hidden_states = use_the_layer * layer_output + (1 - use_the_layer) * hidden_states
 
         hidden_states = hidden_states.transpose(1, 2)
         return hidden_states
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2021 The Fairseq Authors and the HuggingFace Inc. team. All rights reserved.
 # Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -11,30 +12,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
 import numpy as np
+import poptorch
 import torch
 import torch.nn.functional as F
-
-import poptorch
-from optimum.utils import logging
 from transformers import Wav2Vec2ForPreTraining, Wav2Vec2Model
 from transformers.modeling_outputs import CausalLMOutput
 from transformers.models.wav2vec2.modeling_wav2vec2 import (
     Wav2Vec2Adapter,
     Wav2Vec2Encoder,
     Wav2Vec2EncoderStableLayerNorm,
     Wav2Vec2ForCTC,
     Wav2Vec2ForPreTrainingOutput,
     Wav2Vec2GumbelVectorQuantizer,
 )
 
+from optimum.utils import logging
+
 from ...modeling_utils import PipelineMixin, get_layer_ipu, recomputation_checkpoint, register
 from .ipu_gumbel_vector_quantizer import IPUWav2Vec2GumbelVectorQuantizer
 from .ipu_layer_drop import IPUWav2Vec2Adapter, IPUWav2Vec2Encoder, IPUWav2Vec2EncoderStableLayerNorm
 
 
 logger = logging.get_logger(__name__)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/lxmert/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
 # Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .feature_extraction_whisper import WhisperFeatureExtractorTorch
-from .modeling_whisper import PipelinedWhisperForConditionalGeneration
-from .processing_whisper import WhisperProcessorTorch
+from .modeling_lxmert import PipelinedLxmertForQuestionAnswering
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/feature_extraction_whisper.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/feature_extraction_whisper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2022 The HuggingFace Inc. team.
 # Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -9,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
 import torch
-
 from transformers import WhisperFeatureExtractor
 
 
 class WhisperFeatureExtractorTorch(WhisperFeatureExtractor):
     """
     A more efficient version of the numpy based `WhisperFeatureExtractor` which simply replaces
     most of the upstream transformers `_np_extract_fbank_features` with torch ops.
@@ -32,15 +32,15 @@
 
     def _np_extract_fbank_features(self, waveform: np.array) -> np.ndarray:
         """
         Compute the log-Mel spectrogram of the provided audio. This is almost a copy of upstream,
         with np replaced by torch.
         """
         if not torch.is_tensor(self.mel_filters):
-            self.mel_filters = torch.from_numpy(self.mel_filters)
+            self.mel_filters = torch.from_numpy(self.mel_filters).to(torch.float32).T
 
         waveform = torch.from_numpy(waveform)
 
         window = torch.hann_window(self.n_fft)
 
         stft = torch.stft(waveform, self.n_fft, self.hop_length, window=window, return_complex=True)
         magnitudes = torch.abs(stft[:, :-1]) ** 2
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/modeling_whisper.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/modeling_whisper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2022 The OpenAI Authors and The HuggingFace Inc. team. All rights reserved.
 # Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -10,42 +11,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 from typing import Optional, Tuple
 
+import poptorch
 import torch
 from torch import nn
-
-import poptorch
-from optimum.utils import logging
-from transformers import WhisperConfig
+from transformers.modeling_outputs import BaseModelOutput
 from transformers.models.whisper.modeling_whisper import (
     WhisperAttention,
     WhisperDecoder,
+    WhisperEncoder,
     WhisperEncoderLayer,
     WhisperForConditionalGeneration,
     WhisperPositionalEmbedding,
 )
 
-from ...generation import IPUAttentionMixin, IPUGenerationMixin, supports_kv_cache
+from optimum.utils import logging
+
+from ...generation import IPUAttentionMixin, IPUGenerationMixin, assert_poptorch_supports_cond, supports_kv_cache
 from ...modeling_utils import (
     PipelineMixin,
+    SerializedLinear,
     get_layer_ipu,
     recomputation_checkpoint,
     register,
     split_encoder_decoder_ipu_config,
 )
 
 
 logger = logging.get_logger(__name__)
 
-from transformers.activations import ACT2FN
-
 
 FLOAT16_LIMIT = 1e4
 
 
 # Copied from transformers.models.bart.modeling_bart._make_causal_mask
 def _make_causal_mask(input_ids_shape: torch.Size, dtype: torch.dtype, past_key_values_length: int = 0):
     """
@@ -87,17 +88,25 @@
         layer_head_mask: Optional[torch.Tensor] = None,
         output_attentions: bool = False,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
         bsz, tgt_len, _ = hidden_states.size()
 
         query_states = self.q_proj(hidden_states) * self.scaling
         if key_value_states is not None:
-            # cross attention
-            key_states = self._shape(self.k_proj(key_value_states), -1, bsz)
-            value_states = self._shape(self.v_proj(key_value_states), -1, bsz)
+            if self.cross_kv_cache_initialized:
+                # cross attention with cross kv cache
+                key_states, value_states = self.add_to_cross_kv_cache(
+                    key_value_states,
+                    lambda x: self._shape(self.k_proj(x), -1, bsz),
+                    lambda x: self._shape(self.v_proj(x), -1, bsz),
+                )
+            else:
+                # cross attention
+                key_states = self._shape(self.k_proj(key_value_states), -1, bsz)
+                value_states = self._shape(self.v_proj(key_value_states), -1, bsz)
         elif self.kv_cache_initialized:
             # self attention with kv cache
             key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
             value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
 
             if tgt_len != 1:
                 raise ValueError(f"KV cache expects tgt_len = 1, received {tgt_len}.")
@@ -112,16 +121,16 @@
         if self.is_decoder:
             # We handle the KV cache via buffers, not via the eager approach of passing the cache around.
             # This is retained so upstream DecoderLayer can stay as is and that tests pass.
             past_key_value = (key_states, value_states)
 
         proj_shape = (bsz * self.num_heads, -1, self.head_dim)
         query_states = self._shape(query_states, tgt_len, bsz).view(*proj_shape)
-        key_states = key_states.view(*proj_shape)
-        value_states = value_states.view(*proj_shape)
+        key_states = key_states.reshape(*proj_shape)
+        value_states = value_states.reshape(*proj_shape)
 
         src_len = key_states.size(1)
 
         # Change: optionally serialize attention, mainly intended for the encoder with large sequence length.
         if self.is_attention_serialized:
             if layer_head_mask is not None:
                 raise ValueError("layer_head_mask is not supported yet with serialized attention.")
@@ -189,40 +198,24 @@
         if not output_attentions:
             attn_weights = None
 
         return attn_output, attn_weights, past_key_value
 
 
 class _WhisperEncoderLayerClamp(nn.Module):
-    def __init__(self, config: WhisperConfig):
-        super().__init__()
-        self.embed_dim = config.d_model
-        self.self_attn = WhisperAttention(
-            embed_dim=self.embed_dim,
-            num_heads=config.encoder_attention_heads,
-            dropout=config.attention_dropout,
-        )
-        self.self_attn_layer_norm = nn.LayerNorm(self.embed_dim)
-        self.dropout = config.dropout
-        self.activation_fn = ACT2FN[config.activation_function]
-        self.activation_dropout = config.activation_dropout
-        self.fc1 = nn.Linear(self.embed_dim, config.encoder_ffn_dim)
-        self.fc2 = nn.Linear(config.encoder_ffn_dim, self.embed_dim)
-        self.final_layer_norm = nn.LayerNorm(self.embed_dim)
-
     def forward(
         self,
         hidden_states: torch.Tensor,
         attention_mask: torch.Tensor,
         layer_head_mask: torch.Tensor,
         output_attentions: bool = False,
     ):
         """
         Args:
-            hidden_states (`torch.FloatTensor`): input to the layer of shape `(seq_len, batch, embed_dim)`
+            hidden_states (`torch.FloatTensor`): input to the layer of shape `(batch, seq_len, embed_dim)`
             attention_mask (`torch.FloatTensor`): attention mask of size
                 `(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
             layer_head_mask (`torch.FloatTensor`): mask for attention heads in a given layer of size
                 `(config.encoder_attention_heads,)`.
             output_attentions (`bool`, *optional*):
                 Whether or not to return the attentions tensors of all attention layers. See `attentions` under
                 returned tensors for more detail.
@@ -273,21 +266,20 @@
         del self._generation_step
 
         original = copy.deepcopy(self)
         original.__class__ = WhisperPositionalEmbedding
         return original
 
     def forward(self, input_ids: torch.Tensor, past_key_values_length: int = 0):
-        del past_key_values_length
-
         if input_ids.shape[-1] == 1:
             # KV cache enabled.
-            return poptorch.dynamic_slice(self.weight, 0, self._generation_step, 1, 1)
+            del past_key_values_length
+            return torch.index_select(self.weight, 0, self._generation_step)
         else:
-            return self.weight[: input_ids.shape[-1]]
+            return super().forward(input_ids, past_key_values_length=past_key_values_length)
 
 
 class _WhisperDecoderWithCustomMakeCausalAndExpandMask(WhisperDecoder):
     """
     Transformer decoder consisting of *config.decoder_layers* layers. Each layer is a [`WhisperDecoderLayer`]
 
     Args:
@@ -310,26 +302,105 @@
             combined_attention_mask = (
                 expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask + combined_attention_mask
             )
 
         return combined_attention_mask
 
 
+class IPUWhisperConditionalEncoder(WhisperEncoder):
+    @classmethod
+    def from_model(cls, model: WhisperEncoder, batch_size: int, num_beams: int):
+        clone = model
+        clone.__class__ = cls
+        clone.register_buffer(
+            "_encoder_last_hidden_state",
+            torch.zeros((batch_size, model.config.max_source_positions, model.config.d_model), dtype=model.dtype),
+            persistent=False,
+        )
+        clone.register_buffer("_generation_step", torch.tensor([0], dtype=torch.int32), persistent=False)
+        clone._batch_size = batch_size
+        clone._num_beams = num_beams
+        return clone
+
+    def to_model(self) -> WhisperEncoder:
+        del self._encoder_last_hidden_state
+        del self._generation_step
+        del self._batch_size
+        del self._num_beams
+
+        original = self
+        original.__class__ = WhisperEncoder
+        return original
+
+    def forward(
+        self,
+        input_features,
+        attention_mask=None,
+        head_mask=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+    ):
+        if attention_mask is not None or head_mask is not None or output_attentions or output_hidden_states:
+            raise ValueError(f"{self.__class__.__name__} only accepts `input_features`.")
+
+        def run_encoder(input_features):
+            encoder_output = WhisperEncoder.forward(self, input_features, return_dict=True)
+            return encoder_output.last_hidden_state
+
+        def skip_encoder(input_features):
+            return self._encoder_last_hidden_state
+
+        self._encoder_last_hidden_state.copy_(
+            poptorch.cond(self._generation_step == 0, run_encoder, [input_features], skip_encoder, [input_features])[0]
+        )
+        last_hidden_state = self._encoder_last_hidden_state
+        if self._num_beams > 1:
+            # Before being passed to the decoder, we must expand the encoder outputs when beam search is enabled
+            # as this would be done on host.
+            last_hidden_state = last_hidden_state.repeat_interleave(
+                self._num_beams, dim=0, output_size=self._batch_size * self._num_beams
+            )
+        return BaseModelOutput(last_hidden_state=last_hidden_state)
+
+
 @supports_kv_cache
 @register(WhisperForConditionalGeneration)
 class PipelinedWhisperForConditionalGeneration(WhisperForConditionalGeneration, PipelineMixin, IPUGenerationMixin):
     def change_encoder_layer_class(self, restore: bool):
         """Changes the encoder layer class to avoid the dynamic 'if'
 
         Args:
             restore: whether to restore the encoder layers to their original version or not.
         """
         for layer in self.model.encoder.layers:
             layer.__class__ = WhisperEncoderLayer if restore else _WhisperEncoderLayerClamp
 
+    def change_encoder_class(self, restore: bool, **kwargs):
+        """Changes the encoder class to run the encoder under a `poptorch.cond` op.
+
+        Args:
+            restore: whether to restore the encoder to its original version or not.
+        """
+        batch_size = kwargs.get("batch_size", 1)
+        num_beams = kwargs.get("num_beams", 1)
+        encoder = self.model.get_encoder()
+        if restore:
+            if isinstance(encoder, IPUWhisperConditionalEncoder):
+                self.model.encoder = encoder.to_model()
+        else:
+            if self.ipu_config.ipus_per_replica > 1:
+                raise ValueError(
+                    f"`{self.ipu_config.ipus_per_replica=}` should be 1 when placing encoder and decoder on the same IPU."
+                )
+            assert_poptorch_supports_cond(
+                context="Whisper encoder is being conditionally run on the same IPU as the decoder since `use_cond_encoder=True`."
+            )
+            self.model.encoder = IPUWhisperConditionalEncoder.from_model(encoder, batch_size, num_beams)
+
     def change_decoder_class(self, restore: bool):
         """Changes the decoder class to update the _prepare_decoder_attention_mask method.
 
         Args:
             restore: whether to restore the decoder to its original version or not.
         """
         self.model.decoder.__class__ = WhisperDecoder if restore else _WhisperDecoderWithCustomMakeCausalAndExpandMask
@@ -347,18 +418,20 @@
 
     def change_attention_class(self, restore=False, **kwargs):
         """Change the attention layers to support a KV cache.
 
         Args:
             restore: whether to restore the attention layers to their original version or not.
         """
-        use_cache = kwargs.get("use_cache", False)
         batch_size = kwargs.get("batch_size", 1)
-        max_length = kwargs.get("max_length", 448)
         num_beams = kwargs.get("num_beams", 1)
+        use_cache = kwargs.get("use_cache", False)
+        max_length = kwargs.get("max_length", 448)
+        use_cross_cache = kwargs.get("use_cross_cache", False)
+        encoder_max_length = kwargs.get("encoder_max_length", 1500)
         batch_serialization_factor = kwargs.get("batch_serialization_factor", 1)
         sequence_serialization_factor = kwargs.get("sequence_serialization_factor", 1)
 
         for encoder_layer in self.model.encoder.layers:
             if restore:
                 encoder_layer.self_attn = encoder_layer.self_attn.to_model(WhisperAttention)
                 continue
@@ -375,49 +448,90 @@
                 decoder_layer.self_attn = decoder_layer.self_attn.to_model(WhisperAttention)
                 decoder_layer.encoder_attn = decoder_layer.encoder_attn.to_model(WhisperAttention)
                 continue
 
             decoder_layer.self_attn = IPUWhisperAttention.from_model(
                 decoder_layer.self_attn,
                 use_cache=use_cache,
+                use_cross_cache=False,
                 batch_size=batch_size,
                 max_length=max_length,
                 num_beams=num_beams,
                 dtype=decoder_layer.self_attn.k_proj.weight.dtype,
             )
             decoder_layer.encoder_attn = IPUWhisperAttention.from_model(
                 decoder_layer.encoder_attn,
                 use_cache=False,
+                use_cross_cache=use_cross_cache,
+                batch_size=batch_size,
+                encoder_max_length=encoder_max_length,
+                num_beams=num_beams,
+                dtype=decoder_layer.encoder_attn.k_proj.weight.dtype,
+            )
+
+    def change_lm_head(self, restore: bool, use_cache: bool = None):
+        # Maybe use _IndexedInputLinear
+        self.change_lm_head_to_indexed_input_linear(restore or use_cache)
+        # Maybe use SerializedLinear
+        if restore:
+            lm_head = self.get_output_embeddings()
+            if isinstance(lm_head, SerializedLinear):
+                self.set_output_embeddings(lm_head.to_model())
+                self.tie_weights()
+        else:
+            projection_serialization_factor = max(
+                self.ipu_config._projection_serialization_factor or 1,
+                sum(self.ipu_config._serialized_projection_splits_per_ipu or [1]),
             )
+            if projection_serialization_factor > 1:
+                self.set_output_embeddings(
+                    SerializedLinear.from_model(self.get_output_embeddings(), projection_serialization_factor)
+                )
+                self.tie_weights()
 
-    def parallelize(self, for_generation=False, use_cache=False, **kwargs):
+    def parallelize(self, for_generation=False, use_cache=False, use_cross_cache=False, **kwargs):
         super().parallelize()
 
+        if use_cache:
+            kwargs = self._populate_parallelize_kwargs_with_generation_config(**kwargs)
+
+        self._use_cond_encoder = kwargs.get("use_cond_encoder", False)
+        self._use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
+        if self._use_cond_encoder and self._use_encoder_output_buffer:
+            raise ValueError(
+                "`use_cond_encoder=True` is incompatible with `use_encoder_output_buffer=True`, only set one to True."
+            )
+
         self.change_encoder_layer_class(restore=False)
         self.change_decoder_class(restore=False)
         self.change_decoder_positional_embedding(restore=False)
-        self.change_attention_class(restore=False, use_cache=use_cache and for_generation, **kwargs)
-        self.change_lm_head_to_indexed_input_linear(restore=use_cache or not for_generation)
-        self.use_encoder_output_buffer = kwargs.get("use_encoder_output_buffer", False)
+        self.change_attention_class(
+            restore=False,
+            use_cache=use_cache and for_generation,
+            use_cross_cache=use_cross_cache and for_generation,
+            **kwargs,
+        )
+        self.change_lm_head(restore=False, use_cache=use_cache or not for_generation)
+        self.change_encoder_class(restore=not self._use_cond_encoder, **kwargs)
         self.set_on_device_generation_steps(kwargs.get("on_device_generation_steps", 0))
 
         logger.info("---------- Device Allocation -----------")
         logger.info("conv1, conv2, embed_positions  --> IPU 0")
         self.model.encoder.conv1 = poptorch.BeginBlock(self.model.encoder.conv1, "Conv1", ipu_id=0)
         self.model.encoder.conv2 = poptorch.BeginBlock(self.model.encoder.conv2, "Conv2", ipu_id=0)
         self.model.encoder.embed_positions = poptorch.BeginBlock(
             self.model.encoder.embed_positions, "Embed Positions", ipu_id=0
         )
 
         num_encoder_layers = len(self.model.encoder.layers)
         num_decoder_layers = len(self.model.decoder.layers)
 
-        if for_generation:
-            # If running for text generation we split the IPU config into two configs
-            # because we run the encoder and decoder as separate Poplar executors.
+        if for_generation and not self._use_cond_encoder:
+            # If running for text generation (and the encoder and decoder are run as separate Poplar executors)
+            # we split the IPU config into two configs.
             ipu_configs = split_encoder_decoder_ipu_config(self.ipu_config, num_encoder_layers, num_decoder_layers)
             self.encoder_ipu_config, self.decoder_ipu_config = ipu_configs
             encoder_layer_ipu = get_layer_ipu(self.encoder_ipu_config, num_encoder_layers)
             decoder_layer_ipu = get_layer_ipu(self.decoder_ipu_config, num_decoder_layers)
         else:
             number_of_layers = num_encoder_layers + num_decoder_layers
             layer_ipu = get_layer_ipu(self.ipu_config, number_of_layers)
@@ -430,50 +544,82 @@
             self.model.encoder.layers[index] = poptorch.BeginBlock(layer, f"Encoder{index}", ipu_id=ipu)
             logger.info(f"Encoder {index:<2} --> IPU {ipu}")
 
         # we need to deal with the model.encoder.layer norm
         self.model.encoder.layer_norm = poptorch.BeginBlock(
             self.model.encoder.layer_norm, "Encoder Layer Norm", ipu_id=ipu
         )
-        logger.info(f"Encoder LN {index:<2} --> IPU {ipu}")
+        logger.info(f"Encoder LN --> IPU {ipu}")
+
+        decoder_embedding_ipu = decoder_layer_ipu[0]
+        if (serialized_projection_splits_per_ipu := self.ipu_config._serialized_projection_splits_per_ipu) is not None:
+            serialized_projection_ipus = [i for i, x in enumerate(serialized_projection_splits_per_ipu) if x]
+            if len(serialized_projection_ipus) > 1:
+                # This is because we are using SerializedLinear. All splits of a SerializedLinear layer must be on the
+                # same IPU. We are using SerializedLinear instead of SplitLinear because we must tie the weights, which
+                # cannot be done when using SplitLinear.
+                raise ValueError(
+                    "`serialized_projection_splits_per_ipu` must only have 1 non-zero element for Whisper."
+                )
+            decoder_embedding_ipu = serialized_projection_ipus[0]
+        self.model.decoder.embed_tokens = poptorch.BeginBlock(
+            self.model.decoder.embed_tokens, "Decoder Embedding", ipu_id=decoder_embedding_ipu
+        )
+        logger.info(f"Decoder Embedding  --> IPU {decoder_embedding_ipu}")
 
         for index, (layer, ipu) in enumerate(zip(self.model.decoder.layers, decoder_layer_ipu)):
             if self.ipu_config.recompute_checkpoint_every_layer and index != self.config.num_hidden_layers - 1:
                 self._hooks.append(recomputation_checkpoint(layer))
             self.model.decoder.layers[index] = poptorch.BeginBlock(layer, f"Decoder{index}", ipu_id=ipu)
             logger.info(f"Decoder {index:<2} --> IPU {ipu}")
 
         self.model.decoder.layer_norm = poptorch.BeginBlock(
             self.model.decoder.layer_norm, "Decoder Layer Norm", ipu_id=ipu
         )
 
-        logger.info(f"Head       --> IPU 0")
+        logger.info(f"Head       --> IPU {decoder_embedding_ipu}")
         logger.info("---------------------------------------")
-        self.proj_out = poptorch.BeginBlock(self.proj_out, "Output Projection", ipu_id=0)
+        self.proj_out = poptorch.BeginBlock(self.proj_out, "Output Projection", ipu_id=decoder_embedding_ipu)
         return self
 
     def deparallelize(self):
         super().deparallelize()
 
         self.change_encoder_layer_class(restore=True)
         self.change_decoder_class(restore=True)
         self.change_decoder_positional_embedding(restore=True)
         self.change_attention_class(restore=True)
-        self.change_lm_head_to_indexed_input_linear(restore=True)
+        self.change_lm_head(restore=True)
+        self.change_encoder_class(restore=True)
         self.set_on_device_generation_steps(0)
 
+        return self
+
     def prepare_inputs_for_generation(
-        self, decoder_input_ids, past=None, use_cache=None, encoder_outputs=None, attention_mask=None, **kwargs
+        self,
+        decoder_input_ids,
+        past_key_values=None,
+        use_cache=None,
+        encoder_outputs=None,
+        attention_mask=None,
+        **kwargs,
     ):
-        # We don't use `past` for KV caching, and rely on `use_cache` instead.
+        # We don't use `past_key_values` for KV caching, and rely on `use_cache` instead.
         beam_idx = None
         if use_cache:
             decoder_input_ids = decoder_input_ids[:, -1:]
             beam_idx = kwargs.get("beam_idx", torch.arange(decoder_input_ids.shape[0], dtype=torch.long))
 
-        return {
-            "encoder_outputs": encoder_outputs,
+        ret = {
             "past_key_values": None,
             "decoder_input_ids": decoder_input_ids,
             "decoder_attention_mask": None,
             "beam_idx": beam_idx,
         }
+        if self.cond_encoder_enabled:
+            input_features = kwargs.get("input_features", None)
+            if input_features is None:
+                raise ValueError("Missing `input_features` with `use_cond_encoder=True`.")
+            ret["input_features"] = input_features
+        else:
+            ret["encoder_outputs"] = encoder_outputs
+        return ret
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/models/whisper/processing_whisper.py` & `optimum-graphcore-0.7.0/optimum/graphcore/models/whisper/processing_whisper.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,59 @@
+# Copyright 2018 The HuggingFace Inc. team.
 # Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, List, Optional, Union
-
-import torch
+from typing import Any, Dict, List, Optional, Union
 
 import poptorch
+import torch
 import transformers.pipelines
-from optimum.graphcore.generation.utils import IPUGenerationMixin
-from optimum.graphcore.ipu_configuration import IncompatibleIPUConfigError, IPUConfig
-from optimum.graphcore.modeling_utils import to_pipelined
 from transformers import (
     AudioClassificationPipeline,
     AutoFeatureExtractor,
-    AutomaticSpeechRecognitionPipeline,
     AutoModelForAudioClassification,
     AutoModelForCausalLM,
     AutoModelForCTC,
     AutoModelForImageClassification,
     AutoModelForMaskedLM,
     AutoModelForQuestionAnswering,
     AutoModelForSeq2SeqLM,
     AutoModelForSequenceClassification,
+    AutoModelForSpeechSeq2Seq,
     AutoModelForTokenClassification,
     AutoTokenizer,
     ImageClassificationPipeline,
     Pipeline,
     PreTrainedTokenizer,
     QuestionAnsweringPipeline,
     TextClassificationPipeline,
     TextGenerationPipeline,
+    WhisperForConditionalGeneration,
 )
 from transformers.feature_extraction_utils import PreTrainedFeatureExtractor
 from transformers.modeling_utils import PreTrainedModel
 from transformers.pipelines import get_task
 from transformers.utils import HUGGINGFACE_CO_RESOLVE_ENDPOINT, logging
 
+from optimum.graphcore.generation.utils import MODELS_SUPPORTING_KV_CACHE, IPUGenerationMixin
+from optimum.graphcore.ipu_configuration import IncompatibleIPUConfigError, IPUConfig
+from optimum.graphcore.modeling_utils import to_pipelined
+
+from .automatic_speech_recognition import IPUAutomaticSpeechRecognitionPipeline
 from .fill_mask import IPUFillMaskPipeline
 from .text2text_generation import IPUSummarizationPipeline, IPUText2TextGenerationPipeline, IPUTranslationPipeline
 from .token_classification import IPUTokenClassificationPipeline
 from .zero_shot_classification import IPUZeroShotClassificationPipeline
 
 
 logger = logging.get_logger(__name__)
@@ -66,17 +69,16 @@
         "default": {
             "model": ("superb/hubert-base-superb-ks", "d7e0efe"),
             "ipu_config": "Graphcore/hubert-base-ipu",
         },
         "type": "audio",
     },
     "automatic-speech-recognition": {
-        "impl": AutomaticSpeechRecognitionPipeline,
-        # TODO: support AutoModelForSpeechSeq2Seq
-        "class": (AutoModelForCTC,),
+        "impl": IPUAutomaticSpeechRecognitionPipeline,
+        "class": (AutoModelForCTC, AutoModelForSpeechSeq2Seq),
         "default": {
             "model": ("facebook/wav2vec2-base-960h", "55bb623"),
             "ipu_config": "Graphcore/wav2vec2-ctc-base-ipu",
         },
         "type": "multimodal",
     },
     "fill-mask": {
@@ -181,15 +183,20 @@
             "model": ("roberta-large-mnli", "130fb28"),
             "ipu_config": "Graphcore/roberta-large-ipu",
             "max_length": 128,
         },
         "type": "text",
     },
 }
-SUPPORTED_GENERATION_TASKS = {"summarization", "text-generation", "text2text-generation", "translation"}
+SUPPORTED_GENERATION_TASKS = {
+    "summarization",
+    "text-generation",
+    "text2text-generation",
+    "translation",
+}
 SUPPORTED_SEQ2SEQ_GENERATION_TASKS = {"summarization", "text2text-generation", "translation"}
 
 NO_FEATURE_EXTRACTOR_TASKS = set()
 NO_TOKENIZER_TASKS = set()
 for task, values in SUPPORTED_TASKS.items():
     if values["type"] == "text":
         NO_FEATURE_EXTRACTOR_TASKS.add(task)
@@ -205,14 +212,16 @@
 
 
 def get_poplar_executor(
     task: str,
     model: PreTrainedModel,
     ipu_config: Union[IPUConfig, str, dict] = None,
     fp16: bool = True,
+    for_generation: bool = False,
+    **parallelize_kwargs,
 ) -> PreTrainedModel:
     ipu_config_arg = ipu_config
 
     if isinstance(ipu_config, str):
         ipu_config = IPUConfig.from_pretrained(ipu_config)
     elif isinstance(ipu_config, dict):
         ipu_config = IPUConfig.from_dict(ipu_config)
@@ -220,22 +229,24 @@
         raise ValueError("ipu_config must be an IPUConfig, string, or a dictionary.")
 
     # So that IPUConfig returns inference versions of any parameters
     # that are different in training and inference
     ipu_config.eval()
 
     ipu_config.inference_device_iterations = 1
-    # TODO: inference_replication_factor should be adaptive, especially for batching.
-    ipu_config.inference_replication_factor = 1
+    if not parallelize_kwargs.get("use_cond_encoder", False):
+        ipu_config.inference_replication_factor = 1
     if not fp16:
         ipu_config.enable_half_partials = False
     try:
         model = to_pipelined(model, ipu_config, force=False)
         if model.config.is_encoder_decoder and isinstance(model, IPUGenerationMixin):
-            model.parallelize(for_generation=task in SUPPORTED_GENERATION_TASKS)
+            if "use_cache" not in parallelize_kwargs and model.__class__ in MODELS_SUPPORTING_KV_CACHE:
+                parallelize_kwargs["use_cache"] = True
+            model.parallelize(for_generation=for_generation, **parallelize_kwargs)
         else:
             model.parallelize()
     except Exception as error:
         new_message = (
             "The model and ipu_config seem to be incompatible,"
             " please try a different IPU config or customize it for the model."
             f" The config provided is '{ipu_config_arg}'\n"
@@ -244,15 +255,15 @@
         raise IncompatibleIPUConfigError(new_message) from error
     if fp16:
         model.half()
     opts = ipu_config.to_options(for_inference=True)
     opts.setExecutionStrategy(poptorch.ShardedExecution())
 
     # Text generation models have an internal Poplar executor so don't wrap model in that case
-    if task not in SUPPORTED_GENERATION_TASKS:
+    if not for_generation:
         model = poptorch.inferenceModel(model.eval(), opts)
     return model
 
 
 def check_model_type(self, supported_models: Union[List[str], dict]):
     """
     Check if the model class is supported by the pipeline.
@@ -276,29 +287,30 @@
     elif isinstance(self.model, IPUGenerationMixin):
         model_class_name = self.model.__class__.__bases__[0].__name__
     else:
         model_class_name = self.model.__class__.__name__
 
     if model_class_name not in supported_models:
         logger.error(
-            f"The model '{self.model._user_model.__class__.__bases__[0].__name__}' is not supported for {self.task}. Supported models are"
+            f"The model '{model_class_name}' is not supported for {self.task}. Supported models are"
             f" {supported_models}."
         )
 
 
 def pipeline(
     task: str = None,
     model: Optional[Any] = None,
     ipu_config: Union[IPUConfig, str, dict] = None,
     tokenizer: Optional[Union[str, PreTrainedTokenizer]] = None,
     feature_extractor: Optional[Union[str, PreTrainedFeatureExtractor]] = None,
     revision: Optional[str] = None,
     use_auth_token: Optional[Union[str, bool]] = None,
     pipeline_class: Optional[Any] = None,
     fp16: bool = True,
+    parallelize_kwargs: Optional[Dict[str, Any]] = None,
     **kwargs,
 ) -> Pipeline:
     """Utility factory method to build a [ Pipeline ] for IPU models.
 
     Arguments:
         task : The task, see docs for ``transformers.pipeline`` for supported options.
         model : A pre-trained model, see docs for ``transformers.pipeline`` for supported options.
@@ -342,39 +354,48 @@
     # These will never require a tokenizer.
     # the model on the other hand might have a tokenizer, but
     # the files could be missing from the hub, instead of failing
     # on such repos, we just force to not load it.
     load_tokenizer = targeted_task not in NO_TOKENIZER_TASKS
     load_feature_extractor = targeted_task not in NO_FEATURE_EXTRACTOR_TASKS
 
-    if pipeline_class is None:
-        pipeline_class = SUPPORTED_TASKS[targeted_task]["impl"]
-
-    if ipu_config is None and not isinstance(model, poptorch._poplar_executor.PoplarExecutor):
-        ipu_config = SUPPORTED_TASKS[targeted_task]["default"]["ipu_config"]
-
     if model is None:
         model_id, revision = SUPPORTED_TASKS[targeted_task]["default"]["model"]
         logger.warning(
             f"No model was supplied, defaulted to {model_id} and revision"
             f" {revision} ({HUGGINGFACE_CO_RESOLVE_ENDPOINT}/{model_id}).\n"
             "Using a pipeline without specifying a model name and revision in production is not recommended."
         )
         model = SUPPORTED_TASKS[targeted_task]["class"][0].from_pretrained(model_id, revision=revision)
-        model = get_poplar_executor(targeted_task, model, ipu_config, fp16)
     elif isinstance(model, str):
         model_id = model
-        model = SUPPORTED_TASKS[targeted_task]["class"][0].from_pretrained(model_id, revision=revision)
-        model = get_poplar_executor(targeted_task, model, ipu_config, fp16)
+        for cl in SUPPORTED_TASKS[targeted_task]["class"]:
+            try:
+                model = cl.from_pretrained(model_id, revision=revision)
+                break
+            except ValueError:
+                continue
     elif isinstance(model, PreTrainedModel):
-        model = get_poplar_executor(targeted_task, model, ipu_config, fp16)
         if tokenizer is None and load_tokenizer:
             raise ValueError("If you pass a model as a PreTrainedModel, you must pass a tokenizer as well")
         if feature_extractor is None and load_feature_extractor:
             raise ValueError("If you pass a model as a PreTrainedModel, you must pass a feature extractor as well")
+
+    for_generation = targeted_task in SUPPORTED_GENERATION_TASKS
+    if isinstance(model, PreTrainedModel):
+        if ipu_config is None:
+            ipu_config = SUPPORTED_TASKS[targeted_task]["default"]["ipu_config"]
+
+        parallelize_kwargs = parallelize_kwargs or {}
+        # Task of automatic speech recognition is a bit of an edge case where it separates into CTC (not generation) and seq2seq (generation).
+        # This check will do for now.
+        for_generation |= isinstance(model, WhisperForConditionalGeneration)
+        model = get_poplar_executor(
+            targeted_task, model, ipu_config=ipu_config, fp16=fp16, for_generation=for_generation, **parallelize_kwargs
+        )
     elif isinstance(model, poptorch._poplar_executor.PoplarExecutor):
         if tokenizer is None and load_tokenizer:
             raise ValueError(
                 "If you pass a model as a poptorch._poplar_executor.PoplarExecutor, you must pass a tokenizer as well"
             )
         if feature_extractor is None and load_feature_extractor:
             raise ValueError(
@@ -393,19 +414,22 @@
 
     if feature_extractor is None and load_feature_extractor:
         feature_extractor = AutoFeatureExtractor.from_pretrained(model_id)
 
     # Override Pipeline methods
     Pipeline.check_model_type = check_model_type
 
+    if pipeline_class is None:
+        pipeline_class = SUPPORTED_TASKS[targeted_task]["impl"]
+
     # Override pipelines' _forward
     old_forward = pipeline_class._forward
 
     def new_forward(self, model_inputs, *args, **kwargs):
-        if isinstance(self.model, poptorch.PoplarExecutor) and targeted_task not in SUPPORTED_GENERATION_TASKS:
+        if isinstance(self.model, poptorch.PoplarExecutor) and not for_generation:
             # For non-text generation models, support batch size changes.
             poplar_executor = self.model
             if poplar_executor._executable_inputs:
                 for arg in poplar_executor._executable_inputs.args:
                     if isinstance(arg, torch.Tensor):
                         compiled_bs = arg.shape[0]
                         break
@@ -435,15 +459,15 @@
             self.model.poptorch_encoder.destroy()
 
     pipeline_class.__del__ = _del
 
     # Auto padding for some tasks
     if "max_length" in SUPPORTED_TASKS[targeted_task]["default"]:
         default_max_length = SUPPORTED_TASKS[targeted_task]["default"]["max_length"]
-        if targeted_task not in SUPPORTED_GENERATION_TASKS:
+        if not for_generation:
             kwargs["padding"] = kwargs.get("padding", "max_length")
             if kwargs.get("max_length") is None:
                 logger.warning(
                     f"No padding arguments specified, so padding to {default_max_length} by default. "
                     f"Inputs longer than {default_max_length} will be truncated."
                     " To change this behaviour, pass the `padding='max_length'` and"
                     "`max_length=<your desired input length>` arguments to the pipeline function."
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/pipelines/zero_shot_classification.py` & `optimum-graphcore-0.7.0/optimum/graphcore/pipelines/text2text_generation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,93 @@
-from typing import List, Union
-
-import numpy as np
-
-from transformers import ZeroShotClassificationPipeline
-from transformers.pipelines.base import PIPELINE_INIT_ARGS, ArgumentHandler, ChunkPipeline
-from transformers.tokenization_utils import TruncationStrategy
-from transformers.utils import add_end_docstrings, logging
+# Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from transformers import SummarizationPipeline, Text2TextGenerationPipeline, TranslationPipeline
+from transformers.pipelines.text2text_generation import TruncationStrategy
+
+
+class IPUText2TextGenerationPipeline(Text2TextGenerationPipeline):
+    def _sanitize_parameters(
+        self,
+        return_tensors=None,
+        return_text=None,
+        return_type=None,
+        clean_up_tokenization_spaces=None,
+        truncation=None,
+        stop_sequence=None,
+        max_input_length=None,
+        **generate_kwargs,
+    ):
+        preprocess_params, forward_params, postprocess_params = super()._sanitize_parameters(
+            return_tensors,
+            return_text,
+            return_type,
+            clean_up_tokenization_spaces,
+            truncation,
+            stop_sequence,
+            **generate_kwargs,
+        )
+        if max_input_length is not None:
+            preprocess_params["max_input_length"] = max_input_length
+        return preprocess_params, forward_params, postprocess_params
+
+    def _parse_and_tokenize(self, *args, truncation, **kwargs):
+        prefix = self.model.config.prefix if self.model.config.prefix is not None else ""
+        if isinstance(args[0], list):
+            if self.tokenizer.pad_token_id is None:
+                raise ValueError("Please make sure that the tokenizer has a pad_token_id when using a batch input")
+            args = ([prefix + arg for arg in args[0]],)
+            padding = True
+
+        elif isinstance(args[0], str):
+            args = (prefix + args[0],)
+            padding = False
+        else:
+            raise ValueError(
+                f" `args[0]`: {args[0]} have the wrong format. The should be either of type `str` or type `list`"
+            )
+        padding = "max_length"
+        inputs = self.tokenizer(
+            *args,
+            padding=padding,
+            max_length=kwargs.get("max_input_length"),
+            truncation=truncation,
+            return_tensors=self.framework,
+        )
+        # This is produced by tokenizers but is an invalid generate kwargs
+        if "token_type_ids" in inputs:
+            del inputs["token_type_ids"]
+        return inputs
 
 
-logger = logging.get_logger(__name__)
+class IPUSummarizationPipeline(SummarizationPipeline, IPUText2TextGenerationPipeline):
+    pass
 
 
-@add_end_docstrings(PIPELINE_INIT_ARGS)
-class IPUZeroShotClassificationPipeline(ZeroShotClassificationPipeline):
-    def _parse_and_tokenize(
-        self, sequence_pairs, padding=True, add_special_tokens=True, truncation=TruncationStrategy.ONLY_FIRST, **kwargs
+class IPUTranslationPipeline(TranslationPipeline, IPUText2TextGenerationPipeline):
+    def preprocess(
+        self, *args, truncation=TruncationStrategy.DO_NOT_TRUNCATE, src_lang=None, tgt_lang=None, max_input_length=None
     ):
-        """
-        Parse arguments and tokenize only_first so that hypothesis (label) is not truncated
-        """
-        return_tensors = self.framework
-        if self.tokenizer.pad_token is None:
-            # Override for tokenizers not supporting padding
-            logger.error(
-                "Tokenizer was not supporting padding necessary for zero-shot, attempting to use "
-                " `pad_token=eos_token`"
-            )
-            self.tokenizer.pad_token = self.tokenizer.eos_token
-        try:
-            inputs = self.tokenizer(
-                sequence_pairs,
-                add_special_tokens=add_special_tokens,
-                return_tensors=return_tensors,
-                padding=padding,
+        if getattr(self.tokenizer, "_build_translation_inputs", None):
+            return self.tokenizer._build_translation_inputs(
+                *args,
+                return_tensors=self.framework,
+                max_length=max_input_length,
+                padding="max_length",
                 truncation=truncation,
-                **kwargs,
-            )
-        except Exception as e:
-            if "too short" in str(e):
-                # tokenizers might yell that we want to truncate
-                # to a value that is not even reached by the input.
-                # In that case we don't want to truncate.
-                # It seems there's not a really better way to catch that
-                # exception.
-
-                inputs = self.tokenizer(
-                    sequence_pairs,
-                    add_special_tokens=add_special_tokens,
-                    return_tensors=return_tensors,
-                    padding=padding,
-                    truncation=TruncationStrategy.DO_NOT_TRUNCATE,
-                )
-            else:
-                raise e
-
-        return inputs
-
-    def _sanitize_parameters(self, **kwargs):
-        if kwargs.get("multi_class", None) is not None:
-            kwargs["multi_label"] = kwargs["multi_class"]
-            logger.warning(
-                "The `multi_class` argument has been deprecated and renamed to `multi_label`. "
-                "`multi_class` will be removed in a future version of Transformers."
+                src_lang=src_lang,
+                tgt_lang=tgt_lang,
             )
-        preprocess_params = {}
-        if "candidate_labels" in kwargs:
-            preprocess_params["candidate_labels"] = self._args_parser._parse_labels(kwargs["candidate_labels"])
-        if "hypothesis_template" in kwargs:
-            preprocess_params["hypothesis_template"] = kwargs["hypothesis_template"]
-        if "padding" in kwargs:
-            preprocess_params["padding"] = kwargs["padding"]
-        if "max_length" in kwargs:
-            preprocess_params["max_length"] = kwargs["max_length"]
-
-        postprocess_params = {}
-        if "multi_label" in kwargs:
-            postprocess_params["multi_label"] = kwargs["multi_label"]
-        return preprocess_params, {}, postprocess_params
-
-    def preprocess(self, inputs, candidate_labels=None, hypothesis_template="This example is {}.", **tokenizer_kwargs):
-        sequence_pairs, sequences = self._args_parser(inputs, candidate_labels, hypothesis_template)
-
-        for i, (candidate_label, sequence_pair) in enumerate(zip(candidate_labels, sequence_pairs)):
-            model_input = self._parse_and_tokenize([sequence_pair], **tokenizer_kwargs)
-
-            yield {
-                "candidate_label": candidate_label,
-                "sequence": sequences[0],
-                "is_last": i == len(candidate_labels) - 1,
-                **model_input,
-            }
+        else:
+            return super()._parse_and_tokenize(*args, truncation=truncation, max_input_length=max_input_length)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/trainer.py` & `optimum-graphcore-0.7.0/optimum/graphcore/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#  copyright 2021 the huggingface team. all rights reserved.
+#  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
-#  licensed under the apache license, version 2.0 (the "license");
-#  you may not use this file except in compliance with the license.
-#  you may obtain a copy of the license at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/license-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-#  unless required by applicable law or agreed to in writing, software
-#  distributed under the license is distributed on an "as is" basis,
-#  without warranties or conditions of any kind, either express or implied.
-#  see the license for the specific language governing permissions and
-#  limitations under the license.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import collections
 import copy
 import functools
 import inspect
 import math
 import os
@@ -24,38 +25,34 @@
 import sys
 import time
 import warnings
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
-from tqdm.auto import tqdm
-
-
 # Integrations must be imported before ML frameworks:
-from transformers.integrations import (  # isort: split
-    get_reporting_integration_callbacks,
-)
-
 import numpy as np
-import torch
-from packaging import version
-from torch import nn, optim
-from torch.utils.data import Dataset, RandomSampler, SequentialSampler, SubsetRandomSampler
-from torch.utils.data.distributed import DistributedSampler
-
 import poptorch
+import torch
 from huggingface_hub import Repository
-from optimum.graphcore.version import __version__
-from optimum.utils import logging
+from packaging import version
 from poptorch import DataLoaderMode, PoplarExecutor
 from poptorch.optim import LAMB, AdamW
+from torch import nn, optim
+from torch.utils.data import Dataset, RandomSampler, SequentialSampler
+from torch.utils.data.distributed import DistributedSampler
+from tqdm.auto import tqdm
 from transformers.configuration_utils import PretrainedConfig
 from transformers.data.data_collator import DataCollator, DataCollatorWithPadding, default_data_collator
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
+
+
+from transformers.integrations import (  # isort: split
+    get_reporting_integration_callbacks,
+)
 from transformers.modeling_utils import PreTrainedModel
 from transformers.optimization import get_scheduler
 from transformers.pytorch_utils import is_torch_less_than_1_11
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer import OPTIMIZER_NAME, SCHEDULER_NAME, TRAINER_STATE_NAME, TRAINING_ARGS_NAME
 from transformers.trainer_callback import (
     CallbackHandler,
@@ -99,14 +96,17 @@
     WEIGHTS_INDEX_NAME,
     WEIGHTS_NAME,
     find_labels,
     get_full_repo_name,
     is_datasets_available,
 )
 
+from optimum.graphcore.version import __version__
+from optimum.utils import logging
+
 from .data.data_collator import pad_on_batch_axis
 from .ipu_configuration import IPU_CONFIG_NAME, IPUConfig
 from .modelcard import IPUTrainingSummary
 from .modeling_utils import to_pipelined
 from .trainer_utils import _WorkerInit
 from .training_args import IPUTrainingArguments
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/trainer_pt_utils.py` & `optimum-graphcore-0.7.0/optimum/graphcore/trainer_pt_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/trainer_seq2seq.py` & `optimum-graphcore-0.7.0/optimum/graphcore/trainer_seq2seq.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,129 @@
 # Copyright 2022 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import inspect
+from copy import deepcopy
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
+from poptorch._impl import rewrapModelIfNecessary, unwrapModelIfNecessary
 from torch import nn
 from torch.utils.data import Dataset
+from transformers.generation.configuration_utils import GenerationConfig
 
 from optimum.utils import logging
-from poptorch._impl import rewrapModelIfNecessary, unwrapModelIfNecessary
 
-from .trainer import IPUTrainer
+from .trainer import IPUConfig, IPUTrainer, IPUTrainingArguments
+
+
+if TYPE_CHECKING:
+    from transformers.data.data_collator import DataCollator
+    from transformers.modeling_utils import PreTrainedModel
+    from transformers.tokenization_utils_base import PreTrainedTokenizerBase
+    from transformers.trainer_callback import TrainerCallback
+    from transformers.trainer_utils import EvalPrediction, PredictionOutput
 
 
 logger = logging.get_logger(__name__)
 
 
 class IPUSeq2SeqTrainer(IPUTrainer):
     """
     The [`IPUSeq2SeqTrainer`] class is used to train seq2seq models. Its behaviour is exactly the same as [`IPUTrainer`] except that it expects [`IPUSeq2SeqTrainingArguments`] instead of [`IPUTrainingArguments`].
     """
 
+    def __init__(
+        self,
+        model: Union["PreTrainedModel", nn.Module] = None,
+        ipu_config: IPUConfig = None,
+        args: "IPUTrainingArguments" = None,
+        data_collator: Optional["DataCollator"] = None,
+        eval_data_collator: Optional["DataCollator"] = None,
+        train_dataset: Optional[Dataset] = None,
+        eval_dataset: Optional[Dataset] = None,
+        tokenizer: Optional["PreTrainedTokenizerBase"] = None,
+        model_init: Callable[[], "PreTrainedModel"] = None,
+        compute_metrics: Optional[Callable[["EvalPrediction"], Dict]] = None,
+        callbacks: Optional[List["TrainerCallback"]] = None,
+        optimizers: Tuple[torch.optim.Optimizer, torch.optim.lr_scheduler.LambdaLR] = (None, None),
+        preprocess_logits_for_metrics: Optional[Callable[[torch.Tensor, torch.Tensor], torch.Tensor]] = None,
+        force_to_pipelined: bool = False,
+    ):
+        super().__init__(
+            model=model,
+            ipu_config=ipu_config,
+            args=args,
+            data_collator=data_collator,
+            eval_data_collator=eval_data_collator,
+            train_dataset=train_dataset,
+            eval_dataset=eval_dataset,
+            tokenizer=tokenizer,
+            model_init=model_init,
+            compute_metrics=compute_metrics,
+            callbacks=callbacks,
+            optimizers=optimizers,
+            preprocess_logits_for_metrics=preprocess_logits_for_metrics,
+            force_to_pipelined=force_to_pipelined,
+        )
+
+        # Override self.model.generation_config if a GenerationConfig is specified in args.
+        # Priority: args.generation_config > model.generation_config > default GenerationConfig.
+        if self.args.generation_config is not None:
+            gen_config = self.load_generation_config(self.args.generation_config)
+            self.model.generation_config = gen_config
+
+    @staticmethod
+    def load_generation_config(gen_config_arg: Union[str, GenerationConfig]) -> GenerationConfig:
+        """
+        Loads a `~generation.GenerationConfig` from the `Seq2SeqTrainingArguments.generation_config` arguments.
+
+        Args:
+            gen_config_arg (`str` or [`~generation.GenerationConfig`]):
+                `Seq2SeqTrainingArguments.generation_config` argument.
+
+        Returns:
+            A `~generation.GenerationConfig`.
+        """
+
+        # GenerationConfig provided, nothing to do
+        if isinstance(gen_config_arg, GenerationConfig):
+            return deepcopy(gen_config_arg)
+
+        # str or Path
+        pretrained_model_name = Path(gen_config_arg) if isinstance(gen_config_arg, str) else gen_config_arg
+        config_file_name = None
+
+        # Figuring if it is path pointing to a file, pointing to a directory or else a model id or URL
+        # This step is required in order to determine config_file_name
+        if pretrained_model_name.is_file():
+            config_file_name = pretrained_model_name.name
+            pretrained_model_name = pretrained_model_name.parent
+        # dir path
+        elif pretrained_model_name.is_dir():
+            pass
+        # model id or URL
+        else:
+            pretrained_model_name = gen_config_arg
+
+        gen_config = GenerationConfig.from_pretrained(pretrained_model_name, config_file_name)
+        return gen_config
+
     def _wrap_and_compile_model_for_evaluation(self, dataloader, prediction_loss_only):
         if prediction_loss_only:
             return super()._wrap_and_compile_model_for_evaluation(dataloader, prediction_loss_only)
 
         # Unwrap the model, including parameter and buffer annotations and the
         # model as a whole. This is needed to avoid issues with persistent buffers
         # when compiling an inference model for generation
@@ -59,16 +146,15 @@
         rewrapModelIfNecessary(self.model)
 
     def evaluate(
         self,
         eval_dataset: Optional[Dataset] = None,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "eval",
-        max_length: Optional[int] = None,
-        num_beams: Optional[int] = None,
+        **gen_kwargs,
     ) -> Dict[str, float]:
         """
         Run evaluation and returns metrics.
 
         The calling script will be responsible for providing a method to compute metrics, as they are task-dependent
         (pass it to the init `compute_metrics` argument).
 
@@ -86,32 +172,38 @@
                 An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
                 "eval_bleu" if the prefix is `"eval"` (default)
             max_length (`int`, *optional*):
                 The maximum target length to use when predicting with the generate method.
             num_beams (`int`, *optional*):
                 Number of beams for the beam search that will be used when predicting with the generate method. 1 means no
                 beam search.
+            gen_kwargs:
+                Additional `generate` specific kwargs.
 
         Returns:
             A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
             dictionary also contains the epoch number which comes from the training state.
         """
-        self._max_length = max_length if max_length is not None else self.args.generation_max_length
-        self._num_beams = num_beams if num_beams is not None else self.args.generation_num_beams
+        gen_kwargs = gen_kwargs.copy()
+        if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
+            gen_kwargs["max_length"] = self.args.generation_max_length
+        gen_kwargs["num_beams"] = (
+            gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.args.generation_num_beams
+        )
+        self._gen_kwargs = gen_kwargs
         results = super().evaluate(eval_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
         self._rewrap_model_for_training()
         return results
 
     def predict(
         self,
         test_dataset: Dataset,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "test",
-        max_length: Optional[int] = None,
-        num_beams: Optional[int] = None,
+        **gen_kwargs,
     ) -> "PredictionOutput":
         """
         Runs prediction and returns predictions and potential metrics.
 
         Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
         will also return metrics, like `evaluate()`.
 
@@ -126,14 +218,16 @@
                 An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
                 "eval_bleu" if the prefix is `"eval"` (default)
             max_length (`int`, *optional*):
                 The maximum target length to use when predicting with the generate method.
             num_beams (`int`, *optional*):
                 Number of beams for the beam search that will be used when predicting with the generate method. 1 means no
                 beam search.
+            gen_kwargs:
+                Additional `generate` specific kwargs.
 
         <Tip>
 
         If your predictions or labels have different sequence lengths (for instance because you're doing dynamic
         padding in a token classification task) the predictions will be padded (on the right) to allow for
         concatenation into one array. The padding index is -100.
 
@@ -145,16 +239,21 @@
                 The predictions on `test_dataset`.
             - label_ids (`np.ndarray`, *optional*):
                 The labels (if the dataset contained some).
             - metrics (`Dict[str, float]`, *optional*):
                 The potential dictionary of metrics (if the dataset contained
                 labels).
         """
-        self._max_length = max_length if max_length is not None else self.args.generation_max_length
-        self._num_beams = num_beams if num_beams is not None else self.args.generation_num_beams
+        gen_kwargs = gen_kwargs.copy()
+        if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
+            gen_kwargs["max_length"] = self.args.generation_max_length
+        gen_kwargs["num_beams"] = (
+            gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.args.generation_num_beams
+        )
+        self._gen_kwargs = gen_kwargs
         results = super().predict(test_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
         self._rewrap_model_for_training()
         return results
 
     def prediction_step(
         self,
         model: nn.Module,
@@ -189,40 +288,52 @@
                 model,
                 inputs,
                 prediction_loss_only=prediction_loss_only,
                 ignore_keys=ignore_keys,
                 is_last_batch=is_last_batch,
             )
 
-        has_labels = "labels" in inputs
         inputs = self._prepare_inputs(inputs)
 
-        gen_kwargs = {
-            "max_length": self._max_length if self._max_length is not None else self.model.config.max_length,
-            # TODO: disabled beam search for now.
-            "num_beams": self._num_beams if self._num_beams is not None else self.model.config.num_beams,
-            "synced_gpus": False,
-        }
+        # Priority (handled in generate):
+        # gen_kwargs > model.generation_config > default GenerationConfig()
+        gen_kwargs = self._gen_kwargs.copy()
+        if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
+            gen_kwargs["max_length"] = self.model.config.max_length
+        gen_kwargs["num_beams"] = (
+            gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.model.config.num_beams
+        )
 
         # prepare generation inputs
         # some encoder-decoder models can have varying encoder's and thus
         # varying model input names
         if hasattr(self.model, "encoder") and self.model.encoder.main_input_name != self.model.main_input_name:
             generation_inputs = inputs[self.model.encoder.main_input_name]
         else:
             generation_inputs = inputs[self.model.main_input_name]
 
         generated_tokens = model.generate(
             generation_inputs,
             attention_mask=inputs.get("attention_mask", None),
             **gen_kwargs,
         )
+
+        # Temporary hack to ensure the generation config is not initialized for each iteration of the evaluation loop
+        # TODO: remove this hack when the legacy code that initializes generation_config from a model config is
+        # removed in https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/generation/utils.py#L1183
+        if self.model.generation_config._from_model_config:
+            self.model.generation_config._from_model_config = False
+
+        # Retrieves GenerationConfig from model.generation_config
+        gen_config = self.model.generation_config
         # in case the batch is shorter than max length, the output should be padded
-        if generated_tokens.shape[-1] < gen_kwargs["max_length"]:
-            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_length"])
+        if generated_tokens.shape[-1] < gen_config.max_length:
+            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_config.max_length)
+        elif gen_config.max_new_tokens is not None and generated_tokens.shape[-1] < gen_config.max_new_tokens + 1:
+            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_config.max_new_tokens + 1)
 
         # with torch.no_grad():
         #     # with self.autocast_smart_context_manager():
         #     outputs = model(**inputs)
         #     if has_labels:
         #         if self.label_smoother is not None:
         #             loss = self.label_smoother(outputs, inputs["labels"]).mean().detach()
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/trainer_utils.py` & `optimum-graphcore-0.7.0/optimum/graphcore/trainer_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-#  copyright 2021 the huggingface team. all rights reserved.
+#  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
-#  licensed under the apache license, version 2.0 (the "license");
-#  you may not use this file except in compliance with the license.
-#  you may obtain a copy of the license at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/license-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-#  unless required by applicable law or agreed to in writing, software
-#  distributed under the license is distributed on an "as is" basis,
-#  without warranties or conditions of any kind, either express or implied.
-#  see the license for the specific language governing permissions and
-#  limitations under the license.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import functools
 
 import numpy as np
+import poptorch
 import torch
 
 from optimum.utils import logging
 
 
 logger = logging.get_logger(__name__)
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/training_args.py` & `optimum-graphcore-0.7.0/optimum/graphcore/training_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright 2020 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,26 +17,26 @@
 import json
 import math
 import os
 import warnings
 from dataclasses import asdict, dataclass, field
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
 import torch
-
-from optimum.utils import logging
 from poptorch import DataLoaderMode
 from transformers.debug_utils import DebugOption
-from transformers.file_utils import cached_property, get_full_repo_name, is_torch_available, torch_required
+from transformers.file_utils import cached_property, get_full_repo_name, is_torch_available, requires_backends
 from transformers.trainer_utils import EvaluationStrategy, HubStrategy, IntervalStrategy, SchedulerType
 from transformers.training_args import default_logdir
 from transformers.utils import ExplicitEnum
 
+from optimum.utils import logging
+
 
 logger = logging.get_logger(__name__)
 log_levels = logging.get_log_levels_dict().copy()
 trainer_log_levels = dict(**log_levels, passive=-1)
 
 ALLOWED_N_IPU = [2**i for i in range(7)]
 
@@ -563,18 +564,14 @@
     push_to_hub_model_id: str = field(
         default=None, metadata={"help": "The name of the repository to which push `Trainer` to."}
     )
     push_to_hub_organization: str = field(
         default=None, metadata={"help": "The name of the organization to use when pushing `Trainer`."}
     )
     push_to_hub_token: str = field(default=None, metadata={"help": "The token to use to push to the Model Hub."})
-    pod_type: Optional[str] = field(
-        default=None,
-        metadata={"help": "The POD type to run the `Trainer` on."},
-    )
     # IPU Specific arguments
     ipu_config_name: Optional[str] = field(
         default=None, metadata={"help": "Pre-trained IPU config name or path if not the same as model_name."}
     )
     n_ipu: Optional[int] = field(
         default=None,
         metadata={"help": "The number of IPUs to run the `Trainer` on.", "choices": ALLOWED_N_IPU},
@@ -743,22 +740,14 @@
             warnings.warn(
                 "`--push_to_hub_organization` is deprecated and will be removed in version 5 of 🤗 Transformers. Use "
                 "`--hub_model_id` instead and pass the full repo name to this argument (in this case "
                 f"{self.hub_model_id}).",
                 FutureWarning,
             )
 
-        if self.pod_type is not None:
-            warnings.warn(
-                "`pod_type` is deprecated and will be removed in the next release of Optimum Graphcore. Use `n_ipu` "
-                "instead to specify how many IPUs you would like the Trainer to use.",
-                FutureWarning,
-            )
-            self.n_ipu = int(self.pod_type.strip("pod"))
-
         # IPU specific
         dataloader_mode_mapping = {"sync": 0, "async": 1, "async_rebatched": 2}
         self.dataloader_mode = DataLoaderMode(dataloader_mode_mapping[self.dataloader_mode])
 
         override_str = []
         if self.gradient_accumulation_steps is not None:
             override_str.append(f"gradient_accumulation_steps={self.gradient_accumulation_steps}")
@@ -775,28 +764,35 @@
             override_str = ",".join(override_str)
             if self.ipu_config_overrides is None:
                 self.ipu_config_overrides = override_str
             else:
                 self.ipu_config_overrides = ",".join([self.ipu_config_overrides, override_str])
 
     @cached_property
-    @torch_required
     def _setup_devices(self) -> "torch.device":
+        requires_backends(self, ["torch"])
         device = torch.device("cpu")
         return device
 
     @property
-    @torch_required
     def device(self) -> "torch.device":
         """
         The device used by this process.
         """
+        requires_backends(self, ["torch"])
         return self._setup_devices
 
     @property
+    def should_log(self):
+        """
+        Whether or not the current process should produce log.
+        """
+        return True
+
+    @property
     def should_save(self):
         """
         Returns whether the current process should write to disk or not, for example, to save models and checkpoints.
         """
         return True
 
     def get_process_log_level(self):
```

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/utils/__init__.py` & `optimum-graphcore-0.7.0/optimum/graphcore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-graphcore-0.6.1/optimum/graphcore/version.py` & `optimum-graphcore-0.7.0/optimum/graphcore/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #  Copyright 2021 The HuggingFace Team. All rights reserved.
+#  Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `optimum-graphcore-0.6.1/optimum_graphcore.egg-info/PKG-INFO` & `optimum-graphcore-0.7.0/optimum_graphcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-graphcore
-Version: 0.6.1
+Version: 0.7.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://huggingface.co/hardware
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,training,ipu
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `optimum-graphcore-0.6.1/optimum_graphcore.egg-info/SOURCES.txt` & `optimum-graphcore-0.7.0/optimum_graphcore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,28 @@
 optimum/graphcore/models/lxmert/__init__.py
 optimum/graphcore/models/lxmert/modeling_lxmert.py
 optimum/graphcore/models/mt5/__init__.py
 optimum/graphcore/models/mt5/modeling_mt5.py
 optimum/graphcore/models/roberta/__init__.py
 optimum/graphcore/models/roberta/modeling_roberta.py
 optimum/graphcore/models/t5/__init__.py
+optimum/graphcore/models/t5/configuration_t5.py
 optimum/graphcore/models/t5/modeling_t5.py
 optimum/graphcore/models/vit/__init__.py
 optimum/graphcore/models/vit/modeling_vit.py
 optimum/graphcore/models/wav2vec2/__init__.py
 optimum/graphcore/models/wav2vec2/ipu_gumbel_vector_quantizer.py
 optimum/graphcore/models/wav2vec2/ipu_layer_drop.py
 optimum/graphcore/models/wav2vec2/modeling_wav2vec2.py
 optimum/graphcore/models/whisper/__init__.py
 optimum/graphcore/models/whisper/feature_extraction_whisper.py
 optimum/graphcore/models/whisper/modeling_whisper.py
 optimum/graphcore/models/whisper/processing_whisper.py
 optimum/graphcore/pipelines/__init__.py
+optimum/graphcore/pipelines/automatic_speech_recognition.py
 optimum/graphcore/pipelines/fill_mask.py
 optimum/graphcore/pipelines/text2text_generation.py
 optimum/graphcore/pipelines/token_classification.py
 optimum/graphcore/pipelines/zero_shot_classification.py
 optimum/graphcore/utils/__init__.py
 optimum_graphcore.egg-info/PKG-INFO
 optimum_graphcore.egg-info/SOURCES.txt
@@ -87,8 +89,9 @@
 optimum_graphcore.egg-info/top_level.txt
 tests/test_examples.py
 tests/test_examples_match_transformers.py
 tests/test_ipu_configuration.py
 tests/test_modeling_common.py
 tests/test_modeling_utils.py
 tests/test_pipelined_models.py
-tests/test_trainer.py
+tests/test_trainer.py
+tests/test_trainer_seq2seq.py
```

### Comparing `optimum-graphcore-0.6.1/pyproject.toml` & `optimum-graphcore-0.7.0/optimum/graphcore/diffusers/pipelines/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-#  Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-[tool.black]
-line-length = 119
-target-version = ['py38']
+from .stable_diffusion import (
+    INFERENCE_ENGINES_TO_MODEL_NAMES,
+    IPUStableDiffusionImg2ImgPipeline,
+    IPUStableDiffusionInpaintPipeline,
+    IPUStableDiffusionPipeline,
+    get_default_ipu_configs,
+)
```

### Comparing `optimum-graphcore-0.6.1/setup.py` & `optimum-graphcore-0.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2021 The HuggingFace Team. All rights reserved.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import re
 
 from setuptools import find_namespace_packages, setup
 
 
 # Ensure we match the version set in optimum/version.py
 try:
@@ -9,28 +24,30 @@
     with open(filepath) as version_file:
         (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
-    "transformers==4.25.1",
+    "transformers==4.29.2",
     "optimum==1.6.1",
     "diffusers[torch]==0.12.1",
     "datasets",
     "tokenizers",
     "typeguard",
     "sentencepiece",
     "scipy",
     "pillow",
 ]
 
 QUALITY_REQUIRES = [
-    "black",
-    "isort",
+    "black~=23.1",
+    "isort>=5.5.4",
+    # "hf-doc-builder @ git+https://github.com/huggingface/doc-builder.git",
+    "ruff>=0.0.241,<=0.0.259",
 ]
 
 EXTRA_REQUIRE = {
     "testing": [
         "filelock",
         "GitPython",
         "parameterized",
```

### Comparing `optimum-graphcore-0.6.1/tests/test_examples.py` & `optimum-graphcore-0.7.0/tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2022 HuggingFace Inc.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,15 +21,14 @@
 import subprocess
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Callable, Dict, List, Optional, Tuple, Union
 from unittest import TestCase
 
 from filelock import FileLock
-from optimum.graphcore.modeling_utils import _PRETRAINED_TO_PIPELINED_REGISTRY
 from transformers import (
     CONFIG_MAPPING,
     MODEL_FOR_AUDIO_CLASSIFICATION_MAPPING,
     MODEL_FOR_CAUSAL_LM_MAPPING,
     MODEL_FOR_CTC_MAPPING,
     MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING,
     MODEL_FOR_MASKED_LM_MAPPING,
@@ -36,14 +36,16 @@
     MODEL_FOR_QUESTION_ANSWERING_MAPPING,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
 )
 from transformers.testing_utils import slow
 
+from optimum.graphcore.modeling_utils import _PRETRAINED_TO_PIPELINED_REGISTRY
+
 from .utils import MODELS_TO_TEST_MAPPING
 
 
 def _get_supported_models_for_script(
     models_to_test: Dict[str, Tuple[str]], task_mapping: Dict[str, str], task: str = "default"
 ) -> List[Tuple[str]]:
     """
@@ -386,32 +388,44 @@
         self.assertEqual(p.returncode, 0)
 
 
 class TextClassificationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_glue"):
     TASK_NAME = "sst2"
     DATASET_PARAMETER_NAME = "task_name"
     INFERENCE_DEVICE_ITERATIONS = 5
+    EXTRA_COMMAND_LINE_ARGUMENTS = [
+        "--loss_scaling 1024",
+    ]
 
 
 class TokenClassificationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_ner"):
     TASK_NAME = "conll2003"
     TRAIN_BATCH_SIZE = 1
     EVAL_BATCH_SIZE = 1
+    EXTRA_COMMAND_LINE_ARGUMENTS = [
+        "--preprocessing_num_workers 16",
+    ]
 
 
 class MultipleChoiceExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_swag"):
     # Using a small gradient accumulation steps value because input data is repated for the multiple choice task.
     TRAIN_BATCH_SIZE = 1
     EVAL_BATCH_SIZE = 1
     EVAL_SCORE_THRESHOLD_OVERRIDES = {"distilbert-base-uncased": 0.645, "Graphcore/groupbert-base-uncased": 0.66}
+    EXTRA_COMMAND_LINE_ARGUMENTS = [
+        "--preprocessing_num_workers 16",
+    ]
 
 
 class QuestionAnsweringExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_qa"):
     TASK_NAME = "squad"
     SCORE_NAME = "eval_f1"
+    EXTRA_COMMAND_LINE_ARGUMENTS = [
+        "--preprocessing_num_workers 16",
+    ]
 
 
 class SummarizationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_summarization"):
     TASK_NAME = "cnn_dailymail"
     DATASET_CONFIG = "3.0.0"
     TRAIN_BATCH_SIZE = 1
     EVAL_BATCH_SIZE = 1
@@ -421,14 +435,15 @@
     INFERENCE_DEVICE_ITERATIONS = 6
     EXTRA_COMMAND_LINE_ARGUMENTS = [
         "--dataset_config 3.0.0",
         "--prediction_loss_only",
         "--pad_to_max_length",
         "--max_target_length 200",
         "--max_source_length 1024",
+        "--preprocessing_num_workers 16",
     ]
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
         ipu_config_name: str,
@@ -478,14 +493,15 @@
         "--dataset_config ro-en",
         "--source_lang ro",
         "--target_lang en",
         "--pad_to_max_length",
         "--max_source_length 512",
         "--max_target_length 512",
         "--prediction_loss_only",
+        "--preprocessing_num_workers 16",
     ]
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
         ipu_config_name: str,
@@ -565,8 +581,9 @@
         "--mask_time_prob 0.0",
         "--layerdrop 0.0",
         "--weight_decay 0.005",
         "--freeze_feature_encoder",
         "--text_column_name sentence",
         "--length_column_name input_length",
         '--chars_to_ignore , ? . ! - \\; \\: \\" “ % ‘ ” � ',
+        "--preprocessing_num_workers 16",
     ]
```

### Comparing `optimum-graphcore-0.6.1/tests/test_examples_match_transformers.py` & `optimum-graphcore-0.7.0/tests/test_examples_match_transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2022 the HuggingFace Inc. team.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,15 +23,15 @@
 from git import Repo
 
 from .create_diff_file_for_example import DIFF_DIRECTORY, diff
 
 
 TRANSFORMERS_REPO_URL = "https://github.com/huggingface/transformers.git"
 TRANSFORMERS_REPO_PATH = Path("transformers")
-TRANSFORMERS_REPO_BRANCH = "v4.25-release"
+TRANSFORMERS_REPO_BRANCH = "v4.29-release"
 
 
 def get_examples(
     transformers_example_dir: Union[str, PathLike],
     optimum_example_dir: Union[str, PathLike],
     include_readmes: bool = False,
 ) -> List[Tuple[str]]:
```

### Comparing `optimum-graphcore-0.6.1/tests/test_ipu_configuration.py` & `optimum-graphcore-0.7.0/tests/test_ipu_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2021 HuggingFace Inc.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,26 +12,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import random
 import re
-import string
 import unittest
-from collections.abc import Iterable
-from typing import Any, Dict, Optional, Set
+from typing import Any, Dict
 
 import pytest
+from parameterized import parameterized
+from poptorch import OutputMode
 
 from optimum.graphcore import IPUConfig
 from optimum.graphcore.ipu_configuration import IncompatibleIPUConfigError
 from optimum.graphcore.modeling_utils import get_layer_ipu, split_encoder_decoder_ipu_config
-from parameterized import parameterized
-from poptorch import OutputMode
 
 
 def create_ipu_config() -> IPUConfig:
     initial_dict = IPUConfig().to_dict()
     allowed_output_modes = ["all", "sum", "final"]
     initial_dict["output_mode"] = random.choice(allowed_output_modes)
     # Setting this setting to False as it is currently not supported and will throw an error.
@@ -269,21 +268,21 @@
         self.assertEqual(e_ipu_config.matmul_proportion, [0.1, 0.2])
         self.assertEqual(d_ipu_config.matmul_proportion, [0.3, 0.4])
 
         # For generation using encoder decoder models and layers `SplitProjection`
         # and `SerializedEmbedding` placed on different IPUs, cannot
         # have serialized_{linear/embedding}_splits_per_ipu present in
         # both the encoder and decoder
-        with pytest.raises(ValueError, match=f"must have all splits placed on the"):
+        with pytest.raises(ValueError, match="must have all splits placed on the"):
             failing_ipu_config = IPUConfig(
                 layers_per_ipu=[0, 2, 2, 0], serialized_projection_splits_per_ipu=[0, 2, 2, 0]
             )
             split_encoder_decoder_ipu_config(failing_ipu_config, 2, 2)
 
-        with pytest.raises(ValueError, match=f"must have all splits placed on the"):
+        with pytest.raises(ValueError, match="must have all splits placed on the"):
             failing_ipu_config = IPUConfig(
                 layers_per_ipu=[0, 2, 2, 0], serialized_embedding_splits_per_ipu=[0, 2, 2, 0]
             )
             split_encoder_decoder_ipu_config(failing_ipu_config, 2, 2)
 
         # Test that all the other values from the original ipu_config are intact
         ipu_config = ipu_config.to_dict()
@@ -430,15 +429,14 @@
                 "matmul_proportion": [0.2, 0.3, 0.0, 0.4],
                 "replication_factor": 1,
                 "gradient_accumulation_steps": 1,
                 "ipus_per_replica": 1,
                 "embedding_serialization_factor": 1,
                 "device_iterations": 1,
                 "projection_serialization_factor": 1,
-                "embedding_serialization_factor": 1,
             }.items()
         )
     )
     def test_contents_geq_value_validator(self, attr, value, mode):
         ipu_config = IPUConfig()
         ipu_config.mode = mode
         attr = ipu_config._get_managed_attr_mode_name(attr)
```

### Comparing `optimum-graphcore-0.6.1/tests/test_modeling_common.py` & `optimum-graphcore-0.7.0/tests/test_modeling_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import random
 
 import torch
-
 from transformers.testing_utils import torch_device
 
 
 global_rng = random.Random()
 
 
 def ids_tensor(shape, vocab_size, rng=None, name=None):
```

### Comparing `optimum-graphcore-0.6.1/tests/test_modeling_utils.py` & `optimum-graphcore-0.7.0/tests/test_modeling_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+# Copyright (c) 2023 Graphcore Ltd. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import unittest
 from abc import abstractmethod
 
-import pytest
+import poptorch
 import torch
+from parameterized import parameterized
 
-import poptorch
 from optimum.graphcore.modeling_utils import SerializedEmbedding, SerializedLinear, SplitProjection
-from parameterized import parameterized
 
 
 DATALOADER_BATCH_SIZE = 8
 
 
 class RandomDataset:
     def __init__(self, num_features: int, num_samples: int, rand_func: torch.randn) -> None:
@@ -159,7 +172,13 @@
                 serialized_embedding.parallelize(serialized_embedding_splits_per_ipu),
                 options,
             )
         else:
             other_evaluator = PytorchEvaluator(serialized_embedding)
 
         return evaluator, other_evaluator, dataset
+
+    @parameterized.expand(((1, 0, 1), (63, 3, 15)))
+    def test_padding_idx(self, padding_idx, split, expected_padding_idx):
+        embedding = torch.nn.Embedding(num_embeddings=64, embedding_dim=8, padding_idx=padding_idx)
+        serialized_embedding = SerializedEmbedding.from_model(embedding, 4)
+        assert serialized_embedding.split_embeddings[split].padding_idx == expected_padding_idx
```

### Comparing `optimum-graphcore-0.6.1/tests/test_pipelined_models.py` & `optimum-graphcore-0.7.0/tests/test_pipelined_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 # Copyright 2021 HuggingFace Inc.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,24 +12,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 from unittest import TestCase
 
+import requests
 import torch
+import transformers
 from datasets import load_dataset
+from parameterized import parameterized
 from PIL import Image
 from torch.nn.utils.weight_norm import WeightNorm
-
-import requests
-import transformers
-from optimum.graphcore import IPUConfig
-from optimum.graphcore.modeling_utils import _PRETRAINED_TO_PIPELINED_REGISTRY
-from parameterized import parameterized
 from transformers import (
     CONFIG_MAPPING,
     MODEL_FOR_AUDIO_CLASSIFICATION_MAPPING,
     MODEL_FOR_CAUSAL_LM_MAPPING,
     MODEL_FOR_CTC_MAPPING,
     MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING,
     MODEL_FOR_MASKED_LM_MAPPING,
@@ -42,17 +40,22 @@
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
     MODEL_MAPPING,
     AutoFeatureExtractor,
     AutoProcessor,
     AutoTokenizer,
 )
 
-from .utils import MODELS_TO_TEST_MAPPING
+from optimum.graphcore import IPUConfig
+from optimum.graphcore.modeling_utils import _PRETRAINED_TO_PIPELINED_REGISTRY
+
+from .utils import CONFIG_MAPPING_EXTRA, MODEL_MAPPING_EXTRA, MODELS_TO_TEST_MAPPING, MODELS_TO_TEST_MAPPING_EXTRA
 
 
+MODELS_TO_TEST_MAPPING.update(MODELS_TO_TEST_MAPPING_EXTRA)
+[CONFIG_MAPPING.register(k, v) for k, v in CONFIG_MAPPING_EXTRA.items()]
 REVERSE_CONFIG_MAPPING = {v: k for k, v in CONFIG_MAPPING.items()}
 
 
 def _get_models_to_test(model_to_test_names):
     def find_config_class_from_pretrained_class(pretrained_class):
         mappings = [
             MODEL_FOR_AUDIO_CLASSIFICATION_MAPPING,
@@ -65,14 +68,15 @@
             MODEL_FOR_PRETRAINING_MAPPING,
             MODEL_FOR_QUESTION_ANSWERING_MAPPING,
             MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
             MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
             MODEL_FOR_SPEECH_SEQ_2_SEQ_MAPPING,
             MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
             MODEL_MAPPING,
+            MODEL_MAPPING_EXTRA,
         ]
         config_class = None
         for mapping in mappings:
             for k, v in mapping.items():
                 if v is pretrained_class:
                     config_class = k
                     break
```

### Comparing `optimum-graphcore-0.6.1/tests/test_trainer.py` & `optimum-graphcore-0.7.0/tests/test_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,85 +1,71 @@
 # coding=utf-8
 # Copyright 2021 the HuggingFace Inc. team.
+# Copyright (c) 2022 Graphcore Ltd. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import dataclasses
-import gc
 import math
 import os
 import random
 import re
 import subprocess
 import tempfile
 import unittest
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
-
 from huggingface_hub import HfFolder, Repository, delete_repo
-from optimum.graphcore import IPUConfig, IPUTrainingArguments
-from optimum.utils import logging
 from requests.exceptions import HTTPError
-from transformers import AutoTokenizer, IntervalStrategy, PretrainedConfig, is_torch_available
+from transformers import IntervalStrategy, PretrainedConfig, is_torch_available
 from transformers.file_utils import WEIGHTS_NAME
 from transformers.testing_utils import (
     ENDPOINT_STAGING,
     TOKEN,
     USER,
     CaptureLogger,
     TestCasePlus,
     get_gpu_count,
     get_tests_dir,
     is_staging_test,
-    require_optuna,
-    require_ray,
     require_sentencepiece,
-    require_sigopt,
     require_tokenizers,
     require_torch,
-    require_torch_gpu,
-    require_torch_multi_gpu,
-    require_torch_non_multi_gpu,
-    require_torch_up_to_2_gpus,
-    slow,
 )
 from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
-from transformers.utils.hp_naming import TrialShortNamer
+
+from optimum.graphcore import IPUConfig, IPUTrainingArguments
+from optimum.utils import logging
 
 
 if is_torch_available():
+    import poptorch
     import torch
     from torch import nn
     from torch.utils.data import IterableDataset
-
-    import poptorch
-    from optimum.graphcore import IPUTrainer, IPUTrainerState
     from transformers import (
-        AutoModelForSequenceClassification,
         EarlyStoppingCallback,
-        GlueDataset,
-        GlueDataTrainingArguments,
         GPT2Config,
         GPT2LMHeadModel,
-        LineByLineTextDataset,
         PreTrainedModel,
     )
-    from transformers.modeling_utils import unwrap_model
+
+    from optimum.graphcore import IPUTrainer, IPUTrainerState
 
 
 PATH_SAMPLE_TEXT = f"{get_tests_dir()}/fixtures/sample_text.txt"
 
 TRAIN_LEN = 64
 EVAL_LEN = 32
 
@@ -784,15 +770,15 @@
     def test_can_resume_training(self):
         # This test will fail for more than 2 GPUs since the batch size will get bigger and with the number of
         # save_steps, the checkpoint will resume training at epoch 2 or more (so the data seen by the model
         # won't be the same since the training dataloader is shuffled).
 
         with tempfile.TemporaryDirectory() as tmpdir:
             # Make sure there are enough samples to end up with at least a checkpoint-15
-            kwargs = dict(output_dir=tmpdir, train_len=TRAIN_LEN, save_steps=5, learning_rate=0.1)
+            kwargs = {"output_dir": tmpdir, "train_len": TRAIN_LEN, "save_steps": 5, "learning_rate": 0.1}
             trainer = get_regression_trainer(**kwargs)
             trainer.train()
             (a, b) = trainer.model.a.item(), trainer.model.b.item()
             state = dataclasses.asdict(trainer.state)
 
             checkpoint = os.path.join(tmpdir, "checkpoint-5")
 
@@ -818,15 +804,21 @@
             self.assertEqual(a, a1)
             self.assertEqual(b, b1)
             self.check_trainer_state_are_the_same(state, state1)
 
         # With a regular model that is not a PreTrainedModel
         with tempfile.TemporaryDirectory() as tmpdir:
             # Make sure there are enough samples to end up with at least a checkpoint-15
-            kwargs = dict(output_dir=tmpdir, train_len=TRAIN_LEN, save_steps=5, learning_rate=0.1, pretrained=False)
+            kwargs = {
+                "output_dir": tmpdir,
+                "train_len": TRAIN_LEN,
+                "save_steps": 5,
+                "learning_rate": 0.1,
+                "pretrained": False,
+            }
 
             trainer = get_regression_trainer(**kwargs)
             trainer.train()
             (a, b) = trainer.model.a.item(), trainer.model.b.item()
             state = dataclasses.asdict(trainer.state)
 
             checkpoint = os.path.join(tmpdir, "checkpoint-5")
```

