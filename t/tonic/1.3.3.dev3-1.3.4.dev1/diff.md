# Comparing `tmp/tonic-1.3.3.dev3.tar.gz` & `tmp/tonic-1.3.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.3.3.dev3.tar", last modified: Mon Jul 10 22:53:03 2023, max compression
+gzip compressed data, was "tonic-1.3.4.dev1.tar", last modified: Wed Jul 12 22:52:43 2023, max compression
```

## Comparing `tonic-1.3.3.dev3.tar` & `tonic-1.3.4.dev1.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.746700 tonic-1.3.3.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.714700 tonic-1.3.3.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.718700 tonic-1.3.3.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    40083 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-10 22:53:03.746700 tonic-1.3.3.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.718700 tonic-1.3.3.dev3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.722700 tonic-1.3.3.dev3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.722700 tonic-1.3.3.dev3/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.722700 tonic-1.3.3.dev3/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.726700 tonic-1.3.3.dev3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.726700 tonic-1.3.3.dev3/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.726700 tonic-1.3.3.dev3/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.726700 tonic-1.3.3.dev3/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.730700 tonic-1.3.3.dev3/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.730700 tonic-1.3.3.dev3/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.730700 tonic-1.3.3.dev3/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.730700 tonic-1.3.3.dev3/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.730700 tonic-1.3.3.dev3/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.730700 tonic-1.3.3.dev3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-10 22:53:03.746700 tonic-1.3.3.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.734700 tonic-1.3.3.dev3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.734700 tonic-1.3.3.dev3/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.738700 tonic-1.3.3.dev3/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.742700 tonic-1.3.3.dev3/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.742700 tonic-1.3.3.dev3/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.746700 tonic-1.3.3.dev3/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.746700 tonic-1.3.3.dev3/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.746700 tonic-1.3.3.dev3/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    37426 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-07-10 22:52:39.000000 tonic-1.3.3.dev3/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:53:03.738700 tonic-1.3.3.dev3/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 22:53:03.000000 tonic-1.3.3.dev3/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.463929 tonic-1.3.4.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    40197 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.467929 tonic-1.3.4.dev1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.471929 tonic-1.3.4.dev1/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.471929 tonic-1.3.4.dev1/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.471929 tonic-1.3.4.dev1/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.471929 tonic-1.3.4.dev1/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.471929 tonic-1.3.4.dev1/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.471929 tonic-1.3.4.dev1/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.475929 tonic-1.3.4.dev1/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.475929 tonic-1.3.4.dev1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-12 22:52:43.487929 tonic-1.3.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.475929 tonic-1.3.4.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.479929 tonic-1.3.4.dev1/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.479929 tonic-1.3.4.dev1/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.483929 tonic-1.3.4.dev1/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37426 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-07-12 22:52:20.000000 tonic-1.3.4.dev1/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:43.479929 tonic-1.3.4.dev1/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 22:52:43.000000 tonic-1.3.4.dev1/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.3.3.dev3/.github/workflows/ci-pipeline.yml` & `tonic-1.3.4.dev1/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/AUTHORS` & `tonic-1.3.4.dev1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/ChangeLog` & `tonic-1.3.4.dev1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+* add ms\_to\_idx to DSEC data
+
+v1.3.3
+------
+
+* use numpy struct to unstruct function for timesurface generation
 * try/catch case where DAVIS dataset doesn't have optitrack targets
 * update plot\_animation fn
 * update plot\_animation fn
 
 v1.3.2
 ------
