# Comparing `tmp/dingo-gw-0.5.8.tar.gz` & `tmp/dingo-gw-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingo-gw-0.5.8.tar", last modified: Wed Dec  6 12:07:13 2023, max compression
+gzip compressed data, was "dingo-gw-0.5.9.tar", last modified: Mon Dec 11 13:10:43 2023, max compression
```

## Comparing `dingo-gw-0.5.8.tar` & `dingo-gw-0.5.9.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.046543 dingo-gw-0.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.006543 dingo-gw-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.014543 dingo-gw-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-12-06 12:07:13.046543 dingo-gw-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.014543 dingo-gw-0.5.8/compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/remove_domain_window_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_model_input_dims.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_saved_model_for_train_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_saved_model_gnpe_context_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_saved_model_new_gnpe.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_saved_model_new_truncation.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/compatibility/update_waveform_dataset_svd_refactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.014543 dingo-gw-0.5.8/dingo/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-06 12:07:12.000000 dingo-gw-0.5.8/dingo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.014543 dingo-gw-0.5.8/dingo/asimov/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/asimov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/asimov/asimov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/asimov/dingo.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.014543 dingo-gw-0.5.8/dingo/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.018543 dingo-gw-0.5.8/dingo/core/density/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/density/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/density/nde_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/density/unconditional_density_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.018543 dingo-gw-0.5.8/dingo/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16789 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/models/posterior_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.018543 dingo-gw-0.5.8/dingo/core/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/nn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14095 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/nn/enets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14037 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/nn/nsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25730 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    21593 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.018543 dingo-gw-0.5.8/dingo/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/condor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/gnpeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/pt_to_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/torchutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8031 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/core/utils/trainutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.022543 dingo-gw-0.5.8/dingo/gw/
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/SVD.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.022543 dingo-gw-0.5.8/dingo/gw/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/conversion/spin_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.022543 dingo-gw-0.5.8/dingo/gw/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/data/data_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/data/data_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/data/event_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.022543 dingo-gw-0.5.8/dingo/gw/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/dataset/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/dataset/generate_dataset_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/dataset/waveform_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21281 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/download_strain_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/gwutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.022543 dingo-gw-0.5.8/dingo/gw/importance_sampling/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/importance_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/importance_sampling/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/importance_sampling/importance_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.022543 dingo-gw-0.5.8/dingo/gw/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/inference/gw_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/inference/inference_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/inference/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31426 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/ls_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.026543 dingo-gw-0.5.8/dingo/gw/noise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/asd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/asd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/generate_dataset_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.026543 dingo-gw-0.5.8/dingo/gw/noise/synthetic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/synthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/synthetic/asd_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/synthetic/asd_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/synthetic/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/synthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/noise/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)    25645 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/temporary_debug_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.026543 dingo-gw-0.5.8/dingo/gw/training/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/training/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12587 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/training/train_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/training/train_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/training/train_pipeline_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.026543 dingo-gw-0.5.8/dingo/gw/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15842 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/detector_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/general_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/gnpe_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/inference_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/noise_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/transforms/parameter_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.030543 dingo-gw-0.5.8/dingo/gw/waveform_generator/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/waveform_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/waveform_generator/frame_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    60998 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/waveform_generator/waveform_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/gw/waveform_generator/wfg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.030543 dingo-gw-0.5.8/dingo/pipe/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/ACKNOWLEDGMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/dag_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/dingo_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    13305 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.034543 dingo-gw-0.5.8/dingo/pipe/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/generation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/importance_sampling_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/merge_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/pe_summary_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/plot_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/nodes/sampling_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    46302 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/dingo/pipe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.046543 dingo-gw-0.5.8/dingo_gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-12-06 12:07:12.000000 dingo-gw-0.5.8/dingo_gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2023-12-06 12:07:13.000000 dingo-gw-0.5.8/dingo_gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 12:07:12.000000 dingo-gw-0.5.8/dingo_gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-06 12:07:12.000000 dingo-gw-0.5.8/dingo_gw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-12-06 12:07:12.000000 dingo-gw-0.5.8/dingo_gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-06 12:07:12.000000 dingo-gw-0.5.8/dingo_gw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.034543 dingo-gw-0.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.038543 dingo-gw-0.5.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/code_design.md
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/dingo_pipe.md
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/example_gnpe_model.md
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/example_injection.md
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/example_npe_model.md
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/example_toy_npe_model.md
--rw-r--r--   0 runner    (1001) docker     (127)    42481 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/generating_waveforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30150 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/gibbs_figure.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/gnpe.md
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/inference.md
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/network_architecture.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12693 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/noise_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/overview.md
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/result.md
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/sbi.md
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/training.md
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/training_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26097 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/docs/source/waveform_dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.038543 dingo-gw-0.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.038543 dingo-gw-0.5.8/examples/dataset_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/dataset_generation/asd_dataset_settings_synthetic.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.038543 dingo-gw-0.5.8/examples/gnpe_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/gnpe_model/GW150914.ini
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/gnpe_model/asd_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/gnpe_model/asd_dataset_settings_fiducial.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/gnpe_model/train_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/gnpe_model/train_settings_init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/gnpe_model/waveform_dataset_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.038543 dingo-gw-0.5.8/examples/misc/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/misc/is_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/misc/stage_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.042543 dingo-gw-0.5.8/examples/npe_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/npe_model/GW150914.ini
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/npe_model/asd_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/npe_model/asd_dataset_settings_fiducial.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/npe_model/train_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/npe_model/waveform_dataset_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.042543 dingo-gw-0.5.8/examples/toy_npe_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/toy_npe_model/GW150914.ini
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/toy_npe_model/asd_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/toy_npe_model/train_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/examples/toy_npe_model/waveform_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 12:07:13.046543 dingo-gw-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.010543 dingo-gw-0.5.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.042543 dingo-gw-0.5.8/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/core/test_enets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/core/test_nsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/core/test_posterior_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/core/testutils_enets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.042543 dingo-gw-0.5.8/tests/gw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.042543 dingo-gw-0.5.8/tests/gw/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/conversion/test_spin_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/conversion/test_time_delay_from_geocenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/test_noise_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/test_prior_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/test_waveform_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.042543 dingo-gw-0.5.8/tests/gw/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/transforms/test_detector_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/transforms/test_general_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/transforms/test_gnpe_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/transforms/test_parameter_transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   263605 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/transforms/waveform_data.npy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 12:07:13.046543 dingo-gw-0.5.8/tests/gw/waveform_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/waveform_generator/test_wfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2023-12-06 12:07:00.000000 dingo-gw-0.5.8/tests/gw/waveform_generator/test_wfg_m.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.886969 dingo-gw-0.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.846969 dingo-gw-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.854969 dingo-gw-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2023-12-11 13:10:43.886969 dingo-gw-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.854969 dingo-gw-0.5.9/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/remove_domain_window_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_model_input_dims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_saved_model_for_train_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_saved_model_gnpe_context_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_saved_model_new_gnpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_saved_model_new_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/compatibility/update_waveform_dataset_svd_refactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.854969 dingo-gw-0.5.9/dingo/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.854969 dingo-gw-0.5.9/dingo/asimov/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/asimov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/asimov/asimov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/asimov/dingo.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.854969 dingo-gw-0.5.9/dingo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.858969 dingo-gw-0.5.9/dingo/core/density/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/density/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/density/nde_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/density/unconditional_density_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.858969 dingo-gw-0.5.9/dingo/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16789 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/models/posterior_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.858969 dingo-gw-0.5.9/dingo/core/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/nn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14095 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/nn/enets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14037 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/nn/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25730 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21593 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.858969 dingo-gw-0.5.9/dingo/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/condor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/gnpeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/pt_to_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/torchutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/core/utils/trainutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.862969 dingo-gw-0.5.9/dingo/gw/
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/SVD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.862969 dingo-gw-0.5.9/dingo/gw/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/conversion/spin_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.862969 dingo-gw-0.5.9/dingo/gw/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/data/data_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/data/data_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/data/event_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.862969 dingo-gw-0.5.9/dingo/gw/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/dataset/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/dataset/generate_dataset_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/dataset/waveform_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21281 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/download_strain_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/gwutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.862969 dingo-gw-0.5.9/dingo/gw/importance_sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/importance_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/importance_sampling/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/importance_sampling/importance_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.862969 dingo-gw-0.5.9/dingo/gw/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/inference/gw_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/inference/inference_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/inference/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31426 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/ls_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.866969 dingo-gw-0.5.9/dingo/gw/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/asd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/asd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/generate_dataset_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.866969 dingo-gw-0.5.9/dingo/gw/noise/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/synthetic/asd_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/synthetic/asd_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/synthetic/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/synthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/noise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25645 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/temporary_debug_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.866969 dingo-gw-0.5.9/dingo/gw/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/training/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12587 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/training/train_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/training/train_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/training/train_pipeline_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.866969 dingo-gw-0.5.9/dingo/gw/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15842 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/detector_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/general_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/gnpe_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/inference_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/noise_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/transforms/parameter_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.870969 dingo-gw-0.5.9/dingo/gw/waveform_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/waveform_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/waveform_generator/frame_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60998 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/waveform_generator/waveform_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/gw/waveform_generator/wfg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.870969 dingo-gw-0.5.9/dingo/pipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/ACKNOWLEDGMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/dag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/dingo_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.870969 dingo-gw-0.5.9/dingo/pipe/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/importance_sampling_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/merge_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/pe_summary_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/plot_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/nodes/sampling_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46302 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/dingo/pipe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.886969 dingo-gw-0.5.9/dingo_gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo_gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo_gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo_gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo_gw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo_gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-11 13:10:43.000000 dingo-gw-0.5.9/dingo_gw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.874969 dingo-gw-0.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.878969 dingo-gw-0.5.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/code_design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/dingo_pipe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/example_gnpe_model.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/example_injection.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/example_npe_model.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/example_toy_npe_model.md
+-rw-r--r--   0 runner    (1001) docker     (127)    42481 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/generating_waveforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30150 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/gibbs_figure.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/gnpe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/inference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/network_architecture.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12693 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/noise_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/overview.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/result.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/sbi.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/training.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/training_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26097 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/docs/source/waveform_dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.878969 dingo-gw-0.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.878969 dingo-gw-0.5.9/examples/dataset_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/dataset_generation/asd_dataset_settings_synthetic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.878969 dingo-gw-0.5.9/examples/gnpe_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/gnpe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/gnpe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/gnpe_model/asd_dataset_settings_fiducial.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/gnpe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/gnpe_model/train_settings_init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/gnpe_model/waveform_dataset_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.882969 dingo-gw-0.5.9/examples/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/misc/is_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/misc/stage_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.882969 dingo-gw-0.5.9/examples/npe_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/npe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/npe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/npe_model/asd_dataset_settings_fiducial.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/npe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/npe_model/waveform_dataset_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.882969 dingo-gw-0.5.9/examples/toy_npe_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/toy_npe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/toy_npe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/toy_npe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/examples/toy_npe_model/waveform_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 13:10:43.886969 dingo-gw-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.850969 dingo-gw-0.5.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.882969 dingo-gw-0.5.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/core/test_enets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/core/test_nsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/core/test_posterior_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/core/testutils_enets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.882969 dingo-gw-0.5.9/tests/gw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.882969 dingo-gw-0.5.9/tests/gw/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/conversion/test_spin_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/conversion/test_time_delay_from_geocenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/test_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/test_noise_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/test_prior_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/test_waveform_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.886969 dingo-gw-0.5.9/tests/gw/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/transforms/test_detector_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/transforms/test_general_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/transforms/test_gnpe_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/transforms/test_parameter_transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   263605 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/transforms/waveform_data.npy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:10:43.886969 dingo-gw-0.5.9/tests/gw/waveform_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/waveform_generator/test_wfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2023-12-11 13:10:31.000000 dingo-gw-0.5.9/tests/gw/waveform_generator/test_wfg_m.py
```

### Comparing `dingo-gw-0.5.8/.github/workflows/python-publish.yml` & `dingo-gw-0.5.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/.readthedocs.yaml` & `dingo-gw-0.5.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/LICENSE` & `dingo-gw-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/PKG-INFO` & `dingo-gw-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingo-gw
-Version: 0.5.8
+Version: 0.5.9
 Summary: Deep inference for gravitational-wave observations
 Author-email: Maximilian Dax <maximilian.dax@tuebingen.mpg.de>, Stephen Green <Stephen.Green2@nottingham.ac.uk>
 License: MIT
 Project-URL: homepage, https://github.com/dingo-gw/dingo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: astropy
 Requires-Dist: bilby
