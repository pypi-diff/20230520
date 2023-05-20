# Comparing `tmp/GANDLF-0.0.1620230518.tar.gz` & `tmp/GANDLF-0.0.17.dev20230520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.1620230518.tar", last modified: Thu May 18 03:13:09 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230520.tar", last modified: Sat May 20 03:12:51 2023, max compression
```

## Comparing `GANDLF-0.0.1620230518.tar` & `GANDLF-0.0.17.dev20230520.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.356665 GANDLF-0.0.1620230518/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.296664 GANDLF-0.0.1620230518/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.296664 GANDLF-0.0.1620230518/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.304664 GANDLF-0.0.1620230518/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.304664 GANDLF-0.0.1620230518/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.308664 GANDLF-0.0.1620230518/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.308664 GANDLF-0.0.1620230518/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.312665 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.312665 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.312665 GANDLF-0.0.1620230518/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.316665 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.320665 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.320665 GANDLF-0.0.1620230518/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.324665 GANDLF-0.0.1620230518/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.324665 GANDLF-0.0.1620230518/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.340665 GANDLF-0.0.1620230518/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.348665 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.352665 GANDLF-0.0.1620230518/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.352665 GANDLF-0.0.1620230518/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.356665 GANDLF-0.0.1620230518/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 03:13:01.000000 GANDLF-0.0.1620230518/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:13:09.296664 GANDLF-0.0.1620230518/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-18 03:13:09.000000 GANDLF-0.0.1620230518/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-18 03:13:09.000000 GANDLF-0.0.1620230518/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:13:09.000000 GANDLF-0.0.1620230518/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:10:37.000000 GANDLF-0.0.1620230518/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 03:13:09.000000 GANDLF-0.0.1620230518/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 03:13:09.000000 GANDLF-0.0.1620230518/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-18 03:13:09.356665 GANDLF-0.0.1620230518/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:13:09.356665 GANDLF-0.0.1620230518/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-18 03:10:19.000000 GANDLF-0.0.1620230518/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.518996 GANDLF-0.0.17.dev20230520/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.470996 GANDLF-0.0.17.dev20230520/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.474996 GANDLF-0.0.17.dev20230520/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.478996 GANDLF-0.0.17.dev20230520/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.482996 GANDLF-0.0.17.dev20230520/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.482996 GANDLF-0.0.17.dev20230520/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.486996 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.486996 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.486996 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.486996 GANDLF-0.0.17.dev20230520/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.490996 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.494996 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.494996 GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.494996 GANDLF-0.0.17.dev20230520/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.498996 GANDLF-0.0.17.dev20230520/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.506996 GANDLF-0.0.17.dev20230520/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.510996 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.514996 GANDLF-0.0.17.dev20230520/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.514996 GANDLF-0.0.17.dev20230520/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.518996 GANDLF-0.0.17.dev20230520/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 03:12:44.000000 GANDLF-0.0.17.dev20230520/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:12:51.474996 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-20 03:12:51.000000 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-20 03:12:51.000000 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 03:12:51.000000 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 03:10:37.000000 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-20 03:12:51.000000 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 03:12:51.000000 GANDLF-0.0.17.dev20230520/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-20 03:12:51.518996 GANDLF-0.0.17.dev20230520/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 03:12:51.518996 GANDLF-0.0.17.dev20230520/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-20 03:10:20.000000 GANDLF-0.0.17.dev20230520/setup.py
```

### Comparing `GANDLF-0.0.1620230518/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230520/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230520/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230520/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230520/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230520/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230520/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230520/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230520/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230520/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230520/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230520/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230520/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230520/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230520/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230520/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230520/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230520/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230520/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230520/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230520/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230520/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230520/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230520/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230520/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230520/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230520/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230520/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230520/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230520/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230520/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230520/GANDLF.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.1620230518
+Version: 0.0.17.dev20230520
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 
 <p align="center">
   <a href="https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml" alt="Build Status"><img src="https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml/badge.svg" /></a>
   <a href="https://github.com/mlcommons/GaNDLF/actions/workflows/codeql-analysis.yml" alt="Code Analysis"><img src="https://github.com/mlcommons/GaNDLF/workflows/CodeQL/badge.svg" /></a>
   <a href="https://hub.docker.com/repository/docker/cbica/gandlf" alt="Docker CI"><img src="https://github.com/mlcommons/GaNDLF/actions/workflows/docker-image.yml/badge.svg" /></a>
   <a href="https://codecov.io/gh/mlcommons/GaNDLF" alt="Code Coverage"><img src="https://codecov.io/gh/mlcommons/GaNDLF/branch/master/graph/badge.svg?token=4I54XEI3WE" /></a>
   <a href="https://app.codacy.com/gh/mlcommons/GaNDLF?utm_source=github.com&utm_medium=referral&utm_content=mlcommons/GaNDLF&utm_campaign=Badge_Grade_Settings"><img alt="Codacy" src="https://api.codacy.com/project/badge/Grade/b2cf27ddce1b4907abb47a82931dcbca"></a><br>