```

### Comparing `tonic-1.3.3.dev3/LICENSE.txt` & `tonic-1.3.4.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/PKG-INFO` & `tonic-1.3.4.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.3.3.dev3
+Version: 1.3.4.dev1
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.3.3.dev3/README.md` & `tonic-1.3.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/Makefile` & `tonic-1.3.4.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/event-cameras/eventstream.png` & `tonic-1.3.4.dev1/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/event-cameras/framestream.png` & `tonic-1.3.4.dev1/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.3.4.dev1/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.3.4.dev1/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/snn/neuron-models.png` & `tonic-1.3.4.dev1/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/snn/surrogates.png` & `tonic-1.3.4.dev1/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/tonic-logo-black.png` & `tonic-1.3.4.dev1/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/tonic-logo-white.png` & `tonic-1.3.4.dev1/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/_static/tonic_favicon.png` & `tonic-1.3.4.dev1/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/about/info.rst` & `tonic-1.3.4.dev1/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/about/prototype.rst` & `tonic-1.3.4.dev1/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/about/release_notes.rst` & `tonic-1.3.4.dev1/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/conf.py` & `tonic-1.3.4.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/datasets.rst` & `tonic-1.3.4.dev1/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.3.4.dev1/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/representations/plot_toframe.py` & `tonic-1.3.4.dev1/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/representations/plot_toimage.py` & `tonic-1.3.4.dev1/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_decimation.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_denoise.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_downsample.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.3.4.dev1/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/getting_involved/communication_channels.rst` & `tonic-1.3.4.dev1/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/getting_involved/contribute.rst` & `tonic-1.3.4.dev1/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/getting_started/install.rst` & `tonic-1.3.4.dev1/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/getting_started/nmnist.ipynb` & `tonic-1.3.4.dev1/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.3.4.dev1/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/how-tos/visualizing-data.ipynb` & `tonic-1.3.4.dev1/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.3.4.dev1/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/index.md` & `tonic-1.3.4.dev1/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/make.bat` & `tonic-1.3.4.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/reading_material/design_choices.rst` & `tonic-1.3.4.dev1/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/reading_material/intro-event-cameras.rst` & `tonic-1.3.4.dev1/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/reading_material/intro-snns.rst` & `tonic-1.3.4.dev1/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/reading_material/training-snns.rst` & `tonic-1.3.4.dev1/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/transformations.rst` & `tonic-1.3.4.dev1/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/tutorials/batching.ipynb` & `tonic-1.3.4.dev1/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/tutorials/davis_data.ipynb` & `tonic-1.3.4.dev1/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.3.4.dev1/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/tutorials/large_datasets.ipynb` & `tonic-1.3.4.dev1/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/docs/tutorials/slicing.ipynb` & `tonic-1.3.4.dev1/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/setup.cfg` & `tonic-1.3.4.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/dataset_utils.py` & `tonic-1.3.4.dev1/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/prototype_dataset_utils.py` & `tonic-1.3.4.dev1/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_audio_transforms.py` & `tonic-1.3.4.dev1/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_caching.py` & `tonic-1.3.4.dev1/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_chained_transforms.py` & `tonic-1.3.4.dev1/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_data/sample.aedat4` & `tonic-1.3.4.dev1/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_data/sample_ncars.dat` & `tonic-1.3.4.dev1/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_data/sample_nmnist.bin` & `tonic-1.3.4.dev1/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_data/sample_stmnist.mat` & `tonic-1.3.4.dev1/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_datasets.py` & `tonic-1.3.4.dev1/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_dsec.py` & `tonic-1.3.4.dev1/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_io.py` & `tonic-1.3.4.dev1/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_prototype_datasets.py` & `tonic-1.3.4.dev1/test/test_prototype_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_representations.py` & `tonic-1.3.4.dev1/test/test_representations.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_sliced_dataset.py` & `tonic-1.3.4.dev1/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_slicers.py` & `tonic-1.3.4.dev1/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_tonic_utils.py` & `tonic-1.3.4.dev1/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/test_transforms.py` & `tonic-1.3.4.dev1/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/test/utils.py` & `tonic-1.3.4.dev1/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/audio_transforms.py` & `tonic-1.3.4.dev1/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/cached_dataset.py` & `tonic-1.3.4.dev1/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/collation.py` & `tonic-1.3.4.dev1/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/dataset.py` & `tonic-1.3.4.dev1/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/__init__.py` & `tonic-1.3.4.dev1/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/asl_dvs.py` & `tonic-1.3.4.dev1/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/cifar10dvs.py` & `tonic-1.3.4.dev1/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/davisdataset.py` & `tonic-1.3.4.dev1/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/dsec.py` & `tonic-1.3.4.dev1/tonic/datasets/dsec.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,22 +243,24 @@
         base_folder = os.path.join(self.location_on_system, recording)
 
         data_tuple = []
         for data_name in self.data_selection:
             full_base_folder = os.path.join(base_folder, data_name)
             if data_name in ["events_left", "events_right"]:
                 with h5py.File(full_base_folder + "/events.h5", "r") as file:
-                    data = make_structured_array(
+                    data = {}
+                    data[data_name] = make_structured_array(
                         file["events"]["x"][()],
                         file["events"]["y"][()],
                         file["events"]["t"][()],
                         file["events"]["p"][()],
                         dtype=self.dtype,
                     )
-                    data["t"] += file["t_offset"][()]
+                    data[data_name]["t"] += file["t_offset"][()]
+                    data["ms_to_idx"] = file["ms_to_idx"][()]
 
             elif "images" in data_name:
                 images_rectified_filenames = sorted(
                     list_files(full_base_folder, ".png", prefix=True)
                 )
                 data = np.stack(
                     [np.array(Image.open(file)) for file in images_rectified_filenames]
```

### Comparing `tonic-1.3.3.dev3/tonic/datasets/dvs_lips.py` & `tonic-1.3.4.dev1/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/dvsgesture.py` & `tonic-1.3.4.dev1/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/hsd.py` & `tonic-1.3.4.dev1/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/mvsec.py` & `tonic-1.3.4.dev1/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/ncaltech101.py` & `tonic-1.3.4.dev1/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/nmnist.py` & `tonic-1.3.4.dev1/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/pokerdvs.py` & `tonic-1.3.4.dev1/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/s_mnist.py` & `tonic-1.3.4.dev1/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/tum_vie.py` & `tonic-1.3.4.dev1/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/datasets/visual_place_recognition.py` & `tonic-1.3.4.dev1/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/download_utils.py` & `tonic-1.3.4.dev1/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/__init__.py` & `tonic-1.3.4.dev1/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/crop.py` & `tonic-1.3.4.dev1/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/decimate.py` & `tonic-1.3.4.dev1/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/denoise.py` & `tonic-1.3.4.dev1/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/drop_event.py` & `tonic-1.3.4.dev1/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/drop_pixel.py` & `tonic-1.3.4.dev1/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/refractory_period.py` & `tonic-1.3.4.dev1/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/spatial_jitter.py` & `tonic-1.3.4.dev1/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/time_jitter.py` & `tonic-1.3.4.dev1/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/time_skew.py` & `tonic-1.3.4.dev1/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/to_averaged_timesurface.py` & `tonic-1.3.4.dev1/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/to_bina_rep.py` & `tonic-1.3.4.dev1/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/to_frame.py` & `tonic-1.3.4.dev1/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/to_timesurface.py` & `tonic-1.3.4.dev1/tonic/functional/to_timesurface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Tuple
 
 import numpy as np
+from numpy.lib import recfunctions as rfn
 
 from tonic.slicers import slice_events_by_time
 
 
 def to_timesurface_numpy(
     events,
     sensor_size: Tuple[int, int, int],
@@ -37,15 +38,15 @@
     x_index = event_slices[0].dtype.names.index("x")
     y_index = event_slices[0].dtype.names.index("y")
     p_index = event_slices[0].dtype.names.index("p")
     t_index = event_slices[0].dtype.names.index("t")
     start_t = event_slices[0][0][t_index]
     for i, slice in enumerate(event_slices):
         # structured to unstructured in order to access the indices
-        slice = slice.view((int, len(slice.dtype.names)))
+        slice = rfn.structured_to_unstructured(slice, dtype=int)
         indices = slice[:, [p_index, y_index, x_index]].T
         timestamps = slice[:, t_index]
         memory[tuple(indices)] = timestamps
         diff = -((i + 1) * dt + start_t - memory)
         surf = np.exp(diff / tau)
         all_surfaces.append(surf)
     return np.array(all_surfaces)
```

### Comparing `tonic-1.3.3.dev3/tonic/functional/to_voxel_grid.py` & `tonic-1.3.4.dev1/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/functional/uniform_noise.py` & `tonic-1.3.4.dev1/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/io.py` & `tonic-1.3.4.dev1/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/README.md` & `tonic-1.3.4.dev1/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/datasets/ncars.py` & `tonic-1.3.4.dev1/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/datasets/nmnist.py` & `tonic-1.3.4.dev1/tonic/prototype/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/datasets/prophesee.py` & `tonic-1.3.4.dev1/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/datasets/stmnist.py` & `tonic-1.3.4.dev1/tonic/prototype/datasets/stmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.3.4.dev1/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.3.4.dev1/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/prototype/slicers.py` & `tonic-1.3.4.dev1/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/sliced_dataset.py` & `tonic-1.3.4.dev1/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/slicers.py` & `tonic-1.3.4.dev1/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/transforms.py` & `tonic-1.3.4.dev1/tonic/transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic/utils.py` & `tonic-1.3.4.dev1/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic-logo-padded.png` & `tonic-1.3.4.dev1/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.3.dev3/tonic.egg-info/PKG-INFO` & `tonic-1.3.4.dev1/tonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.3.3.dev3
+Version: 1.3.4.dev1
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.3.3.dev3/tonic.egg-info/SOURCES.txt` & `tonic-1.3.4.dev1/tonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