-Requires-Dist: bilby_pipe>=1.2.1
+Requires-Dist: bilby_pipe>=1.3
 Requires-Dist: configargparse
 Requires-Dist: corner
 Requires-Dist: glasflow
 Requires-Dist: gwpy
 Requires-Dist: h5py
 Requires-Dist: lalsuite>=7.15
 Requires-Dist: matplotlib
```

### Comparing `dingo-gw-0.5.8/README.md` & `dingo-gw-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/remove_domain_window_factor.py` & `dingo-gw-0.5.9/compatibility/remove_domain_window_factor.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/update_model_input_dims.py` & `dingo-gw-0.5.9/compatibility/update_model_input_dims.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/update_model_metadata.py` & `dingo-gw-0.5.9/compatibility/update_model_metadata.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/update_saved_model_for_train_stages.py` & `dingo-gw-0.5.9/compatibility/update_saved_model_for_train_stages.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/update_saved_model_gnpe_context_names.py` & `dingo-gw-0.5.9/compatibility/update_saved_model_gnpe_context_names.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/update_saved_model_new_gnpe.py` & `dingo-gw-0.5.9/compatibility/update_saved_model_new_gnpe.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/compatibility/update_saved_model_new_truncation.py` & `dingo-gw-0.5.9/compatibility/update_saved_model_new_truncation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/asimov/asimov.py` & `dingo-gw-0.5.9/dingo/asimov/asimov.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/asimov/dingo.ini` & `dingo-gw-0.5.9/dingo/asimov/dingo.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/dataset.py` & `dingo-gw-0.5.9/dingo/core/dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/density/interpolation.py` & `dingo-gw-0.5.9/dingo/core/density/interpolation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/density/nde_settings.py` & `dingo-gw-0.5.9/dingo/core/density/nde_settings.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/density/unconditional_density_estimation.py` & `dingo-gw-0.5.9/dingo/core/density/unconditional_density_estimation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/likelihood.py` & `dingo-gw-0.5.9/dingo/core/likelihood.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/models/posterior_model.py` & `dingo-gw-0.5.9/dingo/core/models/posterior_model.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/multiprocessing.py` & `dingo-gw-0.5.9/dingo/core/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/nn/enets.py` & `dingo-gw-0.5.9/dingo/core/nn/enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/nn/nsf.py` & `dingo-gw-0.5.9/dingo/core/nn/nsf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/result.py` & `dingo-gw-0.5.9/dingo/core/result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/samplers.py` & `dingo-gw-0.5.9/dingo/core/samplers.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/condor_utils.py` & `dingo-gw-0.5.9/dingo/core/utils/condor_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/gnpeutils.py` & `dingo-gw-0.5.9/dingo/core/utils/gnpeutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/logging_utils.py` & `dingo-gw-0.5.9/dingo/core/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/misc.py` & `dingo-gw-0.5.9/dingo/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/plotting.py` & `dingo-gw-0.5.9/dingo/core/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/pt_to_hdf5.py` & `dingo-gw-0.5.9/dingo/core/utils/pt_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/torchutils.py` & `dingo-gw-0.5.9/dingo/core/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/core/utils/trainutils.py` & `dingo-gw-0.5.9/dingo/core/utils/trainutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/SVD.py` & `dingo-gw-0.5.9/dingo/gw/SVD.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/conversion/spin_conversion.py` & `dingo-gw-0.5.9/dingo/gw/conversion/spin_conversion.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/data/data_download.py` & `dingo-gw-0.5.9/dingo/gw/data/data_download.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/data/data_preparation.py` & `dingo-gw-0.5.9/dingo/gw/data/data_preparation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/dataset/generate_dataset.py` & `dingo-gw-0.5.9/dingo/gw/dataset/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/dataset/generate_dataset_dag.py` & `dingo-gw-0.5.9/dingo/gw/dataset/generate_dataset_dag.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/dataset/utils.py` & `dingo-gw-0.5.9/dingo/gw/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/dataset/waveform_dataset.py` & `dingo-gw-0.5.9/dingo/gw/dataset/waveform_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/domains.py` & `dingo-gw-0.5.9/dingo/gw/domains.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/download_strain_data.py` & `dingo-gw-0.5.9/dingo/gw/download_strain_data.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/gwutils.py` & `dingo-gw-0.5.9/dingo/gw/gwutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/importance_sampling/diagnostics.py` & `dingo-gw-0.5.9/dingo/gw/importance_sampling/diagnostics.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/importance_sampling/importance_weights.py` & `dingo-gw-0.5.9/dingo/gw/importance_sampling/importance_weights.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/inference/gw_samplers.py` & `dingo-gw-0.5.9/dingo/gw/inference/gw_samplers.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/inference/inference_pipeline.py` & `dingo-gw-0.5.9/dingo/gw/inference/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/inference/visualization.py` & `dingo-gw-0.5.9/dingo/gw/inference/visualization.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/injection.py` & `dingo-gw-0.5.9/dingo/gw/injection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/likelihood.py` & `dingo-gw-0.5.9/dingo/gw/likelihood.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/ls_cli.py` & `dingo-gw-0.5.9/dingo/gw/ls_cli.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/asd_dataset.py` & `dingo-gw-0.5.9/dingo/gw/noise/asd_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/asd_estimation.py` & `dingo-gw-0.5.9/dingo/gw/noise/asd_estimation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/generate_dataset.py` & `dingo-gw-0.5.9/dingo/gw/noise/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/generate_dataset_dag.py` & `dingo-gw-0.5.9/dingo/gw/noise/generate_dataset_dag.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/synthetic/asd_parameterization.py` & `dingo-gw-0.5.9/dingo/gw/noise/synthetic/asd_parameterization.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/synthetic/asd_sampling.py` & `dingo-gw-0.5.9/dingo/gw/noise/synthetic/asd_sampling.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/synthetic/generate_dataset.py` & `dingo-gw-0.5.9/dingo/gw/noise/synthetic/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/synthetic/utils.py` & `dingo-gw-0.5.9/dingo/gw/noise/synthetic/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/noise/utils.py` & `dingo-gw-0.5.9/dingo/gw/noise/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/prior.py` & `dingo-gw-0.5.9/dingo/gw/prior.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/result.py` & `dingo-gw-0.5.9/dingo/gw/result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/temporary_debug_utils.py` & `dingo-gw-0.5.9/dingo/gw/temporary_debug_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/training/train_builders.py` & `dingo-gw-0.5.9/dingo/gw/training/train_builders.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/training/train_pipeline.py` & `dingo-gw-0.5.9/dingo/gw/training/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/training/train_pipeline_condor.py` & `dingo-gw-0.5.9/dingo/gw/training/train_pipeline_condor.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/training/utils.py` & `dingo-gw-0.5.9/dingo/gw/training/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/transforms/detector_transforms.py` & `dingo-gw-0.5.9/dingo/gw/transforms/detector_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/transforms/gnpe_transforms.py` & `dingo-gw-0.5.9/dingo/gw/transforms/gnpe_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/transforms/inference_transforms.py` & `dingo-gw-0.5.9/dingo/gw/transforms/inference_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/transforms/noise_transforms.py` & `dingo-gw-0.5.9/dingo/gw/transforms/noise_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/transforms/parameter_transforms.py` & `dingo-gw-0.5.9/dingo/gw/transforms/parameter_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/waveform_generator/frame_utils.py` & `dingo-gw-0.5.9/dingo/gw/waveform_generator/frame_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/waveform_generator/waveform_generator.py` & `dingo-gw-0.5.9/dingo/gw/waveform_generator/waveform_generator.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/gw/waveform_generator/wfg_utils.py` & `dingo-gw-0.5.9/dingo/gw/waveform_generator/wfg_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/dag_creator.py` & `dingo-gw-0.5.9/dingo/pipe/dag_creator.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/data_generation.py` & `dingo-gw-0.5.9/dingo/pipe/data_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,18 @@
 
         if create_data:
             # Added for dingo so that create_data runs. TODO: enable injections
             args.injection = False
             args.injection_numbers = None
             args.injection_file = None
             args.injection_dict = None
