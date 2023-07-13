# Comparing `tmp/antspynet-0.2.2.tar.gz` & `tmp/antspynet-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspynet-0.2.2.tar", last modified: Wed Jun 21 17:16:41 2023, max compression
+gzip compressed data, was "antspynet-0.2.3.tar", last modified: Thu Jul 13 15:45:32 2023, max compression
```

## Comparing `antspynet-0.2.2.tar` & `antspynet-0.2.3.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.249667 antspynet-0.2.2/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.2/LICENSE.md
--rw-r--r--   0 stnava     (501) staff       (20)     8207 2023-06-21 17:16:41.249465 antspynet-0.2.2/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     7786 2023-06-21 17:14:39.000000 antspynet-0.2.2/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.235776 antspynet-0.2.2/antspynet/
--rw-r--r--   0 stnava     (501) staff       (20)      115 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/__init__.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.242016 antspynet-0.2.2/antspynet/architectures/
--rw-r--r--   0 stnava     (501) staff       (20)     3120 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)    14057 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_alexnet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     2090 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_autoencoder_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8296 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_convolutional_autoencoder_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     3121 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_custom_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    36597 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_custom_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    14211 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_cycle_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    19564 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_deep_back_projection_network_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    10368 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_deep_convolutional_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8187 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_deep_denoise_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6197 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     1704 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_dense_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    13539 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_densenet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    19534 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_denseunet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    15888 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_diffusion_probabilistic_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6163 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_expanded_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     5198 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_image_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    12707 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_improved_wasserstein_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    13493 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_partial_convolution_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    17281 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_resnet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8637 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_resnet_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    27712 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_resunet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     7749 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    16664 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_super_resolution_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    21492 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6447 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_vanilla_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    11244 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_vgg_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    11233 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_wasserstein_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    15261 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/architectures/create_wide_resnet_model.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.249170 antspynet-0.2.2/antspynet/utilities/
--rw-r--r--   0 stnava     (501) staff       (20)     4284 2023-06-09 14:56:59.000000 antspynet-0.2.2/antspynet/utilities/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)     8814 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/attention_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     5082 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/brain_age.py
--rw-r--r--   0 stnava     (501) staff       (20)    10772 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/brain_extraction.py
--rw-r--r--   0 stnava     (501) staff       (20)    17672 2023-06-21 17:14:39.000000 antspynet-0.2.2/antspynet/utilities/cerebellum_morphology.py
--rw-r--r--   0 stnava     (501) staff       (20)     8303 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/claustrum_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     8886 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/cortical_thickness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3104 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/cropping_and_padding_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     1002 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/custom_activation_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)    10664 2023-06-06 13:37:10.000000 antspynet-0.2.2/antspynet/utilities/custom_convolution_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)     8323 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/custom_metrics.py
--rw-r--r--   0 stnava     (501) staff       (20)     5826 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/custom_normalization_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)    13137 2023-06-09 14:56:59.000000 antspynet-0.2.2/antspynet/utilities/data_augmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     6820 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/deep_atropos.py
--rw-r--r--   0 stnava     (501) staff       (20)     8009 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/deep_embedded_clustering_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    40348 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/deep_flash.py
--rw-r--r--   0 stnava     (501) staff       (20)     1688 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/denseunet_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    20746 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/desikan_killiany_tourville_labeling.py
--rw-r--r--   0 stnava     (501) staff       (20)     9997 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/extract_image_patches.py
--rw-r--r--   0 stnava     (501) staff       (20)     6901 2023-06-09 14:56:59.000000 antspynet-0.2.2/antspynet/utilities/gaussian_diffusion_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     5812 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/get_antsxnet_data.py
--rw-r--r--   0 stnava     (501) staff       (20)    17128 2023-06-21 17:14:39.000000 antspynet-0.2.2/antspynet/utilities/get_pretrained_network.py
--rw-r--r--   0 stnava     (501) staff       (20)     8601 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/hippmapp3r_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     4847 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/histogram_warp_image_intensities.py
--rw-r--r--   0 stnava     (501) staff       (20)    29323 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/histology.py
--rw-r--r--   0 stnava     (501) staff       (20)     4969 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/hypothalamus_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)    11285 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/inpainting.py
--rw-r--r--   0 stnava     (501) staff       (20)    18785 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/lung_extraction.py
--rw-r--r--   0 stnava     (501) staff       (20)     6558 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/lung_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)    12055 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/mixture_density_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     1606 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/mri_super_resolution.py
--rw-r--r--   0 stnava     (501) staff       (20)    18169 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/neural_style_transfer.py
--rw-r--r--   0 stnava     (501) staff       (20)     8722 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/preprocess_image.py
--rw-r--r--   0 stnava     (501) staff       (20)    17035 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/quality_assessment.py
--rw-r--r--   0 stnava     (501) staff       (20)    11102 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/randomly_transform_image_data.py
--rw-r--r--   0 stnava     (501) staff       (20)    11224 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/reconstruct_image_from_patches.py
--rw-r--r--   0 stnava     (501) staff       (20)     2856 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/regression_match_image.py
--rw-r--r--   0 stnava     (501) staff       (20)    11048 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/resample_tensor_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     2518 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/simulate_bias_field.py
--rw-r--r--   0 stnava     (501) staff       (20)    14538 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/spatial_transformer_network_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    11177 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/super_resolution_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     8426 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/ukbb.py
--rw-r--r--   0 stnava     (501) staff       (20)     2871 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/unet_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    46891 2023-06-06 13:36:51.000000 antspynet-0.2.2/antspynet/utilities/white_matter_hyperintensity_segmentation.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-21 17:16:41.236753 antspynet-0.2.2/antspynet.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     8207 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     3898 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-06 13:37:14.000000 antspynet-0.2.2/antspynet.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)       99 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)       54 2023-06-21 17:16:41.000000 antspynet-0.2.2/antspynet.egg-info/top_level.txt
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-06-21 17:16:41.249716 antspynet-0.2.2/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      791 2023-06-21 17:15:26.000000 antspynet-0.2.2/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.682082 antspynet-0.2.3/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.3/LICENSE.md
+-rw-r--r--   0 stnava     (501) staff       (20)     8365 2023-07-13 15:45:32.681891 antspynet-0.2.3/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     7944 2023-07-13 13:29:28.000000 antspynet-0.2.3/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.663018 antspynet-0.2.3/antspynet/
+-rw-r--r--   0 stnava     (501) staff       (20)       76 2023-07-13 13:31:06.000000 antspynet-0.2.3/antspynet/__init__.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.671349 antspynet-0.2.3/antspynet/architectures/
+-rw-r--r--   0 stnava     (501) staff       (20)     3369 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/architectures/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14057 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_alexnet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2090 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_autoencoder_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8296 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_convolutional_autoencoder_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3121 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_custom_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    36597 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_custom_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14211 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_cycle_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    19564 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_deep_back_projection_network_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    10368 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_deep_convolutional_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8187 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_deep_denoise_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6197 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1704 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_dense_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    13539 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_densenet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    19534 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_denseunet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    15888 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_diffusion_probabilistic_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6163 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_expanded_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5198 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_image_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    12707 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_improved_wasserstein_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    13493 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_partial_convolution_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17166 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/architectures/create_resnet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8637 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_resnet_super_resolution_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    27712 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_resunet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     7749 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    16664 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_super_resolution_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    16819 2023-07-13 14:21:43.000000 antspynet-0.2.3/antspynet/architectures/create_transformer_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    21396 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/architectures/create_unet_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6447 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_vanilla_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11244 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_vgg_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11233 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_wasserstein_gan_model.py
+-rw-r--r--   0 stnava     (501) staff       (20)    15261 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_wide_resnet_model.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.681253 antspynet-0.2.3/antspynet/utilities/
+-rw-r--r--   0 stnava     (501) staff       (20)     4519 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8814 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/attention_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4994 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/brain_age.py
+-rw-r--r--   0 stnava     (501) staff       (20)    10684 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/brain_extraction.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17634 2023-07-13 14:23:17.000000 antspynet-0.2.3/antspynet/utilities/cerebellum_morphology.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8215 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/claustrum_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8886 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/cortical_thickness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3104 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/cropping_and_padding_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1002 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/custom_activation_layers.py
+-rw-r--r--   0 stnava     (501) staff       (20)    10664 2023-06-06 13:37:10.000000 antspynet-0.2.3/antspynet/utilities/custom_convolution_layers.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8323 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/custom_metrics.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5826 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/custom_normalization_layers.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14233 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/data_augmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6732 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/deep_atropos.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8009 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/deep_embedded_clustering_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    40258 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/deep_flash.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1688 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/denseunet_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    20657 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/desikan_killiany_tourville_labeling.py
+-rw-r--r--   0 stnava     (501) staff       (20)     9997 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/extract_image_patches.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6901 2023-06-09 14:56:59.000000 antspynet-0.2.3/antspynet/utilities/gaussian_diffusion_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     5768 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/get_antsxnet_data.py
+-rw-r--r--   0 stnava     (501) staff       (20)    17235 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/get_pretrained_network.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8513 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/hippmapp3r_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4847 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/histogram_warp_image_intensities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    28688 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/histology.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4881 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/hypothalamus_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11197 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/inpainting.py
+-rw-r--r--   0 stnava     (501) staff       (20)    18688 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/lung_extraction.py
+-rw-r--r--   0 stnava     (501) staff       (20)     6470 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/lung_segmentation.py
+-rw-r--r--   0 stnava     (501) staff       (20)    12055 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/mixture_density_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3375 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/mri_modality_classification.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1518 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/mri_super_resolution.py
+-rw-r--r--   0 stnava     (501) staff       (20)    18169 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/neural_style_transfer.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8633 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/preprocess_image.py
+-rw-r--r--   0 stnava     (501) staff       (20)    16947 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/quality_assessment.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11102 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/randomly_transform_image_data.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11224 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/reconstruct_image_from_patches.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2856 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/regression_match_image.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11048 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/resample_tensor_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2518 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/simulate_bias_field.py
+-rw-r--r--   0 stnava     (501) staff       (20)    14538 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/spatial_transformer_network_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    11177 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/super_resolution_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     7144 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/transformer_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)     8233 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/ukbb.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2871 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/unet_utilities.py
+-rw-r--r--   0 stnava     (501) staff       (20)    46627 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/white_matter_hyperintensity_segmentation.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.664145 antspynet-0.2.3/antspynet.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)     8365 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     4046 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-06 13:37:14.000000 antspynet-0.2.3/antspynet.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)       99 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       54 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/top_level.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-07-13 15:45:32.682126 antspynet-0.2.3/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-07-13 13:29:28.000000 antspynet-0.2.3/setup.py
```

### Comparing `antspynet-0.2.2/LICENSE.md` & `antspynet-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/PKG-INFO` & `antspynet-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: antspynet
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of deep learning architectures ported to the python language and tools for basic medical image processing.
 Home-page: https://github.com/ANTsX/ANTsPyNet
 Author: Nicholas J. Tustison and Brian B. Avants and Nick Cullen
 Author-email: ntustison@gmail.com
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.md
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
+[![PubMed](https://img.shields.io/badge/ANTsX_paper-Open_Access-8DABFF?logo=pubmed)](https://pubmed.ncbi.nlm.nih.gov/33907199/)
 
 # ANTsPyNet
 
 A collection of deep learning architectures and applications ported to the python language and tools for basic medical image processing. Based on `keras` and `tensorflow` with cross-compatibility with our R analog [ANTsRNet](https://github.com/ANTsX/ANTsRNet/).
 
 Documentation page [https://antsx.github.io/ANTsPyNet/](https://antsx.github.io/ANTsPyNet/).
 
@@ -89,14 +90,15 @@
 * [Sysu white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/30125711/)
 * [HyperMapp3r white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/35088930/)
 * [Hypothalamus segmentation](https://pubmed.ncbi.nlm.nih.gov/32853816/)
 * [Claustrum segmentation](https://arxiv.org/abs/2008.03465)
 * [Deep Flash](https://www.medrxiv.org/content/10.1101/2023.01.17.23284693v1)
 * Desikan-Killiany-Tourville cortical labeling
 * Cerebellum segmentation, parcellation, and thickness
+* MRI modality classification
 * Lung extraction
     * [Proton](https://www.ncbi.nlm.nih.gov/pubmed/30195415)
     * CT
 * [Functional lung segmentation](https://www.medrxiv.org/content/10.1101/2021.03.04.21252588v2)
 * [Neural style transfer](https://arxiv.org/abs/1508.06576)
 * Image quality assessment
     * [TID2013](https://www.sciencedirect.com/science/article/pii/S0923596514001490)
```

### Comparing `antspynet-0.2.2/README.md` & `antspynet-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
+[![PubMed](https://img.shields.io/badge/ANTsX_paper-Open_Access-8DABFF?logo=pubmed)](https://pubmed.ncbi.nlm.nih.gov/33907199/)
 
 # ANTsPyNet
 
 A collection of deep learning architectures and applications ported to the python language and tools for basic medical image processing. Based on `keras` and `tensorflow` with cross-compatibility with our R analog [ANTsRNet](https://github.com/ANTsX/ANTsRNet/).
 
 Documentation page [https://antsx.github.io/ANTsPyNet/](https://antsx.github.io/ANTsPyNet/).
 
@@ -79,14 +80,15 @@
 * [Sysu white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/30125711/)
 * [HyperMapp3r white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/35088930/)
 * [Hypothalamus segmentation](https://pubmed.ncbi.nlm.nih.gov/32853816/)
 * [Claustrum segmentation](https://arxiv.org/abs/2008.03465)
 * [Deep Flash](https://www.medrxiv.org/content/10.1101/2023.01.17.23284693v1)
 * Desikan-Killiany-Tourville cortical labeling
 * Cerebellum segmentation, parcellation, and thickness
+* MRI modality classification
 * Lung extraction
     * [Proton](https://www.ncbi.nlm.nih.gov/pubmed/30195415)
     * CT
 * [Functional lung segmentation](https://www.medrxiv.org/content/10.1101/2021.03.04.21252588v2)
 * [Neural style transfer](https://arxiv.org/abs/1508.06576)
 * Image quality assessment
     * [TID2013](https://www.sciencedirect.com/science/article/pii/S0923596514001490)
```

### Comparing `antspynet-0.2.2/antspynet/architectures/__init__.py` & `antspynet-0.2.3/antspynet/architectures/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,7 +33,10 @@
 from .create_deep_convolutional_gan_model import DeepConvolutionalGanModel
 from .create_wasserstein_gan_model import WassersteinGanModel
 from .create_improved_wasserstein_gan_model import ImprovedWassersteinGanModel
 from .create_cycle_gan_model import CycleGanModel
 from .create_super_resolution_gan_model import SuperResolutionGanModel
 
 from .create_dense_model import create_dense_model
+
+from .create_transformer_model import create_vision_transformer_model_2d, create_vision_transformer_model_3d
+from .create_transformer_model import create_compact_convolutional_transformer_model_2d, create_compact_convolutional_transformer_model_3d
```

### Comparing `antspynet-0.2.2/antspynet/architectures/create_alexnet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_alexnet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_autoencoder_model.py` & `antspynet-0.2.3/antspynet/architectures/create_autoencoder_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_convolutional_autoencoder_model.py` & `antspynet-0.2.3/antspynet/architectures/create_convolutional_autoencoder_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_custom_model.py` & `antspynet-0.2.3/antspynet/architectures/create_custom_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_custom_unet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_custom_unet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_cycle_gan_model.py` & `antspynet-0.2.3/antspynet/architectures/create_cycle_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_deep_back_projection_network_model.py` & `antspynet-0.2.3/antspynet/architectures/create_deep_back_projection_network_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_deep_convolutional_gan_model.py` & `antspynet-0.2.3/antspynet/architectures/create_deep_convolutional_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_deep_denoise_super_resolution_model.py` & `antspynet-0.2.3/antspynet/architectures/create_deep_denoise_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py` & `antspynet-0.2.3/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_dense_model.py` & `antspynet-0.2.3/antspynet/architectures/create_dense_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_densenet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_densenet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_denseunet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_denseunet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_diffusion_probabilistic_unet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_diffusion_probabilistic_unet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_expanded_super_resolution_model.py` & `antspynet-0.2.3/antspynet/architectures/create_expanded_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_image_super_resolution_model.py` & `antspynet-0.2.3/antspynet/architectures/create_image_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_improved_wasserstein_gan_model.py` & `antspynet-0.2.3/antspynet/architectures/create_improved_wasserstein_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_partial_convolution_unet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_partial_convolution_unet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_resnet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_resnet_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 
 import tensorflow as tf
 
 import tensorflow.keras.backend as K
 
 from tensorflow.keras.models import Model
-from tensorflow.keras.layers import (Input, Dropout, BatchNormalization, Add,
+from tensorflow.keras.layers import (Input, BatchNormalization, Add,
                                      LeakyReLU, Concatenate, Lambda, Dense,
-                                     Reshape, Permute, Multiply,
-                                     Conv2D, Conv2DTranspose,
-                                     MaxPooling2D, GlobalAveragePooling2D,
-                                     UpSampling2D,
-                                     Conv3D, Conv3DTranspose,
-                                     MaxPooling3D, GlobalAveragePooling3D,
-                                     UpSampling3D)
+                                     Reshape, Multiply, Conv2D,
+                                     MaxPooling2D, GlobalAveragePooling2D, Conv3D,
+                                     MaxPooling3D, GlobalAveragePooling3D)
 
 def create_resnet_model_2d(input_image_size,
                            input_scalars_size=0,
                            number_of_classification_labels=1000,
                            layers=(1, 2, 3, 4),
                            residual_block_schedule=(3, 4, 6, 3),
                            lowest_resolution=64,
@@ -57,22 +53,22 @@
     residual_block_schedule : tuple
         A tuple defining the how many residual blocks repeats for each layer.
 
     lowest_resolution : integer
         Number of filters at the initial layer.
 
     cardinality : integer
-        perform ResNet (cardinality = 1) or ResNeX (cardinality does not 1 but,
+        perform ResNet (cardinality = 1) or ResNeX (cardinality is not 1 but,
         instead, powers of 2---try '32').
 
     squeeze_and_excite : boolean
         add the squeeze-and-excite block variant.
 
     mode : string
-        'classification' or 'regression'.  Default = 'classification'.
+        'classification', 'sigmoid' or 'regression'.  Default = 'classification'.
 
     Returns
     -------
     Keras model
         A 2-D Keras model defining the network.
 
     Example
@@ -96,15 +92,15 @@
                                    strides=strides,
                                    padding='same')(model)
             return(grouped_model)
 
         if number_of_filters % cardinality != 0:
             raise ValueError('number_of_filters `%` cardinality != 0')
 
-        number_of_group_filters = int(number_of_filters / cardinality)
+        number_of_group_filters = number_of_filters // cardinality
 
         convolution_layers = []
         for j in range(cardinality):
             local_layer = Lambda(lambda z: z[:, :, :,
               j * number_of_group_filters:j * number_of_group_filters + number_of_group_filters])(model)
             convolution_layers.append(Conv2D(filters=number_of_group_filters,
                                              kernel_size=(3, 3),
@@ -132,19 +128,19 @@
                       kernel_initializer='he_normal',
                       use_bias=False)(block)
 
         x = Multiply()([initial, block])
         return(x)
 
     def residual_block_2d(model,
-                         number_of_filters_in,
-                         number_of_filters_out,
-                         strides=(1, 1),
-                         project_shortcut=False,
-                         squeeze_and_excite=False):
+                          number_of_filters_in,
+                          number_of_filters_out,
+                          strides=(1, 1),
+                          project_shortcut=False,
+                          squeeze_and_excite=False):
         shortcut = model
 
         model = Conv2D(filters=number_of_filters_in,
                        kernel_size=(1, 1),
                        strides=(1, 1),
                        padding='same')(model)
         model = add_common_layers(model)
@@ -157,22 +153,22 @@
 
         model = Conv2D(filters=number_of_filters_out,
                        kernel_size=(1, 1),
                        strides=(1, 1),
                        padding='same')(model)
         model = BatchNormalization()(model)
 
-        if project_shortcut == True or strides != (1,1):
+        if project_shortcut or strides != (1,1):
             shortcut = Conv2D(filters=number_of_filters_out,
                               kernel_size=(1, 1),
                               strides=strides,
                               padding='same')(shortcut)
             shortcut = BatchNormalization()(shortcut)
 
-        if squeeze_and_excite == True:
+        if squeeze_and_excite:
             model = squeeze_and_excite_block_2d(model)
 
         model = Add()([shortcut, model])
         model = LeakyReLU()(model)
         return(model)
 
 
@@ -213,14 +209,16 @@
     outputs = GlobalAveragePooling2D()(outputs)
 
     layer_activation = ''
     if mode == 'classification':
         layer_activation = 'softmax'
     elif mode == 'regression':
         layer_activation = 'linear'
+    elif mode == 'sigmoid':
+        layer_activation = 'sigmoid'
     else:
         raise ValueError('mode must be either `classification` or `regression`.')
 
     resnet_model = None
     if input_scalars_size > 0:
         input_scalars = Input( shape = (input_scalars_size,) )
         concatenated_layer = Concatenate()([outputs, input_scalars])
@@ -277,22 +275,22 @@
     residual_block_schedule : tuple
         A tuple defining the how many residual blocks repeats for each layer.
 
     lowest_resolution : integer
         Number of filters at the initial layer.
 
     cardinality : integer
-        perform ResNet (cardinality = 1) or ResNeX (cardinality does not 1 but,
+        perform ResNet (cardinality = 1) or ResNeX (cardinality is not 1 but,
         instead, powers of 2---try '32').
 
     squeeze_and_excite : boolean
         add the squeeze-and-excite block variant.
 
     mode : string
-        'classification' or 'regression'.  Default = 'classification'.
+        'classification', 'sigmoid' or 'regression'.  Default = 'classification'.
 
     Returns
     -------
     Keras model
         A 3-D Keras model defining the network.
 
     Example
@@ -316,15 +314,15 @@
                                    strides=strides,
                                    padding='same')(model)
             return(grouped_model)
 
         if number_of_filters % cardinality != 0:
             raise ValueError('number_of_filters `%` cardinality != 0')
 
-        number_of_group_filters = int(number_of_filters / cardinality)
+        number_of_group_filters = number_of_filters // cardinality
 
         convolution_layers = []
         for j in range(cardinality):
             local_layer = Lambda(lambda z: z[:, :, :, :,
               j * number_of_group_filters:j * number_of_group_filters + number_of_group_filters])(model)
             convolution_layers.append(Conv3D(filters=number_of_group_filters,
                                              kernel_size=(3, 3, 3),
@@ -377,22 +375,22 @@
 
         model = Conv3D(filters=number_of_filters_out,
                        kernel_size=(1, 1, 1),
                        strides=(1, 1, 1),
                        padding='same')(model)
         model = BatchNormalization()(model)
 
-        if project_shortcut == True or strides != (1,1,1):
+        if project_shortcut or strides != (1,1,1):
             shortcut = Conv3D(filters=number_of_filters_out,
                               kernel_size=(1, 1, 1),
                               strides=strides,
                               padding='same')(shortcut)
             shortcut = BatchNormalization()(shortcut)
 
-        if squeeze_and_excite == True:
+        if squeeze_and_excite:
             model = squeeze_and_excite_block_3d(model)
 
         model = Add()([shortcut, model])
         model = LeakyReLU()(model)
         return(model)
 
 
@@ -434,14 +432,16 @@
     outputs = GlobalAveragePooling3D()(outputs)
 
     layer_activation = ''
     if mode == 'classification':
         layer_activation = 'softmax'
     elif mode == 'regression':
         layer_activation = 'linear'
+    elif mode == 'sigmoid':
+        layer_activation = 'sigmoid'
     else:
         raise ValueError('mode must be either `classification` or `regression`.')
 
     resnet_model = None
     if input_scalars_size > 0:
         input_scalars = Input( shape = (input_scalars_size,) )
         concatenated_layer = Concatenate()([outputs, input_scalars])
```

### Comparing `antspynet-0.2.2/antspynet/architectures/create_resnet_super_resolution_model.py` & `antspynet-0.2.3/antspynet/architectures/create_resnet_super_resolution_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_resunet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_resunet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py` & `antspynet-0.2.3/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_super_resolution_gan_model.py` & `antspynet-0.2.3/antspynet/architectures/create_super_resolution_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_unet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_unet_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
                           kernel_regularizer=regularizers.l2(weight_decay))(inputs)
         else:
             conv = Conv2D(filters=number_of_filters[i],
                           kernel_size=convolution_kernel_size,
                           padding='same',
                           kernel_regularizer=regularizers.l2(weight_decay))(pool)
 
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             conv = nn_unet_activation(conv)
         else:
             conv = ReLU()(conv)
 
         if dropout_rate > 0.0:
             conv = Dropout(rate=dropout_rate)(conv)
 
@@ -197,15 +197,15 @@
                           kernel_size=initial_convolution_kernel_size,
                           padding='same')(conv)
         else:
             conv = Conv2D(filters=number_of_filters[i],
                           kernel_size=convolution_kernel_size,
                           padding='same')(conv)
 
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             conv = nn_unet_activation(conv)
         else:
             conv = ReLU()(conv)
 
         encoding_convolution_layers.append(conv)
 
         if i < number_of_layers - 1:
@@ -225,44 +225,44 @@
 
     outputs = encoding_convolution_layers[number_of_layers - 1]
     for i in range(1, number_of_layers):
         deconv = Conv2DTranspose(filters=number_of_filters[number_of_layers-i-1],
                                  kernel_size=deconvolution_kernel_size,
                                  padding='same',
                                  kernel_regularizer=regularizers.l2(weight_decay))(outputs)
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             deconv = nn_unet_activation(deconv)
         deconv = UpSampling2D(size=pool_size)(deconv)
 
-        if add_attention_gating == True:
+        if add_attention_gating:
             outputs = attention_gate_2d(deconv,
               encoding_convolution_layers[number_of_layers-i-1],
               number_of_filters[number_of_layers-i-1] // 4)
             outputs = Concatenate(axis=3)([deconv, outputs])
         else:
             outputs = Concatenate(axis=3)([deconv, encoding_convolution_layers[number_of_layers-i-1]])
 
         outputs = Conv2D(filters=number_of_filters[number_of_layers-i-1],
                          kernel_size=convolution_kernel_size,
                          padding='same',
                          kernel_regularizer=regularizers.l2(weight_decay))(outputs)
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             outputs = nn_unet_activation(outputs)
         else:
             outputs = ReLU()(outputs)
 
         if dropout_rate > 0.0:
             outputs = Dropout(rate=dropout_rate)(outputs)
 
         outputs = Conv2D(filters=number_of_filters[number_of_layers-i-1],
                          kernel_size=convolution_kernel_size,
                          padding='same',
                          kernel_regularizer=regularizers.l2(weight_decay))(outputs)
 
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             outputs = nn_unet_activation(outputs)
         else:
             outputs = ReLU()(outputs)
 
     conv_activation = ''
 
     if mode == 'sigmoid':
@@ -457,15 +457,15 @@
                           kernel_regularizer=regularizers.l2(weight_decay))(inputs)
         else:
             conv = Conv3D(filters=number_of_filters[i],
                           kernel_size=convolution_kernel_size,
                           padding='same',
                           kernel_regularizer=regularizers.l2(weight_decay))(pool)
 
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             conv = nn_unet_activation(conv)
         else:
             conv = ReLU()(conv)
 
         if dropout_rate > 0.0:
             conv = Dropout(rate=dropout_rate)(conv)
 
@@ -474,15 +474,15 @@
                           kernel_size=initial_convolution_kernel_size,
                           padding='same')(conv)
         else:
             conv = Conv3D(filters=number_of_filters[i],
                           kernel_size=convolution_kernel_size,
                           padding='same')(conv)
 
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             conv = nn_unet_activation(conv)
         else:
             conv = ReLU()(conv)
 
         encoding_convolution_layers.append(conv)
 
         if i < number_of_layers - 1:
@@ -502,44 +502,44 @@
 
     outputs = encoding_convolution_layers[number_of_layers - 1]
     for i in range(1, number_of_layers):
         deconv = Conv3DTranspose(filters=number_of_filters[number_of_layers-i-1],
                                  kernel_size=deconvolution_kernel_size,
                                  padding='same',
                                  kernel_regularizer=regularizers.l2(weight_decay))(outputs)
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             deconv = nn_unet_activation(deconv)
         deconv = UpSampling3D(size=pool_size)(deconv)
 
-        if add_attention_gating == True:
+        if add_attention_gating:
             outputs = attention_gate_3d(deconv,
               encoding_convolution_layers[number_of_layers-i-1],
               number_of_filters[number_of_layers-i-1] // 4)
             outputs = Concatenate(axis=4)([deconv, outputs])
         else:
             outputs = Concatenate(axis=4)([deconv, encoding_convolution_layers[number_of_layers-i-1]])
 
         outputs = Conv3D(filters=number_of_filters[number_of_layers-i-1],
                          kernel_size=convolution_kernel_size,
                          padding='same',
                          kernel_regularizer=regularizers.l2(weight_decay))(outputs)
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             outputs = nn_unet_activation(outputs)
         else:
             outputs = ReLU()(outputs)
 
         if dropout_rate > 0.0:
             outputs = Dropout(rate=dropout_rate)(outputs)
 
         outputs = Conv3D(filters=number_of_filters[number_of_layers-i-1],
                          kernel_size=convolution_kernel_size,
                          padding='same',
                          kernel_regularizer=regularizers.l2(weight_decay))(outputs)
 
-        if nn_unet_activation_style == True:
+        if nn_unet_activation_style:
             outputs = nn_unet_activation(outputs)
         else:
             outputs = ReLU()(outputs)
 
     conv_activation = ''
     if mode == 'sigmoid':
         conv_activation = 'sigmoid'
```

### Comparing `antspynet-0.2.2/antspynet/architectures/create_vanilla_gan_model.py` & `antspynet-0.2.3/antspynet/architectures/create_vanilla_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_vgg_model.py` & `antspynet-0.2.3/antspynet/architectures/create_vgg_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_wasserstein_gan_model.py` & `antspynet-0.2.3/antspynet/architectures/create_wasserstein_gan_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/architectures/create_wide_resnet_model.py` & `antspynet-0.2.3/antspynet/architectures/create_wide_resnet_model.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/__init__.py` & `antspynet-0.2.3/antspynet/utilities/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from .unet_utilities import encode_unet
 from .unet_utilities import decode_unet
 from .denseunet_utilities import Scale
 
 from .spatial_transformer_network_utilities import SpatialTransformer2D, SpatialTransformer3D
 
+from .transformer_utilities import ExtractPatches2D, ExtractPatches3D, EncodePatches, StochasticDepth, ExtractConvolutionalPatches2D, ExtractConvolutionalPatches3D
+
 from .extract_image_patches import extract_image_patches
 from .reconstruct_image_from_patches import reconstruct_image_from_patches
 
 from .regression_match_image import regression_match_image
 
 from .super_resolution_utilities import mse, mae, psnr, ssim, gmsd
 from .super_resolution_utilities import apply_super_resolution_model_to_image
@@ -83,8 +85,10 @@
 from .cerebellum_morphology import cerebellum_morphology
 from .brain_age import brain_age
 from .mri_super_resolution import mri_super_resolution
 from .quality_assessment import tid_neural_image_assessment
 from .quality_assessment import random_mask
 from .lung_segmentation import el_bicho
 
+from .mri_modality_classification import mri_modality_classification
+
 from .neural_style_transfer import neural_style_transfer
```

### Comparing `antspynet-0.2.2/antspynet/utilities/attention_utilities.py` & `antspynet-0.2.3/antspynet/utilities/attention_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/brain_age.py` & `antspynet-0.2.3/antspynet/utilities/brain_age.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,17 +66,14 @@
     from ..utilities import preprocess_brain_image
     from ..utilities import get_pretrained_network
     from ..utilities import randomly_transform_image_data
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     ################################
     #
     # Preprocess images
     #
     ################################
 
     t1_preprocessed = t1
```

### Comparing `antspynet-0.2.2/antspynet/utilities/brain_extraction.py` & `antspynet-0.2.3/antspynet/utilities/brain_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,14 @@
     classes = ("background", "brain")
     number_of_classification_labels = len(classes)
 
     channel_size = 1
     if isinstance(image, list):
         channel_size = len(image)
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     input_images = list()
     if channel_size == 1:
         input_images.append(image)
     else:
         input_images = image
 
     if input_images[0].dimension != 3:
```

### Comparing `antspynet-0.2.2/antspynet/utilities/cerebellum_morphology.py` & `antspynet-0.2.3/antspynet/utilities/cerebellum_morphology.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                           verbose=False
                           ):
 
     """
     Cerebellum tissue segmentation, Schmahmann parcellation, and thickness.
 
     Perform cerebellum segmentation using a modification of the set of
-    MaGET cerebellum atlases --- https://github.com/CoBrALab/MAGeTbrain.
+    MaGET cerebellum atlases --- https://www.cobralab.ca/cerebellum-lobules
 
     The tissue labeling is as follows:
 
     Label 1 : CSF
     Label 2 : Gray matter
     Label 3 : White matter
 
@@ -51,30 +51,30 @@
     Preprocessing on the training data consisted of:
        * n4 bias correction,
     which is performed on the input images if do_preprocessing = True.
 
     Arguments
     ---------
     t1 : ANTsImage
-        raw or preprocessed 3-D T1-weighted brain image.
+        raw or preprocessed 3-D T1-weighted whole head ( not brain extracted ) image.
 
     cerebellum_mask : ANTsImage
         Option for initialization.  If not specified, the cerebellum ROI is
         determined using ANTsXNet brain_extraction followed by registration
         to a template.
 
     compute_thickness_image : boolean
         Compute KellyKapowski thickness image of the gray matter.
 
     do_preprocessing : boolean
         See description above.
 
     antsxnet_cache_directory : string
         Destination directory for storing the downloaded template and model weights.
-        Since these can be resused, if is None, these data will be downloaded to a
+        Since these can be reused, if is None, these data will be downloaded to a
         ~/.keras/ANTsXNet/.
 
     verbose : boolean
         Print progress to the screen.
 
     Returns
     -------
@@ -92,17 +92,14 @@
     from ..utilities import get_antsxnet_data
     from ..utilities import pad_or_crop_image_to_size
     from ..utilities import brain_extraction
 
     if t1.dimension != 3:
         raise ValueError("Image dimension must be 3.")
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     transform_type = "antsRegistrationSyNQuick[s]"
     whichtoinvert=[True, False, True]
     # transform_type = "antsRegistrationSyNQuick[a]"
     # whichtoinvert=[True, True]
 
     ################################
     #
@@ -110,15 +107,15 @@
     #
     ################################
 
     t1_template = ants.image_read(get_antsxnet_data("magetTemplate"))
     t1_template_brain_mask = ants.image_read(get_antsxnet_data("magetTemplateBrainMask"))
     t1_template_brain = t1_template * t1_template_brain_mask
     t1_cerebellum_template = ants.image_read(get_antsxnet_data("magetCerebellumTemplate"))
-    t1_cerebellum_template = ((t1_cerebellum_template - t1_cerebellum_template.min()) / 
+    t1_cerebellum_template = ((t1_cerebellum_template - t1_cerebellum_template.min()) /
                               (t1_cerebellum_template.max() - t1_cerebellum_template.min()))
     cerebellum_x_template_xfrm = get_antsxnet_data("magetCerebellumxTemplate0GenericAffine")
 
     # spatial priors are in the space of the cerebellar template.  First three are
     # csf, gm, and wm followed by the regions.
     spatial_priors_file_name_path = get_antsxnet_data("magetCerebellumTemplatePriors",
         antsxnet_cache_directory=antsxnet_cache_directory)
@@ -129,15 +126,15 @@
 
     ################################
     #
     # Preprocess images
     #
     ################################
 
-    t1_preprocessed = t1
+    t1_preprocessed = ants.image_clone( t1 )
     t1_mask = None
 
     template_transforms = None
     if do_preprocessing:
 
         if verbose:
             print("Preprocessing T1.")
```

### Comparing `antspynet-0.2.2/antspynet/utilities/claustrum_segmentation.py` & `antspynet-0.2.3/antspynet/utilities/claustrum_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,14 @@
     from ..utilities import get_pretrained_network
     from ..utilities import preprocess_brain_image
     from ..utilities import pad_or_crop_image_to_size
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     image_size = (180, 180)
 
     ################################
     #
     # Preprocess images
     #
     ################################
```

### Comparing `antspynet-0.2.2/antspynet/utilities/cortical_thickness.py` & `antspynet-0.2.3/antspynet/utilities/cortical_thickness.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/cropping_and_padding_utilities.py` & `antspynet-0.2.3/antspynet/utilities/cropping_and_padding_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/custom_activation_layers.py` & `antspynet-0.2.3/antspynet/utilities/custom_activation_layers.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/custom_convolution_layers.py` & `antspynet-0.2.3/antspynet/utilities/custom_convolution_layers.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/custom_metrics.py` & `antspynet-0.2.3/antspynet/utilities/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/custom_normalization_layers.py` & `antspynet-0.2.3/antspynet/utilities/custom_normalization_layers.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/data_augmentation.py` & `antspynet-0.2.3/antspynet/utilities/data_augmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,18 @@
         we used the first image in the input image list.
 
     transform_type : string
         One of the following options: "translation", "rigid", "scaleShear", "affine",
         "deformation", "affineAndDeformation".
 
     noise_model : string
-        'additivegaussian', 'saltandpepper', 'shot', or 'speckle'.
+        'additivegaussian', 'saltandpepper', 'shot', and 'speckle'. Alternatively, one
+        can specify a tuple or list of one or more of the options and one is selected
+        at random with reasonable, randomized parameters.  Note that the "speckle" model
+        takes much longer than the others.
 
     noise_parameters : tuple or array or float
         'additivegaussian': (mean, standardDeviation)
         'saltandpepper': (probability, saltValue, pepperValue)
         'shot': scale
         'speckle': standardDeviation
         Note that the standard deviation, scale, and probability values are *max* values
@@ -204,53 +207,68 @@
 
             image = ants.iMath(image, "Normalize")
 
             # Noise
 
             if noise_model is not None:
 
+                if not isinstance(noise_model, str):
+                    noise_model = random.sample(noise_model, 1)[0]
+                    # Just picked some parameters that looked reasonable
+                    if noise_model == "additivegaussian":
+                        noise_parameters = (random.uniform(0.0, 1.0),
+                                            random.uniform(0.01, 0.25))
+                    elif noise_model == "saltandpepper":
+                        noise_parameters = (random.uniform(0.0, 0.25),
+                                            random.uniform(0.0, 0.25),
+                                            random.uniform(0.75, 1.0))
+                    elif noise_model == "shot":
+                        noise_parameters = (random.uniform(10, 1000),)
+                    elif noise_model == "speckle":
+                        noise_parameters = (random.uniform(0.1, 1),)
+                    else:
+                        raise ValueError("Unrecognized noise model.")
+
                 if verbose:
                     print("        Adding noise (" + noise_model + ").")
 
-                if any( np.array(noise_parameters) > 0 ):
-
-                   if noise_model.lower() == "additivegaussian":
-                       parameters = (noise_parameters[0], random.uniform(0.0, noise_parameters[1]))
-                       image = ants.add_noise_to_image(image,
-                                                       noise_model="additivegaussian",
-                                                       noise_parameters=parameters)
-                   elif noise_model.lower() == "saltandpepper":
-                       parameters = (random.uniform(0.0, noise_parameters[0]), noise_parameters[1], noise_parameters[2])
-                       image = ants.add_noise_to_image(image,
-                                                       noise_model="saltandpepper",
-                                                       noise_parameters=parameters)
-                   elif noise_model.lower() == "shot":
-                       parameters = (random.uniform(0.0, noise_parameters[0]))
-                       image = ants.add_noise_to_image(image,
-                                                       noise_model="shot",
-                                                       noise_parameters=parameters)
-                   elif noise_model.lower() == "speckle":
-                       parameters = (random.uniform(0.0, noise_parameters[0]))
-                       image = ants.add_noise_to_image(image,
-                                                       noise_model="speckle",
-                                                       noise_parameters=parameters)
-                   else:
-                       raise ValueError("Unrecognized noise model.")
+                if noise_model.lower() == "additivegaussian":
+                    parameters = (noise_parameters[0], random.uniform(0.0, noise_parameters[1]))
+                    image = ants.add_noise_to_image(image,
+                                                    noise_model="additivegaussian",
+                                                    noise_parameters=parameters)
+                elif noise_model.lower() == "saltandpepper":
+                    parameters = (random.uniform(0.0, noise_parameters[0]), noise_parameters[1], noise_parameters[2])
+                    image = ants.add_noise_to_image(image,
+                                                    noise_model="saltandpepper",
+                                                    noise_parameters=parameters)
+                elif noise_model.lower() == "shot":
+                    parameters = (random.uniform(0.0, noise_parameters[0]))
+                    image = ants.add_noise_to_image(image,
+                                                    noise_model="shot",
+                                                    noise_parameters=parameters)
+                elif noise_model.lower() == "speckle":
+                    parameters = (random.uniform(0.0, noise_parameters[0]))
+                    image = ants.add_noise_to_image(image,
+                                                    noise_model="speckle",
+                                                    noise_parameters=parameters)
+                else:
+                    raise ValueError("Unrecognized noise model.")
 
             # Simulated bias field
 
             if sd_simulated_bias_field > 0:
 
                 if verbose:
                     print("        Adding simulated bias field.")
 
                 log_field = simulate_bias_field(image, number_of_points=10, sd_bias_field=sd_simulated_bias_field, number_of_fitting_levels=2, mesh_size=10)
                 log_field = log_field.iMath("Normalize")
                 field_array = np.power(np.exp(log_field.numpy()), random.sample((2, 3, 4), 1)[0])
-                image = image * ants.from_numpy(field_array, origin=image.origin, spacing=image.spacing, direction=image.direction)                
+                image = image * ants.from_numpy(field_array, origin=image.origin, spacing=image.spacing, direction=image.direction)
 
             # Histogram intensity warping
 
             if sd_histogram_warping > 0:
 
                 if verbose:
                     print("        Performing intensity histogram warping.")
```

### Comparing `antspynet-0.2.2/antspynet/utilities/deep_atropos.py` & `antspynet-0.2.3/antspynet/utilities/deep_atropos.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,17 +67,14 @@
     from ..utilities import preprocess_brain_image
     from ..utilities import extract_image_patches
     from ..utilities import reconstruct_image_from_patches
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     ################################
     #
     # Preprocess images
     #
     ################################
 
     t1_preprocessed = t1
```

### Comparing `antspynet-0.2.2/antspynet/utilities/deep_embedded_clustering_utilities.py` & `antspynet-0.2.3/antspynet/utilities/deep_embedded_clustering_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/deep_flash.py` & `antspynet-0.2.3/antspynet/utilities/deep_flash.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,31 +82,28 @@
     from ..utilities import get_pretrained_network
     from ..utilities import get_antsxnet_data
     from ..utilities import brain_extraction
 
     if t1.dimension != 3:
         raise ValueError("Image dimension must be 3.")
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     ################################
     #
     # Options temporarily taken from the user
     #
     ################################
 
     # use_hierarchical_parcellation : boolean
     #     If True, use u-net model with additional outputs of the medial temporal lobe
     #     region, hippocampal, and entorhinal/perirhinal/parahippocampal regions.  Otherwise
     #     the only additional output is the medial temporal lobe.
     #
     # use_contralaterality : boolean
     #     Use both hemispherical models to also predict the corresponding contralateral
-    #     segmentation and use both sets of priors to produce the results.  
+    #     segmentation and use both sets of priors to produce the results.
 
     use_hierarchical_parcellation = True
     use_contralaterality = True
 
     ################################
     #
     # Preprocess images
```

### Comparing `antspynet-0.2.2/antspynet/utilities/denseunet_utilities.py` & `antspynet-0.2.3/antspynet/utilities/denseunet_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/desikan_killiany_tourville_labeling.py` & `antspynet-0.2.3/antspynet/utilities/desikan_killiany_tourville_labeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,18 +246,14 @@
     from ..utilities import get_antsxnet_data
     from ..utilities import preprocess_brain_image
     from ..utilities import deep_atropos
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
-
     template_transform_type = "antsRegistrationSyNQuickRepro[a]"
     ################################
     #
     # Preprocess images
     #
     ################################
```

### Comparing `antspynet-0.2.2/antspynet/utilities/extract_image_patches.py` & `antspynet-0.2.3/antspynet/utilities/extract_image_patches.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/gaussian_diffusion_utilities.py` & `antspynet-0.2.3/antspynet/utilities/gaussian_diffusion_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/get_antsxnet_data.py` & `antspynet-0.2.3/antspynet/utilities/get_antsxnet_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             "nki": "https://ndownloader.figshare.com/files/25516355",
             "nki10": "https://ndownloader.figshare.com/files/25516346",
             "oasis": "https://ndownloader.figshare.com/files/25516352",
             "magetTemplate": "https://figshare.com/ndownloader/files/41052572",
             "magetTemplateBrainMask": "https://figshare.com/ndownloader/files/41052569",
             "magetCerebellumTemplate": "https://figshare.com/ndownloader/files/41052581",
             "magetCerebellumTemplatePriors": "https://figshare.com/ndownloader/files/41052578",
-            "magetCerebellumxTemplate0GenericAffine": "https://figshare.com/ndownloader/files/41052575"            
+            "magetCerebellumxTemplate0GenericAffine": "https://figshare.com/ndownloader/files/41052575"
         }
         return(switcher.get(argument, "Invalid argument."))
 
     if file_id == None:
         raise ValueError("Missing file id.")
 
     valid_list = ("biobank",
@@ -105,28 +105,26 @@
         raise ValueError("No data with the id you passed - try \"show\" to get list of valid ids.")
 
     if file_id == "show":
        return(valid_list)
 
     url = switch_data(file_id)
 
-    if target_file_name == None:
+    if target_file_name is None:
         if file_id == "magetCerebellumxTemplate0GenericAffine":
             target_file_name = file_id + ".mat"
         else:
             target_file_name = file_id + ".nii.gz"
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
+    if antsxnet_cache_directory is None:
+        antsxnet_cache_directory = os.path.join(os.path.expanduser('~'), ".keras/ANTsXNet")
+    target_file_name_path = os.path.join(antsxnet_cache_directory, target_file_name)
 
     # keras get_file does not work on read-only file systems. It will attempt to download the file even
     # if it exists. This is a problem for shared cache directories and read-only containers.
     #
     # Check if the file exists here, and if so, return it. Else let keras handle the download
-    target_file_name_path = os.path.join(os.path.expanduser('~'), '.keras', antsxnet_cache_directory,
-                                        target_file_name)
-
     if not os.path.exists(target_file_name_path):
         target_file_name_path = tf.keras.utils.get_file(target_file_name, url,
-                                                        cache_subdir = antsxnet_cache_directory)
+                                                        cache_subdir=antsxnet_cache_directory)
 
     return(target_file_name_path)
```

### Comparing `antspynet-0.2.2/antspynet/utilities/get_pretrained_network.py` & `antspynet-0.2.3/antspynet/utilities/get_pretrained_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             "brainExtractionRobustFA": "https://figshare.com/ndownloader/files/34870410",
             "brainExtractionNoBrainer": "https://ndownloader.figshare.com/files/22598039",
             "brainExtractionInfantT1T2": "https://ndownloader.figshare.com/files/22968833",
             "brainExtractionInfantT1": "https://ndownloader.figshare.com/files/22968836",
             "brainExtractionInfantT2": "https://ndownloader.figshare.com/files/22968830",
             "brainSegmentation": "https://ndownloader.figshare.com/files/13900010",
             "brainSegmentationPatchBased": "https://ndownloader.figshare.com/files/14249717",
-            "cerebellumWhole": "https://figshare.com/ndownloader/files/41228604",
+            "cerebellumWhole": "https://figshare.com/ndownloader/files/41460447",
             "cerebellumTissue": "https://figshare.com/ndownloader/files/41107724",
             "cerebellumLabels": "https://figshare.com/ndownloader/files/41168678",
             "claustrum_axial_0": "https://ndownloader.figshare.com/files/27844068",
             "claustrum_axial_1": "https://ndownloader.figshare.com/files/27844059",
             "claustrum_axial_2": "https://ndownloader.figshare.com/files/27844062",
             "claustrum_coronal_0": "https://ndownloader.figshare.com/files/27844074",
             "claustrum_coronal_1": "https://ndownloader.figshare.com/files/27844071",
@@ -125,14 +125,15 @@
             "koniqMBCS": "https://ndownloader.figshare.com/files/24967376",
             "koniqMS": "https://figshare.com/ndownloader/files/35295403",
             "koniqMS2": "https://figshare.com/ndownloader/files/35295397",
             "koniqMS3": "https://ndownloader.figshare.com/files/25474847",
             "lungCtWithPriorsSegmentationWeights": "https://ndownloader.figshare.com/files/28357818",
             "maskLobes": "https://figshare.com/ndownloader/files/30678458",
             "mriSuperResolution": "https://figshare.com/ndownloader/files/35290684",
+            "mriModalityClassification": "https://figshare.com/ndownloader/files/41510736",
             "protonLungMri": "https://ndownloader.figshare.com/files/13606799",
             "protonLobes": "https://figshare.com/ndownloader/files/30678455",
             "sixTissueOctantBrainSegmentation": "https://ndownloader.figshare.com/files/23776025",
             "sixTissueOctantBrainSegmentationWithPriors1": "https://ndownloader.figshare.com/files/28159869",
             "sysuMediaWmhFlairOnlyModel0": "https://ndownloader.figshare.com/files/22898441",
             "sysuMediaWmhFlairOnlyModel1": "https://ndownloader.figshare.com/files/22898570",
             "sysuMediaWmhFlairOnlyModel2": "https://ndownloader.figshare.com/files/22898438",
@@ -243,14 +244,15 @@
                   "koniqMBCS",
                   "koniqMS",
                   "koniqMS2",
                   "koniqMS3",
                   "lungCtWithPriorsSegmentationWeights",
                   "maskLobes",
                   "mriSuperResolution",
+                  "mriModalityClassification",
                   "protonLungMri",
                   "protonLobes",
                   "sixTissueOctantBrainSegmentation",
                   "sixTissueOctantBrainSegmentationWithPriors1",
                   "sixTissueOctantBrainSegmentationWithPriors2",
                   "sysuMediaWmhFlairOnlyModel0",
                   "sysuMediaWmhFlairOnlyModel1",
@@ -271,25 +273,23 @@
         raise ValueError("No data with the id you passed - try \"show\" to get list of valid ids.")
 
     if file_id == "show":
        return(valid_list)
 
     url = switch_networks(file_id)
 
-    if target_file_name == None:
+    if target_file_name is None:
         target_file_name = file_id + ".h5"
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
+    if antsxnet_cache_directory is None:
+        antsxnet_cache_directory = os.path.join(os.path.expanduser('~'), ".keras/ANTsXNet")
+    target_file_name_path = os.path.join(antsxnet_cache_directory, target_file_name)
 
     # keras get_file does not work on read-only file systems. It will attempt to download the file even
     # if it exists. This is a problem for shared cache directories and read-only containers.
     #
     # Check if the file exists here, and if so, return it. Else let keras handle the download
-    target_file_name_path = os.path.join(os.path.expanduser('~'), '.keras', antsxnet_cache_directory,
-                                        target_file_name)
-
     if not os.path.exists(target_file_name_path):
         target_file_name_path = tf.keras.utils.get_file(target_file_name, url,
-                                                        cache_subdir = antsxnet_cache_directory)
+                                                        cache_subdir=antsxnet_cache_directory)
 
     return(target_file_name_path)
```

### Comparing `antspynet-0.2.2/antspynet/utilities/hippmapp3r_segmentation.py` & `antspynet-0.2.3/antspynet/utilities/hippmapp3r_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,14 @@
     from ..utilities import preprocess_brain_image
     from ..utilities import get_pretrained_network
     from ..utilities import get_antsxnet_data
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if verbose == True:
         print("*************  Preprocessing  ***************")
         print("")
 
     t1_preprocessed = t1
     if do_preprocessing == True:
         t1_preprocessing = preprocess_brain_image(t1,
```

### Comparing `antspynet-0.2.2/antspynet/utilities/histogram_warp_image_intensities.py` & `antspynet-0.2.3/antspynet/utilities/histogram_warp_image_intensities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/histology.py` & `antspynet-0.2.3/antspynet/utilities/histology.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,14 @@
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
     if image.dimension != 2:
         raise ValueError( "Image dimension must be 2." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     channel_size = 1
 
     weights_file_name = get_pretrained_network("arterialLesionWeibinShi",
         antsxnet_cache_directory=antsxnet_cache_directory)
 
     resampled_image_size = (512, 512)
 
@@ -121,22 +118,19 @@
     -------
     >>> output = allen_e13x5_brain_extraction(histology_image)
     """
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if which_axis < 0 or which_axis > 2:
         raise ValueError("Chosen axis not supported.")
 
     weights_file_name = ""
-    if view.lower() == "coronal":  
+    if view.lower() == "coronal":
         weights_file_name = get_pretrained_network("ex5_coronal_weights",
             antsxnet_cache_directory=antsxnet_cache_directory)
     elif view.lower() == "sagittal":
         weights_file_name = get_pretrained_network("ex5_sagittal_weights",
             antsxnet_cache_directory=antsxnet_cache_directory)
     else:
         raise ValueError("Valid view options are coronal and sagittal.")
@@ -157,23 +151,23 @@
     if verbose:
         print("Preprocessing:  Resampling.")
 
     number_of_channels = image.components
     number_of_slices = 1
     if image.dimension > 2:
         number_of_slices = image.shape[which_axis]
-    
+
     image_channels = list()
     if number_of_channels == 1:
         image_channels.append(image)
     else:
         image_channels = ants.split_channels(image)
-     
+
     batch_X = np.zeros((number_of_channels * number_of_slices, *resampled_image_size, 1))
-    
+
     count = 0
     for i in range(number_of_channels):
         image_channel_array = image_channels[i].numpy()
         for j in range(number_of_slices):
             slice = None
             if image.dimension > 2:
                 if which_axis == 0:
@@ -195,27 +189,27 @@
     if verbose:
         print("Prediction: ")
 
     predicted_data = unet_model.predict(batch_X, verbose=int(verbose))
     if number_of_channels > 1:
         if verbose:
             print("Averaging across channels.")
-        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0) 
+        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0)
         predicted_data = np.zeros((number_of_slices, *resampled_image_size, 1))
         for i in range(number_of_channels):
             predicted_data = (predicted_data * i + predicted_data_temp[i]) / (i + 1)
 
     if verbose:
         print("Post-processing:  resampling to original space.")
 
     foreground_probability_array = np.zeros(image.shape)
     for j in range(number_of_slices):
         slice_resampled = ants.from_numpy(np.squeeze(predicted_data[j,:,:,1]))
         slice = ants.resample_image(slice_resampled, original_slice_shape, use_voxels=True, interp_type=0)
-        if image.dimension == 2: 
+        if image.dimension == 2:
             foreground_probability_array[:,:] = slice.numpy()
         else:
             if which_axis == 0:
                 foreground_probability_array[j,:,:] = slice.numpy()
             elif which_axis == 1:
                 foreground_probability_array[:,j,:] = slice.numpy()
             else:
@@ -262,17 +256,14 @@
     -------
     >>> output = allen_histology_brain_mask(histology_image)
     """
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if which_axis < 0 or which_axis > 2:
         raise ValueError("Chosen axis not supported.")
 
     weights_file_name = get_pretrained_network("allen_brain_mask_weights",
         antsxnet_cache_directory=antsxnet_cache_directory)
 
     resampled_image_size = (512, 512)
@@ -291,23 +282,23 @@
     if verbose:
         print("Preprocessing:  Resampling.")
 
     number_of_channels = image.components
     number_of_slices = 1
     if image.dimension > 2:
         number_of_slices = image.shape[which_axis]
-    
+
     image_channels = list()
     if number_of_channels == 1:
         image_channels.append(image)
     else:
         image_channels = ants.split_channels(image)
-     
+
     batch_X = np.zeros((number_of_channels * number_of_slices, *resampled_image_size, 1))
-    
+
     count = 0
     for i in range(number_of_channels):
         image_channel_array = image_channels[i].numpy()
         for j in range(number_of_slices):
             slice = None
             if image.dimension > 2:
                 if which_axis == 0:
@@ -329,27 +320,27 @@
     if verbose:
         print("Prediction: ")
 
     predicted_data = unet_model.predict(batch_X, verbose=int(verbose))
     if number_of_channels > 1:
         if verbose:
             print("Averaging across channels.")
-        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0) 
+        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0)
         predicted_data = np.zeros((number_of_slices, *resampled_image_size, 1))
         for i in range(number_of_channels):
             predicted_data = (predicted_data * i + predicted_data_temp[i]) / (i + 1)
 
     if verbose:
         print("Post-processing:  resampling to original space.")
 
     foreground_probability_array = np.zeros(image.shape)
     for j in range(number_of_slices):
         slice_resampled = ants.from_numpy(np.squeeze(predicted_data[j,:,:,1]))
         slice = ants.resample_image(slice_resampled, original_slice_shape, use_voxels=True, interp_type=0)
-        if image.dimension == 2: 
+        if image.dimension == 2:
             foreground_probability_array[:,:] = slice.numpy()
         else:
             if which_axis == 0:
                 foreground_probability_array[j,:,:] = slice.numpy()
             elif which_axis == 1:
                 foreground_probability_array[:,j,:] = slice.numpy()
             else:
@@ -366,15 +357,15 @@
 
 def allen_histology_hemispherical_coronal_mask(image,
                                                which_axis=2,
                                                antsxnet_cache_directory=None,
                                                verbose=False):
 
     """
-    Determine left and right hemisphere brain masks of Allen's mouse data in coronal 
+    Determine left and right hemisphere brain masks of Allen's mouse data in coronal
     acquisitions for both P* and E*x5 data.  This assumes that the original histology
     image has been pre-extracted.
 
     Arguments
     ---------
     image : ANTsImage
         input image
@@ -398,17 +389,14 @@
     -------
     >>> output = allen_histology_hemispherical_coronal_mask(histology_image)
     """
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if which_axis < 0 or which_axis > 2:
         raise ValueError("Chosen axis not supported.")
 
     weights_file_name = get_pretrained_network("allen_brain_leftright_coronal_mask_weights",
         antsxnet_cache_directory=antsxnet_cache_directory)
 
     resampled_image_size = (512, 512)
@@ -430,23 +418,23 @@
     if verbose:
         print("Preprocessing:  Resampling.")
 
     number_of_channels = image.components
     number_of_slices = 1
     if image.dimension > 2:
         number_of_slices = image.shape[which_axis]
-    
+
     image_channels = list()
     if number_of_channels == 1:
         image_channels.append(image)
     else:
         image_channels = ants.split_channels(image)
-     
+
     batch_X = np.zeros((number_of_channels * number_of_slices, *resampled_image_size, 1))
-    
+
     count = 0
     for i in range(number_of_channels):
         image_channel_array = image_channels[i].numpy()
         for j in range(number_of_slices):
             slice = None
             if image.dimension > 2:
                 if which_axis == 0:
@@ -469,15 +457,15 @@
     if verbose:
         print("Prediction: ")
 
     predicted_data = unet_model.predict(batch_X, verbose=int(verbose))
     if number_of_channels > 1:
         if verbose:
             print("Averaging across channels.")
-        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0) 
+        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0)
         predicted_data = np.zeros((number_of_slices, *resampled_image_size, 1))
         for i in range(number_of_channels):
             predicted_data = (predicted_data * i + predicted_data_temp[i]) / (i + 1)
 
     if verbose:
         print("Post-processing:  resampling to original space.")
 
@@ -490,15 +478,15 @@
         if verbose == True:
             print("Reconstructing image", classes[i])
 
         probability_image_array = np.zeros(image.shape)
         for j in range(number_of_slices):
             slice_resampled = ants.from_numpy(np.squeeze(predicted_data[j,:,:,i]))
             slice = ants.resample_image(slice_resampled, original_slice_shape, use_voxels=True, interp_type=0)
-            if image.dimension == 2: 
+            if image.dimension == 2:
                 probability_image_array[:,:] = slice.numpy()
             else:
                 if which_axis == 0:
                     probability_image_array[j,:,:] = slice.numpy()
                 elif which_axis == 1:
                     probability_image_array[:,j,:] = slice.numpy()
                 else:
@@ -550,29 +538,26 @@
     -------
     >>> output = allen_histology_cerebellum_mask(histology_image)
     """
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if which_axis < 0 or which_axis > 2:
         raise ValueError("Chosen axis not supported.")
 
     weights_file_name = None
     if view == "sagittal":
         weights_file_name = get_pretrained_network("allen_cerebellum_sagittal_mask_weights",
             antsxnet_cache_directory=antsxnet_cache_directory)
-    elif view == "coronal":   
+    elif view == "coronal":
         weights_file_name = get_pretrained_network("allen_cerebellum_coronal_mask_weights",
             antsxnet_cache_directory=antsxnet_cache_directory)
     else:
-        raise ValueError("Unrecognized option for view.  Must be sagittal or coronal.")    
+        raise ValueError("Unrecognized option for view.  Must be sagittal or coronal.")
 
     resampled_image_size = (512, 512)
     original_slice_shape = image.shape
     if image.dimension > 2:
         original_slice_shape = tuple(np.delete(np.array(image.shape), which_axis))
 
     unet_model = create_unet_model_2d((*resampled_image_size, 1),
@@ -586,23 +571,23 @@
     if verbose:
         print("Preprocessing:  Resampling.")
 
     number_of_channels = image.components
     number_of_slices = 1
     if image.dimension > 2:
         number_of_slices = image.shape[which_axis]
-    
+
     image_channels = list()
     if number_of_channels == 1:
         image_channels.append(image)
     else:
         image_channels = ants.split_channels(image)
-     
+
     batch_X = np.zeros((number_of_channels * number_of_slices, *resampled_image_size, 1))
-    
+
     count = 0
     for i in range(number_of_channels):
         image_channel_array = image_channels[i].numpy()
         for j in range(number_of_slices):
             slice = None
             if image.dimension > 2:
                 if which_axis == 0:
@@ -624,27 +609,27 @@
     if verbose:
         print("Prediction: ")
 
     predicted_data = unet_model.predict(batch_X, verbose=int(verbose))
     if number_of_channels > 1:
         if verbose:
             print("Averaging across channels.")
-        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0) 
+        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0)
         predicted_data = np.zeros((number_of_slices, *resampled_image_size, 1))
         for i in range(number_of_channels):
             predicted_data = (predicted_data * i + predicted_data_temp[i]) / (i + 1)
 
     if verbose:
         print("Post-processing:  resampling to original space.")
 
     foreground_probability_array = np.zeros(image.shape)
     for j in range(number_of_slices):
         slice_resampled = ants.from_numpy(np.squeeze(predicted_data[j,:,:,0]))
         slice = ants.resample_image(slice_resampled, original_slice_shape, use_voxels=True, interp_type=0)
-        if image.dimension == 2: 
+        if image.dimension == 2:
             foreground_probability_array[:,:] = slice.numpy()
         else:
             if which_axis == 0:
                 foreground_probability_array[j,:,:] = slice.numpy()
             elif which_axis == 1:
                 foreground_probability_array[:,j,:] = slice.numpy()
             else:
@@ -696,74 +681,71 @@
     if isinstance(image, list):
         image_list = image
     else:
         image_list.append(image)
 
     lr_image_size = (256, 256)
     sr_image_size = (512, 512)
-    
+
     image_lr_list = list()
     for i in range(len(image_list)):
 
         if image_list[i].components != 3:
             raise ValueError("Number of image channels should be 3 (rgb).")
         if image_list[i].dimension != 2:
             raise ValueError("Input image should be 2-D.")
-                
+
         do_resample = False
         if image_list[i].shape != lr_image_size:
             warnings.warn("Resampling input image to (256, 256).")
             do_resample = True
 
         image_lr = ants.image_clone(image_list[i])
         image_lr_channels = ants.split_channels(image_lr)
         for c in range(len(image_lr_channels)):
             if do_resample:
-                image_lr_channels[c] = ants.resample_image(image_lr_channels[c], resample_params=lr_image_size, 
+                image_lr_channels[c] = ants.resample_image(image_lr_channels[c], resample_params=lr_image_size,
                                                            use_voxels=True, interp_type=0)
-            image_lr_channels[c] = ((image_lr_channels[c] - image_lr_channels[c].min()) / 
+            image_lr_channels[c] = ((image_lr_channels[c] - image_lr_channels[c].min()) /
                                     (image_lr_channels[c].max() - image_lr_channels[c].min()))
         image_lr = ants.merge_channels(image_lr_channels)
         image_lr_list.append(image_lr)
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     weights_file_name = get_pretrained_network("allen_sr_weights",
         antsxnet_cache_directory=antsxnet_cache_directory)
 
     sr_model = create_deep_back_projection_network_model_2d((*lr_image_size, 3),
         number_of_outputs=3, convolution_kernel_size=(6, 6), strides=(2, 2))
     sr_model.load_weights(weights_file_name)
 
     batch_X = np.zeros((len(image_lr_list), *lr_image_size, 3))
     for i in range(len(image_lr_list)):
         batch_X[i,:,:,:] = image_lr_list[i].numpy()
-    
+
     if verbose:
         print("Prediction: ")
 
     predicted_data = sr_model.predict(batch_X, verbose=int(verbose))
-    
+
     if verbose:
         print("Regression match output image.")
 
     spacing_factor = (lr_image_size[0] - 1) / (sr_image_size[0] - 1)
-    
+
     image_sr_list = list()
     for i in range(len(image_lr_list)):
         image_sr = ants.from_numpy(predicted_data[i,:,:,:], origin=image_list[i].origin,
-                                   direction=image_list[i].direction, 
-                                   spacing=(spacing_factor * image_list[i].spacing[0], 
+                                   direction=image_list[i].direction,
+                                   spacing=(spacing_factor * image_list[i].spacing[0],
                                             spacing_factor * image_list[i].spacing[1]),
                                    has_components=True)
         image_channels = ants.split_channels(image_list[i])
         image_sr_channels = ants.split_channels(image_sr)
         for c in range(len(image_sr_channels)):
-            image_lr_channel_resampled = ants.resample_image(image_channels[c], resample_params=sr_image_size, 
+            image_lr_channel_resampled = ants.resample_image(image_channels[c], resample_params=sr_image_size,
                                                              use_voxels=True, interp_type=0)
             image_sr_channels[c] = regression_match_image(image_sr_channels[c], image_lr_channel_resampled)
         image_sr_list.append(ants.merge_channels(image_sr_channels))
 
     if isinstance(image, list):
         return(image_sr_list)
     else:
```

### Comparing `antspynet-0.2.2/antspynet/utilities/hypothalamus_segmentation.py` & `antspynet-0.2.3/antspynet/utilities/hypothalamus_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,14 @@
 
     from ..architectures import create_hypothalamus_unet_model_3d
     from ..utilities import get_pretrained_network
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     classes = ("background",
                "left anterior-inferior",
                "left anterior-superior",
                "left posterior",
                "left tubular inferior",
                "left tubular superior",
                "right anterior-inferior",
```

### Comparing `antspynet-0.2.2/antspynet/utilities/inpainting.py` & `antspynet-0.2.3/antspynet/utilities/inpainting.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,14 @@
     from ..utilities import regression_match_image
     from ..utilities import extract_image_patches
     from ..utilities import reconstruct_image_from_patches
 
     if image.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if slicewise:
 
         image_size = (256, 256)
         channel_size = 1
 
         if verbose:
             print("Preprocessing:  Reorientation.")
```

### Comparing `antspynet-0.2.2/antspynet/utilities/lung_extraction.py` & `antspynet-0.2.3/antspynet/utilities/lung_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Arguments
     ---------
     image : ANTsImage
         input image
 
     modality : string
-        Modality image type.  Options include "ct", "proton", "protonLobes", 
+        Modality image type.  Options include "ct", "proton", "protonLobes",
         "maskLobes", and "ventilation".
 
     antsxnet_cache_directory : string
         Destination directory for storing the downloaded template and model weights.
         Since these can be resused, if is None, these data will be downloaded to a
         ~/.keras/ANTsXNet/.
 
@@ -45,17 +45,14 @@
     from ..utilities import get_pretrained_network
     from ..utilities import get_antsxnet_data
     from ..utilities import pad_or_crop_image_to_size
 
     if image.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     image_mods = [modality]
     channel_size = len(image_mods)
 
     weights_file_name = None
     unet_model = None
 
     if modality == "proton":
@@ -131,15 +128,15 @@
         spatial_priors = ants.image_read(spatial_priors_file_name_path)
         priors_image_list = ants.ndimage_to_list(spatial_priors)
 
         channel_size = 1 + len(priors_image_list)
         number_of_classification_labels = 1 + len(priors_image_list)
 
         unet_model = create_unet_model_3d((*resampled_image_size, channel_size),
-            number_of_outputs=number_of_classification_labels, mode="classification", 
+            number_of_outputs=number_of_classification_labels, mode="classification",
             number_of_filters_at_base_layer=16, number_of_layers=4,
             convolution_kernel_size=(3, 3, 3), deconvolution_kernel_size=(2, 2, 2),
             dropout_rate=0.0, weight_decay=0, additional_options=("attentionGating",))
 
         if modality == "protonLobes":
             penultimate_layer = unet_model.layers[-2].output
             outputs2 = Conv3D(filters=1,
@@ -165,15 +162,15 @@
             center=np.asarray(center_of_mass_template), translation=translation)
         warped_image = ants.apply_ants_transform_to_image(xfrm, image, reorient_template)
         warped_array = warped_image.numpy()
         if modality == "protonLobes":
             warped_array = (warped_array - warped_array.mean()) / warped_array.std()
         else:
             warped_array[warped_array != 0] = 1
-       
+
         batchX = np.zeros((1, *warped_array.shape, channel_size))
         batchX[0,:,:,:,0] = warped_array
         for i in range(len(priors_image_list)):
             batchX[0,:,:,:,i+1] = priors_image_list[i].numpy()
 
         predicted_data = unet_model.predict(batchX, verbose=int(verbose))
```

### Comparing `antspynet-0.2.2/antspynet/utilities/lung_segmentation.py` & `antspynet-0.2.3/antspynet/utilities/lung_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,14 @@
 
     if ventilation_image.dimension != 3:
         raise ValueError("Image dimension must be 3.")
 
     if ventilation_image.shape != mask.shape:
         raise ValueError("Ventilation image and mask size are not the same size.")
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     ################################
     #
     # Preprocess image
     #
     ################################
 
     template_size = (256, 256)
```

### Comparing `antspynet-0.2.2/antspynet/utilities/mixture_density_utilities.py` & `antspynet-0.2.3/antspynet/utilities/mixture_density_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/mri_super_resolution.py` & `antspynet-0.2.3/antspynet/utilities/mri_super_resolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,14 @@
     from ..utilities import get_pretrained_network
     from ..utilities import apply_super_resolution_model_to_image
     from ..utilities import regression_match_image
 
     if image.dimension != 3:
         raise ValueError("Image dimension must be 3.")
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     model_and_weights_file_name = get_pretrained_network("mriSuperResolution", antsxnet_cache_directory=antsxnet_cache_directory)
     model_sr = tf.keras.models.load_model(model_and_weights_file_name, compile=False)
 
     image_sr = apply_super_resolution_model_to_image(
         image, model_sr, target_range=(-127.5, 127.5)
     )
     image_sr = regression_match_image(
```

### Comparing `antspynet-0.2.2/antspynet/utilities/neural_style_transfer.py` & `antspynet-0.2.3/antspynet/utilities/neural_style_transfer.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/preprocess_image.py` & `antspynet-0.2.3/antspynet/utilities/preprocess_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,17 +88,14 @@
 
     from ..utilities import brain_extraction
     from ..utilities import regression_match_image
     from ..utilities import get_antsxnet_data
 
     preprocessed_image = ants.image_clone(image)
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     # Truncate intensity
     if truncate_intensity is not None:
         quantiles = (image.quantile(truncate_intensity[0]), image.quantile(truncate_intensity[1]))
         if verbose == True:
             print("Preprocessing:  truncate intensities ( low =", quantiles[0], ", high =", quantiles[1], ").")
 
         preprocessed_image[image < quantiles[0]] = quantiles[0]
@@ -128,15 +125,15 @@
         if mask is None:
             registration = ants.registration(fixed=template_image, moving=preprocessed_image,
                 type_of_transform=template_transform_type, verbose=verbose)
             preprocessed_image = registration['warpedmovout']
             transforms = dict(fwdtransforms=registration['fwdtransforms'],
                               invtransforms=registration['invtransforms'])
         else:
-            template_probability_mask = brain_extraction(template_image, modality=brain_extraction_modality, 
+            template_probability_mask = brain_extraction(template_image, modality=brain_extraction_modality,
                 antsxnet_cache_directory=antsxnet_cache_directory, verbose=verbose)
             template_mask = ants.threshold_image(template_probability_mask, 0.5, 1, 1, 0)
             template_brain_image = template_mask * template_image
 
             preprocessed_brain_image = preprocessed_image * mask
 
             registration = ants.registration(fixed=template_brain_image, moving=preprocessed_brain_image,
```

### Comparing `antspynet-0.2.2/antspynet/utilities/quality_assessment.py` & `antspynet-0.2.3/antspynet/utilities/quality_assessment.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,14 @@
         tid_model = which_model # should be a tf model
         which_model = "user_defined"
 
     valid_models = ("tidsQualityAssessment", "koniqMS", "koniqMS2", "koniqMS3", "user_defined")
     if not which_model in valid_models:
         raise ValueError("Please pass valid model")
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if verbose == True:
         print("Neural QA:  retreiving model and weights.")
 
     is_koniq = "koniq" in which_model
     if which_model != "user_defined":
         model_and_weights_file_name = get_pretrained_network(which_model, antsxnet_cache_directory=antsxnet_cache_directory)
         tid_model = tf.keras.models.load_model(model_and_weights_file_name, compile=False)
```

### Comparing `antspynet-0.2.2/antspynet/utilities/randomly_transform_image_data.py` & `antspynet-0.2.3/antspynet/utilities/randomly_transform_image_data.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/reconstruct_image_from_patches.py` & `antspynet-0.2.3/antspynet/utilities/reconstruct_image_from_patches.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/regression_match_image.py` & `antspynet-0.2.3/antspynet/utilities/regression_match_image.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/resample_tensor_utilities.py` & `antspynet-0.2.3/antspynet/utilities/resample_tensor_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/simulate_bias_field.py` & `antspynet-0.2.3/antspynet/utilities/simulate_bias_field.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/spatial_transformer_network_utilities.py` & `antspynet-0.2.3/antspynet/utilities/spatial_transformer_network_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/super_resolution_utilities.py` & `antspynet-0.2.3/antspynet/utilities/super_resolution_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/ukbb.py` & `antspynet-0.2.3/antspynet/utilities/ukbb.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,14 @@
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
     if image.dimension != 2:
         raise ValueError( "Image dimension must be 2." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     channel_size = 1
 
     weights_file_name = get_pretrained_network("arterialLesionWeibinShi",
         antsxnet_cache_directory=antsxnet_cache_directory)
 
     resampled_image_size = (512, 512)
 
@@ -122,22 +119,19 @@
     -------
     >>> output = allen_e13x5_brain_extraction(histology_image)
     """
 
     from ..architectures import create_unet_model_2d
     from ..utilities import get_pretrained_network
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     if which_axis < 0 or which_axis > 2:
         raise ValueError("Chosen axis not supported.")
 
     weights_file_name = ""
-    if view.lower() == "coronal":  
+    if view.lower() == "coronal":
         weights_file_name = get_pretrained_network("e13x5_coronal_weights",
             antsxnet_cache_directory=antsxnet_cache_directory)
     elif view.lower() == "sagittal":
         weights_file_name = get_pretrained_network("e13x5_sagittal_weights",
             antsxnet_cache_directory=antsxnet_cache_directory)
     else:
         raise ValueError("Valid view options are coronal and sagittal.")
@@ -158,23 +152,23 @@
     if verbose:
         print("Preprocessing:  Resampling.")
 
     number_of_channels = image.components
     number_of_slices = 1
     if image.dimension > 2:
         number_of_slices = image.shape[which_axis]
-    
+
     image_channels = list()
     if number_of_channels == 1:
         image_channels.append(image)
     else:
         image_channels = ants.split_channels(image)
-     
+
     batch_X = np.zeros((number_of_channels * number_of_slices, *resampled_image_size, 1))
-    
+
     count = 0
     for i in range(number_of_channels):
         image_channel_array = image_channels[i].numpy()
         for j in range(number_of_slices):
             slice = None
             if image.dimension > 2:
                 if which_axis == 0:
@@ -196,27 +190,27 @@
     if verbose:
         print("Prediction: ")
 
     predicted_data = unet_model.predict(batch_X, verbose=int(verbose))
     if number_of_channels > 1:
         if verbose:
             print("Averaging across channels.")
-        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0) 
+        predicted_data_temp = np.split(predicted_data, number_of_channels, axis=0)
         predicted_data = np.zeros((number_of_slices, *resampled_image_size, 1))
         for i in range(number_of_channels):
             predicted_data = (predicted_data * i + predicted_data_temp[i]) / (i + 1)
 
     if verbose:
         print("Post-processing:  resampling to original space.")
 
     foreground_probability_array = np.zeros(image.shape)
     for j in range(number_of_slices):
         slice_resampled = ants.from_numpy(np.squeeze(predicted_data[j,:,:,1]))
         slice = ants.resample_image(slice_resampled, original_slice_shape, use_voxels=True, interp_type=0)
-        if image.dimension == 2: 
+        if image.dimension == 2:
             foreground_probability_array[:,:] = slice.numpy()
         else:
             if which_axis == 0:
                 foreground_probability_array[j,:,:] = slice.numpy()
             elif which_axis == 1:
                 foreground_probability_array[:,j,:] = slice.numpy()
             else:
```

### Comparing `antspynet-0.2.2/antspynet/utilities/unet_utilities.py` & `antspynet-0.2.3/antspynet/utilities/unet_utilities.py`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.2/antspynet/utilities/white_matter_hyperintensity_segmentation.py` & `antspynet-0.2.3/antspynet/utilities/white_matter_hyperintensity_segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,14 @@
     from ..utilities import pad_or_crop_image_to_size
     from ..utilities import preprocess_brain_image
     from ..utilities import binary_dice_coefficient
 
     if flair.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     image_size = (200, 200)
 
     ################################
     #
     # Preprocess images
     #
     ################################
@@ -316,17 +313,14 @@
     from ..architectures import create_hypermapp3r_unet_model_3d
     from ..utilities import preprocess_brain_image
     from ..utilities import get_pretrained_network
 
     if t1.dimension != 3:
         raise ValueError( "Image dimension must be 3." )
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     ################################
     #
     # Preprocess images
     #
     ################################
 
     if verbose:
@@ -518,17 +512,14 @@
             raise ValueError("Segmentation requires T1.")
         else:
             use_t1_segmentation = True
 
     if use_t1_segmentation and do_preprocessing == False:
         raise ValueError("Using the t1 segmentation requires do_preprocessing=True.")
 
-    if antsxnet_cache_directory == None:
-        antsxnet_cache_directory = "ANTsXNet"
-
     do_slicewise = True
 
     if do_slicewise == False:
 
         raise ValueError("Not available.")
 
         # ################################
```

### Comparing `antspynet-0.2.2/antspynet.egg-info/PKG-INFO` & `antspynet-0.2.3/antspynet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: antspynet
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of deep learning architectures ported to the python language and tools for basic medical image processing.
 Home-page: https://github.com/ANTsX/ANTsPyNet
 Author: Nicholas J. Tustison and Brian B. Avants and Nick Cullen
 Author-email: ntustison@gmail.com
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.md
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)
+[![PubMed](https://img.shields.io/badge/ANTsX_paper-Open_Access-8DABFF?logo=pubmed)](https://pubmed.ncbi.nlm.nih.gov/33907199/)
 
 # ANTsPyNet
 
 A collection of deep learning architectures and applications ported to the python language and tools for basic medical image processing. Based on `keras` and `tensorflow` with cross-compatibility with our R analog [ANTsRNet](https://github.com/ANTsX/ANTsRNet/).
 
 Documentation page [https://antsx.github.io/ANTsPyNet/](https://antsx.github.io/ANTsPyNet/).
 
@@ -89,14 +90,15 @@
 * [Sysu white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/30125711/)
 * [HyperMapp3r white matter hyperintensity segmentation](https://pubmed.ncbi.nlm.nih.gov/35088930/)
 * [Hypothalamus segmentation](https://pubmed.ncbi.nlm.nih.gov/32853816/)
 * [Claustrum segmentation](https://arxiv.org/abs/2008.03465)
 * [Deep Flash](https://www.medrxiv.org/content/10.1101/2023.01.17.23284693v1)
 * Desikan-Killiany-Tourville cortical labeling
 * Cerebellum segmentation, parcellation, and thickness
+* MRI modality classification
 * Lung extraction
     * [Proton](https://www.ncbi.nlm.nih.gov/pubmed/30195415)
     * CT
 * [Functional lung segmentation](https://www.medrxiv.org/content/10.1101/2021.03.04.21252588v2)
 * [Neural style transfer](https://arxiv.org/abs/1508.06576)
 * Image quality assessment
     * [TID2013](https://www.sciencedirect.com/science/article/pii/S0923596514001490)
```

### Comparing `antspynet-0.2.2/antspynet.egg-info/SOURCES.txt` & `antspynet-0.2.3/antspynet.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 antspynet/architectures/create_improved_wasserstein_gan_model.py
 antspynet/architectures/create_partial_convolution_unet_model.py
 antspynet/architectures/create_resnet_model.py
 antspynet/architectures/create_resnet_super_resolution_model.py
 antspynet/architectures/create_resunet_model.py
 antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py
 antspynet/architectures/create_super_resolution_gan_model.py
+antspynet/architectures/create_transformer_model.py
 antspynet/architectures/create_unet_model.py
 antspynet/architectures/create_vanilla_gan_model.py
 antspynet/architectures/create_vgg_model.py
 antspynet/architectures/create_wasserstein_gan_model.py
 antspynet/architectures/create_wide_resnet_model.py
 antspynet/utilities/__init__.py
 antspynet/utilities/attention_utilities.py
@@ -63,21 +64,23 @@
 antspynet/utilities/histogram_warp_image_intensities.py
 antspynet/utilities/histology.py
 antspynet/utilities/hypothalamus_segmentation.py
 antspynet/utilities/inpainting.py
 antspynet/utilities/lung_extraction.py
 antspynet/utilities/lung_segmentation.py
 antspynet/utilities/mixture_density_utilities.py
+antspynet/utilities/mri_modality_classification.py
 antspynet/utilities/mri_super_resolution.py
 antspynet/utilities/neural_style_transfer.py
 antspynet/utilities/preprocess_image.py
 antspynet/utilities/quality_assessment.py
 antspynet/utilities/randomly_transform_image_data.py
 antspynet/utilities/reconstruct_image_from_patches.py
 antspynet/utilities/regression_match_image.py
 antspynet/utilities/resample_tensor_utilities.py
 antspynet/utilities/simulate_bias_field.py
 antspynet/utilities/spatial_transformer_network_utilities.py
 antspynet/utilities/super_resolution_utilities.py
+antspynet/utilities/transformer_utilities.py
 antspynet/utilities/ukbb.py
 antspynet/utilities/unet_utilities.py
 antspynet/utilities/white_matter_hyperintensity_segmentation.py
```