-  <a href="https://anaconda.org/conda-forge/gandlf" alt="Install"><img src="https://img.shields.io/conda/vn/conda-forge/gandlf" /></a>
+  <a href="https://pypi.org/project/GANDLF/" alt="Install"><img src="https://img.shields.io/pypi/v/gandlf" /></a>
   <a href="https://github.com/mlcommons/GaNDLF/discussions" alt="Issues"><img src="https://img.shields.io/badge/Support-Discussion-blue" /></a>
   <a href="https://arxiv.org/abs/2103.01006" alt="Citation"><img src="https://img.shields.io/badge/Cite-citation-lightblue" /></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/Code%20Style-black-000000.svg"></a>
 </p>
 
 The **G**ener**a**lly **N**uanced **D**eep **L**earning **F**ramework for segmentation, regression and classification.
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.1620230518 Summary: PyTorch-
-based framework that handles segmentation/regression/classification using
-various DL architectures for medical imaging. Author: MLCommons Author-email:
-gandlf@mlcommons.org License: Apache-2.0 Keywords:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230520 Summary:
+PyTorch-based framework that handles segmentation/regression/classification
+using various DL architectures for medical imaging. Author: MLCommons Author-
+email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Scientific/Engineering :: Medical Science Apps. Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # GaNDLF
     [https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml/
  badge.svg] [https://github.com/mlcommons/GaNDLF/workflows/CodeQL/badge.svg]
    [https://github.com/mlcommons/GaNDLF/actions/workflows/docker-image.yml/
     badge.svg] [https://codecov.io/gh/mlcommons/GaNDLF/branch/master/graph/
                      badge.svg?token=4I54XEI3WE] [Codacy]
- [https://img.shields.io/conda/vn/conda-forge/gandlf] [https://img.shields.io/
-  badge/Support-Discussion-blue] [https://img.shields.io/badge/Cite-citation-
-                        lightblue] [Code_style:_black]
+ [https://img.shields.io/pypi/v/gandlf] [https://img.shields.io/badge/Support-
+ Discussion-blue] [https://img.shields.io/badge/Cite-citation-lightblue] [Code
+                                 style:_black]
 The **G**ener**a**lly **N**uanced **D**eep **L**earning **F**ramework for
 segmentation, regression and classification.
                              [GaNDLF all options]
 ## Why use this? - Supports multiple - Deep Learning model architectures - Data
 dimensions (2D/3D) - Channels/images/sequences - Prediction classes - Domain
 modalities (i.e., Radiology Scans and Digitized Histopathology Tissue Sections)
 - Problem types (segmentation, regression, classification) - Multi-GPU (on same
```

### Comparing `GANDLF-0.0.1620230518/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230520/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/HISTORY.md` & `GANDLF-0.0.17.dev20230520/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## 0.0.17
+
+
 ## 0.0.16
 - Added a script "gandlf_deploy", allowing deployment of models into MLCubes (currently requires Docker)
 - ImageNet pre-trained models for UNet with variable encoders is now available
 - ACS/Soft conversion is available for ImageNet-pretrained UNet
 - Updated links, copyright and email to MLCommons
 - Allowing provision for user to generate multiple configurations for experimentation
 - Added ability to combine classification inference results from different architectures
```

### Comparing `GANDLF-0.0.1620230518/LICENSE` & `GANDLF-0.0.17.dev20230520/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/PKG-INFO` & `GANDLF-0.0.17.dev20230520/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.1620230518
+Version: 0.0.17.dev20230520
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 
 <p align="center">
   <a href="https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml" alt="Build Status"><img src="https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml/badge.svg" /></a>
   <a href="https://github.com/mlcommons/GaNDLF/actions/workflows/codeql-analysis.yml" alt="Code Analysis"><img src="https://github.com/mlcommons/GaNDLF/workflows/CodeQL/badge.svg" /></a>
   <a href="https://hub.docker.com/repository/docker/cbica/gandlf" alt="Docker CI"><img src="https://github.com/mlcommons/GaNDLF/actions/workflows/docker-image.yml/badge.svg" /></a>
   <a href="https://codecov.io/gh/mlcommons/GaNDLF" alt="Code Coverage"><img src="https://codecov.io/gh/mlcommons/GaNDLF/branch/master/graph/badge.svg?token=4I54XEI3WE" /></a>
   <a href="https://app.codacy.com/gh/mlcommons/GaNDLF?utm_source=github.com&utm_medium=referral&utm_content=mlcommons/GaNDLF&utm_campaign=Badge_Grade_Settings"><img alt="Codacy" src="https://api.codacy.com/project/badge/Grade/b2cf27ddce1b4907abb47a82931dcbca"></a><br>
-  <a href="https://anaconda.org/conda-forge/gandlf" alt="Install"><img src="https://img.shields.io/conda/vn/conda-forge/gandlf" /></a>
+  <a href="https://pypi.org/project/GANDLF/" alt="Install"><img src="https://img.shields.io/pypi/v/gandlf" /></a>
   <a href="https://github.com/mlcommons/GaNDLF/discussions" alt="Issues"><img src="https://img.shields.io/badge/Support-Discussion-blue" /></a>
   <a href="https://arxiv.org/abs/2103.01006" alt="Citation"><img src="https://img.shields.io/badge/Cite-citation-lightblue" /></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/Code%20Style-black-000000.svg"></a>
 </p>
 
 The **G**ener**a**lly **N**uanced **D**eep **L**earning **F**ramework for segmentation, regression and classification.
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.1620230518 Summary: PyTorch-
-based framework that handles segmentation/regression/classification using
-various DL architectures for medical imaging. Author: MLCommons Author-email:
-gandlf@mlcommons.org License: Apache-2.0 Keywords:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230520 Summary:
+PyTorch-based framework that handles segmentation/regression/classification
+using various DL architectures for medical imaging. Author: MLCommons Author-
+email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Scientific/Engineering :: Medical Science Apps. Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # GaNDLF
     [https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml/
  badge.svg] [https://github.com/mlcommons/GaNDLF/workflows/CodeQL/badge.svg]
    [https://github.com/mlcommons/GaNDLF/actions/workflows/docker-image.yml/
     badge.svg] [https://codecov.io/gh/mlcommons/GaNDLF/branch/master/graph/
                      badge.svg?token=4I54XEI3WE] [Codacy]
- [https://img.shields.io/conda/vn/conda-forge/gandlf] [https://img.shields.io/
-  badge/Support-Discussion-blue] [https://img.shields.io/badge/Cite-citation-
-                        lightblue] [Code_style:_black]
+ [https://img.shields.io/pypi/v/gandlf] [https://img.shields.io/badge/Support-
+ Discussion-blue] [https://img.shields.io/badge/Cite-citation-lightblue] [Code
+                                 style:_black]
 The **G**ener**a**lly **N**uanced **D**eep **L**earning **F**ramework for
 segmentation, regression and classification.
                              [GaNDLF all options]
 ## Why use this? - Supports multiple - Deep Learning model architectures - Data
 dimensions (2D/3D) - Channels/images/sequences - Prediction classes - Domain
 modalities (i.e., Radiology Scans and Digitized Histopathology Tissue Sections)
 - Problem types (segmentation, regression, classification) - Multi-GPU (on same
```

### Comparing `GANDLF-0.0.1620230518/README.md` & `GANDLF-0.0.17.dev20230520/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <p align="center">
   <a href="https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml" alt="Build Status"><img src="https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml/badge.svg" /></a>
   <a href="https://github.com/mlcommons/GaNDLF/actions/workflows/codeql-analysis.yml" alt="Code Analysis"><img src="https://github.com/mlcommons/GaNDLF/workflows/CodeQL/badge.svg" /></a>
   <a href="https://hub.docker.com/repository/docker/cbica/gandlf" alt="Docker CI"><img src="https://github.com/mlcommons/GaNDLF/actions/workflows/docker-image.yml/badge.svg" /></a>
   <a href="https://codecov.io/gh/mlcommons/GaNDLF" alt="Code Coverage"><img src="https://codecov.io/gh/mlcommons/GaNDLF/branch/master/graph/badge.svg?token=4I54XEI3WE" /></a>
   <a href="https://app.codacy.com/gh/mlcommons/GaNDLF?utm_source=github.com&utm_medium=referral&utm_content=mlcommons/GaNDLF&utm_campaign=Badge_Grade_Settings"><img alt="Codacy" src="https://api.codacy.com/project/badge/Grade/b2cf27ddce1b4907abb47a82931dcbca"></a><br>
-  <a href="https://anaconda.org/conda-forge/gandlf" alt="Install"><img src="https://img.shields.io/conda/vn/conda-forge/gandlf" /></a>
+  <a href="https://pypi.org/project/GANDLF/" alt="Install"><img src="https://img.shields.io/pypi/v/gandlf" /></a>
   <a href="https://github.com/mlcommons/GaNDLF/discussions" alt="Issues"><img src="https://img.shields.io/badge/Support-Discussion-blue" /></a>
   <a href="https://arxiv.org/abs/2103.01006" alt="Citation"><img src="https://img.shields.io/badge/Cite-citation-lightblue" /></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/Code%20Style-black-000000.svg"></a>
 </p>
 
 The **G**ener**a**lly **N**uanced **D**eep **L**earning **F**ramework for segmentation, regression and classification.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # GaNDLF
     [https://github.com/mlcommons/GaNDLF/actions/workflows/python-test.yml/
  badge.svg] [https://github.com/mlcommons/GaNDLF/workflows/CodeQL/badge.svg]
    [https://github.com/mlcommons/GaNDLF/actions/workflows/docker-image.yml/
     badge.svg] [https://codecov.io/gh/mlcommons/GaNDLF/branch/master/graph/
                      badge.svg?token=4I54XEI3WE] [Codacy]
- [https://img.shields.io/conda/vn/conda-forge/gandlf] [https://img.shields.io/
-  badge/Support-Discussion-blue] [https://img.shields.io/badge/Cite-citation-
-                        lightblue] [Code_style:_black]
+ [https://img.shields.io/pypi/v/gandlf] [https://img.shields.io/badge/Support-
+ Discussion-blue] [https://img.shields.io/badge/Cite-citation-lightblue] [Code
+                                 style:_black]
 The **G**ener**a**lly **N**uanced **D**eep **L**earning **F**ramework for
 segmentation, regression and classification.
                              [GaNDLF all options]
 ## Why use this? - Supports multiple - Deep Learning model architectures - Data
 dimensions (2D/3D) - Channels/images/sequences - Prediction classes - Domain
 modalities (i.e., Radiology Scans and Digitized Histopathology Tissue Sections)
 - Problem types (segmentation, regression, classification) - Multi-GPU (on same
```

### Comparing `GANDLF-0.0.1620230518/SECURITY.md` & `GANDLF-0.0.17.dev20230520/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230520/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_collectStats` & `GANDLF-0.0.17.dev20230520/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230520/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230520/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_deploy` & `GANDLF-0.0.17.dev20230520/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230520/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230520/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_preprocess` & `GANDLF-0.0.17.dev20230520/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230520/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_run` & `GANDLF-0.0.17.dev20230520/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230520/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.1620230518/setup.py` & `GANDLF-0.0.17.dev20230520/setup.py`

 * *Files identical despite different names*