-            args.gaussian_noise = False
             args.injection_waveform_arguments = None
+            args.injection_frequency_domain_source_model = None
+            self.frequency_domain_source_model = None
+            self.gaussian_noise = False
 
             self.create_data(args)
 
     def save_hdf5(self):
         """Save frequency-domain strain and ASDs as DingoDataset HDF5 format."""
 
         # PSD and strain data.
```

### Comparing `dingo-gw-0.5.8/dingo/pipe/default_settings.py` & `dingo-gw-0.5.9/dingo/pipe/default_settings.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/dingo_result.py` & `dingo-gw-0.5.9/dingo/pipe/dingo_result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/importance_sampling.py` & `dingo-gw-0.5.9/dingo/pipe/importance_sampling.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/main.py` & `dingo-gw-0.5.9/dingo/pipe/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         self.accounting_user = args.accounting_user
         # self.sampler = args.sampler
         self.detectors = args.detectors
         self.coherence_test = (
             False  # dingo mod: Cannot use different sets of detectors.
         )
         self.data_dict = args.data_dict
+        self.channel_dict = args.channel_dict
         self.frame_type_dict = args.frame_type_dict
         self.data_find_url = args.data_find_url
         self.data_find_urltype = args.data_find_urltype
         self.n_parallel = args.n_parallel
         self.transfer_files = args.transfer_files
         self.additional_transfer_paths = args.additional_transfer_paths
         self.osg = args.osg
@@ -167,16 +168,16 @@
 
         # self.ignore_gwpy_data_quality_check = args.ignore_gwpy_data_quality_check
         self.trigger_time = args.trigger_time
         # self.deltaT = args.deltaT
         self.gps_tuple = args.gps_tuple
         self.gps_file = args.gps_file
         self.timeslide_file = args.timeslide_file
-        # self.gaussian_noise = args.gaussian_noise
-        # self.zero_noise = args.zero_noise
+        self.gaussian_noise = False  # DINGO MOD: Cannot use different noise types.
+        self.zero_noise = False  # DINGO MOD: does not support zero noise yet
         # self.n_simulation = args.n_simulation
         #
         # self.injection = args.injection
         # self.injection_numbers = args.injection_numbers
         self.injection_file = args.injection_file
         # self.injection_dict = args.injection_dict
         # self.injection_waveform_arguments = args.injection_waveform_arguments
```

### Comparing `dingo-gw-0.5.8/dingo/pipe/nodes/generation_node.py` & `dingo-gw-0.5.9/dingo/pipe/nodes/generation_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/nodes/importance_sampling_node.py` & `dingo-gw-0.5.9/dingo/pipe/nodes/importance_sampling_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/nodes/merge_node.py` & `dingo-gw-0.5.9/dingo/pipe/nodes/merge_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/nodes/pe_summary_node.py` & `dingo-gw-0.5.9/dingo/pipe/nodes/pe_summary_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/nodes/plot_node.py` & `dingo-gw-0.5.9/dingo/pipe/nodes/plot_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/nodes/sampling_node.py` & `dingo-gw-0.5.9/dingo/pipe/nodes/sampling_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/parser.py` & `dingo-gw-0.5.9/dingo/pipe/parser.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/plot.py` & `dingo-gw-0.5.9/dingo/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo/pipe/sampling.py` & `dingo-gw-0.5.9/dingo/pipe/sampling.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo_gw.egg-info/PKG-INFO` & `dingo-gw-0.5.9/dingo_gw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingo-gw
-Version: 0.5.8
+Version: 0.5.9
 Summary: Deep inference for gravitational-wave observations
 Author-email: Maximilian Dax <maximilian.dax@tuebingen.mpg.de>, Stephen Green <Stephen.Green2@nottingham.ac.uk>
 License: MIT
 Project-URL: homepage, https://github.com/dingo-gw/dingo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: astropy
 Requires-Dist: bilby
-Requires-Dist: bilby_pipe>=1.2.1
+Requires-Dist: bilby_pipe>=1.3
 Requires-Dist: configargparse
 Requires-Dist: corner
 Requires-Dist: glasflow
 Requires-Dist: gwpy
 Requires-Dist: h5py
 Requires-Dist: lalsuite>=7.15
 Requires-Dist: matplotlib
```

### Comparing `dingo-gw-0.5.8/dingo_gw.egg-info/SOURCES.txt` & `dingo-gw-0.5.9/dingo_gw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/dingo_gw.egg-info/entry_points.txt` & `dingo-gw-0.5.9/dingo_gw.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/Makefile` & `dingo-gw-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/README.md` & `dingo-gw-0.5.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/make.bat` & `dingo-gw-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/code_design.md` & `dingo-gw-0.5.9/docs/source/code_design.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/conf.py` & `dingo-gw-0.5.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/dingo_pipe.md` & `dingo-gw-0.5.9/docs/source/dingo_pipe.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/example_gnpe_model.md` & `dingo-gw-0.5.9/docs/source/example_gnpe_model.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/example_injection.md` & `dingo-gw-0.5.9/docs/source/example_injection.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/example_npe_model.md` & `dingo-gw-0.5.9/docs/source/example_npe_model.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/example_toy_npe_model.md` & `dingo-gw-0.5.9/docs/source/example_toy_npe_model.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/generating_waveforms.ipynb` & `dingo-gw-0.5.9/docs/source/generating_waveforms.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/gibbs_figure.jpg` & `dingo-gw-0.5.9/docs/source/gibbs_figure.jpg`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/gnpe.md` & `dingo-gw-0.5.9/docs/source/gnpe.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/index.md` & `dingo-gw-0.5.9/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/inference.md` & `dingo-gw-0.5.9/docs/source/inference.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/installation.md` & `dingo-gw-0.5.9/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/network_architecture.ipynb` & `dingo-gw-0.5.9/docs/source/network_architecture.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/noise_dataset.ipynb` & `dingo-gw-0.5.9/docs/source/noise_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/overview.md` & `dingo-gw-0.5.9/docs/source/overview.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/quickstart.md` & `dingo-gw-0.5.9/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/refs.bib` & `dingo-gw-0.5.9/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/result.md` & `dingo-gw-0.5.9/docs/source/result.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/sbi.md` & `dingo-gw-0.5.9/docs/source/sbi.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/training.md` & `dingo-gw-0.5.9/docs/source/training.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/training_transforms.ipynb` & `dingo-gw-0.5.9/docs/source/training_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/docs/source/waveform_dataset.ipynb` & `dingo-gw-0.5.9/docs/source/waveform_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/README.md` & `dingo-gw-0.5.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/dataset_generation/asd_dataset_settings_synthetic.yaml` & `dingo-gw-0.5.9/examples/dataset_generation/asd_dataset_settings_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/gnpe_model/GW150914.ini` & `dingo-gw-0.5.9/examples/gnpe_model/GW150914.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/gnpe_model/asd_dataset_settings.yaml` & `dingo-gw-0.5.9/examples/gnpe_model/asd_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/gnpe_model/train_settings.yaml` & `dingo-gw-0.5.9/examples/gnpe_model/train_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/gnpe_model/train_settings_init.yaml` & `dingo-gw-0.5.9/examples/gnpe_model/train_settings_init.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/gnpe_model/waveform_dataset_settings.yaml` & `dingo-gw-0.5.9/examples/gnpe_model/waveform_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/misc/is_settings.yaml` & `dingo-gw-0.5.9/examples/misc/is_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/npe_model/GW150914.ini` & `dingo-gw-0.5.9/examples/npe_model/GW150914.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/npe_model/asd_dataset_settings.yaml` & `dingo-gw-0.5.9/examples/npe_model/asd_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/npe_model/train_settings.yaml` & `dingo-gw-0.5.9/examples/npe_model/train_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/npe_model/waveform_dataset_settings.yaml` & `dingo-gw-0.5.9/examples/npe_model/waveform_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/toy_npe_model/GW150914.ini` & `dingo-gw-0.5.9/examples/toy_npe_model/GW150914.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/toy_npe_model/asd_dataset_settings.yaml` & `dingo-gw-0.5.9/examples/toy_npe_model/asd_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/toy_npe_model/train_settings.yaml` & `dingo-gw-0.5.9/examples/toy_npe_model/train_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/examples/toy_npe_model/waveform_dataset_settings.yaml` & `dingo-gw-0.5.9/examples/toy_npe_model/waveform_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/pyproject.toml` & `dingo-gw-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
     "astropy",
     "bilby",
-    "bilby_pipe>=1.2.1",
+    "bilby_pipe>=1.3",
     "configargparse",
     "corner",
     "glasflow",
     "gwpy",
     "h5py",
     "lalsuite>=7.15",
     "matplotlib",
```

### Comparing `dingo-gw-0.5.8/tests/core/test_enets.py` & `dingo-gw-0.5.9/tests/core/test_enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/core/test_nsf.py` & `dingo-gw-0.5.9/tests/core/test_nsf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/core/test_posterior_model.py` & `dingo-gw-0.5.9/tests/core/test_posterior_model.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/core/testutils_enets.py` & `dingo-gw-0.5.9/tests/core/testutils_enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/conversion/test_spin_conversion.py` & `dingo-gw-0.5.9/tests/gw/conversion/test_spin_conversion.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/conversion/test_time_delay_from_geocenter.py` & `dingo-gw-0.5.9/tests/gw/conversion/test_time_delay_from_geocenter.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/test_domains.py` & `dingo-gw-0.5.9/tests/gw/test_domains.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/test_injection.py` & `dingo-gw-0.5.9/tests/gw/test_injection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/test_noise_dataset.py` & `dingo-gw-0.5.9/tests/gw/test_noise_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/test_prior_split.py` & `dingo-gw-0.5.9/tests/gw/test_prior_split.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/test_waveform_dataset.py` & `dingo-gw-0.5.9/tests/gw/test_waveform_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/transforms/test_detector_projection.py` & `dingo-gw-0.5.9/tests/gw/transforms/test_detector_projection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/transforms/test_gnpe_transforms.py` & `dingo-gw-0.5.9/tests/gw/transforms/test_gnpe_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/transforms/test_parameter_transforms.py` & `dingo-gw-0.5.9/tests/gw/transforms/test_parameter_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/transforms/waveform_data.npy` & `dingo-gw-0.5.9/tests/gw/transforms/waveform_data.npy`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/waveform_generator/test_wfg.py` & `dingo-gw-0.5.9/tests/gw/waveform_generator/test_wfg.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.8/tests/gw/waveform_generator/test_wfg_m.py` & `dingo-gw-0.5.9/tests/gw/waveform_generator/test_wfg_m.py`

 * *Files identical despite different names*

