# Comparing `tmp/audio_upscaler-0.0.7.tar.gz` & `tmp/audio_upscaler-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_upscaler-0.0.7.tar", last modified: Thu May  9 18:09:12 2024, max compression
+gzip compressed data, was "audio_upscaler-0.0.8.tar", last modified: Thu May  9 18:24:11 2024, max compression
```

## Comparing `audio_upscaler-0.0.7.tar` & `audio_upscaler-0.0.8.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.810790 audio_upscaler-0.0.7/
--rw-rw-rw-   0        0        0     1092 2024-04-26 20:27:22.000000 audio_upscaler-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4637 2024-05-09 18:09:12.809790 audio_upscaler-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2024-04-26 20:27:22.000000 audio_upscaler-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.720296 audio_upscaler-0.0.7/audio_upscaler/
--rw-rw-rw-   0        0        0       34 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.724802 audio_upscaler-0.0.7/audio_upscaler/clap/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.739593 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/
--rw-rw-rw-   0        0        0      664 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/__init__.py
--rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-rw-   0        0        0    11261 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/factory.py
--rw-rw-rw-   0        0        0     7369 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/feature_fusion.py
--rw-rw-rw-   0        0        0    49373 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/htsat.py
--rw-rw-rw-   0        0        0    16493 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/loss.py
--rw-rw-rw-   0        0        0    33855 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.756724 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json
--rw-rw-rw-   0        0        0      520 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-10.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14.json
--rw-rw-rw-   0        0        0      517 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-6.json
--rw-rw-rw-   0        0        0      409 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/RN101-quickgelu.json
--rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/RN101.json
--rw-rw-rw-   0        0        0      411 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/RN50-quickgelu.json
--rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/RN50.json
--rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/RN50x16.json
--rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/RN50x4.json
--rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/ViT-B-16.json
--rw-rw-rw-   0        0        0      334 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/ViT-B-32.json
--rw-rw-rw-   0        0        0      311 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/ViT-L-14.json
--rw-rw-rw-   0        0        0     5179 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/openai.py
--rw-rw-rw-   0        0        0    24066 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/pann_model.py
--rw-rw-rw-   0        0        0     6607 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/pretrained.py
--rw-rw-rw-   0        0        0     4444 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/timm_model.py
--rw-rw-rw-   0        0        0     6597 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/tokenizer.py
--rw-rw-rw-   0        0        0     1096 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/transform.py
--rw-rw-rw-   0        0        0    12319 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.762215 audio_upscaler-0.0.7/audio_upscaler/clap/training/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/training/__init__.py
--rw-rw-rw-   0        0        0    84448 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/training/audioset_textmap.npy
--rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz
--rw-rw-rw-   0        0        0    30558 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/training/data.py
--rw-rw-rw-   0        0        0    17765 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/clap/training/params.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.765215 audio_upscaler-0.0.7/audio_upscaler/hifigan/
--rw-rw-rw-   0        0        0      238 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/hifigan/__init__.py
--rw-rw-rw-   0        0        0     5698 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/hifigan/models.py
--rw-rw-rw-   0        0        0    13214 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/hifigan/models_v2.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.766718 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.769843 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/__init__.py
--rw-rw-rw-   0        0        0    17996 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/ddim.py
--rw-rw-rw-   0        0        0    62623 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/ddpm.py
--rw-rw-rw-   0        0        0    13215 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/plms.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.772849 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/__init__.py
--rw-rw-rw-   0        0        0    16226 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/attention.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.774847 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/
--rw-rw-rw-   0        0        0     5542 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/__init__.py
--rw-rw-rw-   0        0        0    21730 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py
--rw-rw-rw-   0        0        0     7927 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.783845 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/
--rw-rw-rw-   0        0        0     1406 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py
--rw-rw-rw-   0        0        0     1991 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py
--rw-rw-rw-   0        0        0     2086 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py
--rw-rw-rw-   0        0        0     2521 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py
--rw-rw-rw-   0        0        0      913 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py
--rw-rw-rw-   0        0        0    14970 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py
--rw-rw-rw-   0        0        0     4508 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py
--rw-rw-rw-   0        0        0     8838 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py
--rw-rw-rw-   0        0        0     2335 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.786348 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/__init__.py
--rw-rw-rw-   0        0        0    35533 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py
--rw-rw-rw-   0        0        0    41338 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rw-rw-rw-   0        0        0    10172 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.788353 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/distributions/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/distributions/__init__.py
--rw-rw-rw-   0        0        0     3199 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/distributions/distributions.py
--rw-rw-rw-   0        0        0     3148 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/ema.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.790352 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/encoders/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/encoders/__init__.py
--rw-rw-rw-   0        0        0    26015 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/encoders/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.793810 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/__init__.py
--rw-rw-rw-   0        0        0    15296 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py
--rw-rw-rw-   0        0        0     5121 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py
--rw-rw-rw-   0        0        0     1652 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.796735 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/
--rw-rw-rw-   0        0        0     1695 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py
--rw-rw-rw-   0        0        0     3229 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py
--rw-rw-rw-   0        0        0      651 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py
--rw-rw-rw-   0        0        0     8084 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.798740 audio_upscaler-0.0.7/audio_upscaler/latent_encoder/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_encoder/__init__.py
--rw-rw-rw-   0        0        0    11648 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/latent_encoder/autoencoder.py
--rw-rw-rw-   0        0        0     7668 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/lowpass.py
--rw-rw-rw-   0        0        0     5010 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/pipeline.py
--rw-rw-rw-   0        0        0     1585 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.801740 audio_upscaler-0.0.7/audio_upscaler/utilities/
--rw-rw-rw-   0        0        0       65 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.805739 audio_upscaler-0.0.7/audio_upscaler/utilities/audio/
--rw-rw-rw-   0        0        0       76 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/audio/__init__.py
--rw-rw-rw-   0        0        0     2752 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/audio/audio_processing.py
--rw-rw-rw-   0        0        0     6522 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/audio/stft.py
--rw-rw-rw-   0        0        0     2603 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/audio/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.807789 audio_upscaler-0.0.7/audio_upscaler/utilities/data/
--rw-rw-rw-   0        0        0       30 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/data/__init__.py
--rw-rw-rw-   0        0        0    15571 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/data/add_on.py
--rw-rw-rw-   0        0        0    20705 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/data/dataset.py
--rw-rw-rw-   0        0        0     5335 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/model.py
--rw-rw-rw-   0        0        0    20126 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/sampler.py
--rw-rw-rw-   0        0        0    18618 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utilities/tools.py
--rw-rw-rw-   0        0        0    17182 2024-04-27 09:12:21.000000 audio_upscaler-0.0.7/audio_upscaler/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:09:12.808790 audio_upscaler-0.0.7/audio_upscaler.egg-info/
--rw-rw-rw-   0        0        0     4637 2024-05-09 18:09:12.000000 audio_upscaler-0.0.7/audio_upscaler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5399 2024-05-09 18:09:12.000000 audio_upscaler-0.0.7/audio_upscaler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:09:12.000000 audio_upscaler-0.0.7/audio_upscaler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      243 2024-05-09 18:09:12.000000 audio_upscaler-0.0.7/audio_upscaler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 18:09:12.000000 audio_upscaler-0.0.7/audio_upscaler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 18:09:12.810790 audio_upscaler-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3380 2024-04-27 09:23:09.000000 audio_upscaler-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.334028 audio_upscaler-0.0.8/
+-rw-rw-rw-   0        0        0     1092 2024-04-26 20:27:22.000000 audio_upscaler-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4637 2024-05-09 18:24:11.333019 audio_upscaler-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3348 2024-04-26 20:27:22.000000 audio_upscaler-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.240869 audio_upscaler-0.0.8/audio_upscaler/
+-rw-rw-rw-   0        0        0       28 2024-05-09 18:22:25.000000 audio_upscaler-0.0.8/audio_upscaler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.245880 audio_upscaler-0.0.8/audio_upscaler/clap/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.260098 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/
+-rw-rw-rw-   0        0        0      664 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/__init__.py
+-rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-rw-   0        0        0    11261 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/factory.py
+-rw-rw-rw-   0        0        0     7369 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/feature_fusion.py
+-rw-rw-rw-   0        0        0    49373 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/htsat.py
+-rw-rw-rw-   0        0        0    16493 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/loss.py
+-rw-rw-rw-   0        0        0    33855 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.279588 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json
+-rw-rw-rw-   0        0        0      520 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-10.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14.json
+-rw-rw-rw-   0        0        0      517 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-6.json
+-rw-rw-rw-   0        0        0      409 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/RN101-quickgelu.json
+-rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/RN101.json
+-rw-rw-rw-   0        0        0      411 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/RN50-quickgelu.json
+-rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/RN50.json
+-rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/RN50x16.json
+-rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/RN50x4.json
+-rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/ViT-B-16.json
+-rw-rw-rw-   0        0        0      334 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/ViT-B-32.json
+-rw-rw-rw-   0        0        0      311 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/ViT-L-14.json
+-rw-rw-rw-   0        0        0     5179 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/openai.py
+-rw-rw-rw-   0        0        0    24066 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/pann_model.py
+-rw-rw-rw-   0        0        0     6607 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/pretrained.py
+-rw-rw-rw-   0        0        0     4444 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/timm_model.py
+-rw-rw-rw-   0        0        0     6597 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/tokenizer.py
+-rw-rw-rw-   0        0        0     1096 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/transform.py
+-rw-rw-rw-   0        0        0    12319 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.284590 audio_upscaler-0.0.8/audio_upscaler/clap/training/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/training/__init__.py
+-rw-rw-rw-   0        0        0    84448 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/training/audioset_textmap.npy
+-rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-rw-   0        0        0    30558 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/training/data.py
+-rw-rw-rw-   0        0        0    17765 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/clap/training/params.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.287691 audio_upscaler-0.0.8/audio_upscaler/hifigan/
+-rw-rw-rw-   0        0        0      238 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/hifigan/__init__.py
+-rw-rw-rw-   0        0        0     5698 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/hifigan/models.py
+-rw-rw-rw-   0        0        0    13214 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/hifigan/models_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.288694 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.293056 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/__init__.py
+-rw-rw-rw-   0        0        0    17996 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/ddim.py
+-rw-rw-rw-   0        0        0    62623 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/ddpm.py
+-rw-rw-rw-   0        0        0    13215 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/plms.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.295056 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/__init__.py
+-rw-rw-rw-   0        0        0    16226 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/attention.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.298991 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/
+-rw-rw-rw-   0        0        0     5542 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/__init__.py
+-rw-rw-rw-   0        0        0    21730 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py
+-rw-rw-rw-   0        0        0     7927 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.307502 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/
+-rw-rw-rw-   0        0        0     1406 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py
+-rw-rw-rw-   0        0        0     1991 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py
+-rw-rw-rw-   0        0        0     2086 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py
+-rw-rw-rw-   0        0        0     2521 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rw-rw-rw-   0        0        0      913 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rw-rw-rw-   0        0        0    14970 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py
+-rw-rw-rw-   0        0        0     4508 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rw-rw-rw-   0        0        0     8838 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rw-rw-rw-   0        0        0     2335 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.310510 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/__init__.py
+-rw-rw-rw-   0        0        0    35533 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py
+-rw-rw-rw-   0        0        0    41338 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rw-rw-rw-   0        0        0    10172 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.312519 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/distributions/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/distributions/__init__.py
+-rw-rw-rw-   0        0        0     3199 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/distributions/distributions.py
+-rw-rw-rw-   0        0        0     3148 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/ema.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.313511 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/encoders/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/encoders/__init__.py
+-rw-rw-rw-   0        0        0    26015 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/encoders/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.317023 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rw-rw-rw-   0        0        0    15296 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rw-rw-rw-   0        0        0     5121 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py
+-rw-rw-rw-   0        0        0     1652 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.320032 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/
+-rw-rw-rw-   0        0        0     1695 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py
+-rw-rw-rw-   0        0        0     3229 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py
+-rw-rw-rw-   0        0        0      651 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py
+-rw-rw-rw-   0        0        0     8084 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.321039 audio_upscaler-0.0.8/audio_upscaler/latent_encoder/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_encoder/__init__.py
+-rw-rw-rw-   0        0        0    11648 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/latent_encoder/autoencoder.py
+-rw-rw-rw-   0        0        0     7668 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/lowpass.py
+-rw-rw-rw-   0        0        0     5010 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/pipeline.py
+-rw-rw-rw-   0        0        0     1579 2024-05-09 18:22:22.000000 audio_upscaler-0.0.8/audio_upscaler/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.325034 audio_upscaler-0.0.8/audio_upscaler/utilities/
+-rw-rw-rw-   0        0        0       65 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.328101 audio_upscaler-0.0.8/audio_upscaler/utilities/audio/
+-rw-rw-rw-   0        0        0       76 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/audio/__init__.py
+-rw-rw-rw-   0        0        0     2752 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/audio/audio_processing.py
+-rw-rw-rw-   0        0        0     6522 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/audio/stft.py
+-rw-rw-rw-   0        0        0     2603 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/audio/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.330108 audio_upscaler-0.0.8/audio_upscaler/utilities/data/
+-rw-rw-rw-   0        0        0       30 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/data/__init__.py
+-rw-rw-rw-   0        0        0    15571 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/data/add_on.py
+-rw-rw-rw-   0        0        0    20705 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/data/dataset.py
+-rw-rw-rw-   0        0        0     5335 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/model.py
+-rw-rw-rw-   0        0        0    20126 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/sampler.py
+-rw-rw-rw-   0        0        0    18618 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utilities/tools.py
+-rw-rw-rw-   0        0        0    17182 2024-04-27 09:12:21.000000 audio_upscaler-0.0.8/audio_upscaler/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:24:11.332016 audio_upscaler-0.0.8/audio_upscaler.egg-info/
+-rw-rw-rw-   0        0        0     4637 2024-05-09 18:24:10.000000 audio_upscaler-0.0.8/audio_upscaler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5399 2024-05-09 18:24:11.000000 audio_upscaler-0.0.8/audio_upscaler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:24:10.000000 audio_upscaler-0.0.8/audio_upscaler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2024-05-09 18:24:10.000000 audio_upscaler-0.0.8/audio_upscaler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 18:24:11.000000 audio_upscaler-0.0.8/audio_upscaler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 18:24:11.334028 audio_upscaler-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3380 2024-05-09 18:24:05.000000 audio_upscaler-0.0.8/setup.py
```

### Comparing `audio_upscaler-0.0.7/LICENSE` & `audio_upscaler-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/PKG-INFO` & `audio_upscaler-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_upscaler
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/IAHispano/Audio-Upscaler
 Author: Aitron Emper
 Author-email: aitronssesin@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audio_upscaler-0.0.7/README.md` & `audio_upscaler-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/__init__.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/factory.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/feature_fusion.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/htsat.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/loss.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-10.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-10.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-14.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-14.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/model_configs/PANN-6.json` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/model_configs/PANN-6.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/openai.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/pann_model.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/pretrained.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/timm_model.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/tokenizer.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/transform.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/open_clip/utils.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/training/audioset_textmap.npy` & `audio_upscaler-0.0.8/audio_upscaler/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audio_upscaler-0.0.8/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/training/data.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/clap/training/params.py` & `audio_upscaler-0.0.8/audio_upscaler/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/hifigan/models.py` & `audio_upscaler-0.0.8/audio_upscaler/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/hifigan/models_v2.py` & `audio_upscaler-0.0.8/audio_upscaler/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/ddim.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/ddpm.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/ddpm.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/models/plms.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/attention.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/distributions/distributions.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/ema.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/encoders/modules.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_diffusion/util.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/latent_encoder/autoencoder.py` & `audio_upscaler-0.0.8/audio_upscaler/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/lowpass.py` & `audio_upscaler-0.0.8/audio_upscaler/lowpass.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/pipeline.py` & `audio_upscaler-0.0.8/audio_upscaler/pipeline.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/predict.py` & `audio_upscaler-0.0.8/audio_upscaler/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             ddim_steps=ddim_steps,
             latent_t_per_second=12.8
         )
         out_wav = (waveform[0] * 32767).astype(np.int16).T
         out_path = os.path.join(os.path.dirname(input_file), f"{os.path.splitext(os.path.basename(input_file))[0]}" + "_output.wav")
         sf.write(out_path, data=out_wav, samplerate=sr)
 
-def start_predict(input_file, sr=48000, ddim_steps=50, guidance_scale=3.5, model_name="basic", device="auto", seed=None):
+def upscale(input_file, sr=48000, ddim_steps=50, guidance_scale=3.5, model_name="basic", device="auto", seed=None):
     p = Predictor()
     p.setup(model_name, device)
     out = p.predict(
         input_file,
         sr=sr,
         ddim_steps=ddim_steps,
         guidance_scale=guidance_scale,
```

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/audio/audio_processing.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/audio/stft.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/audio/tools.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/data/add_on.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/data/dataset.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/model.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/sampler.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utilities/tools.py` & `audio_upscaler-0.0.8/audio_upscaler/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler/utils.py` & `audio_upscaler-0.0.8/audio_upscaler/utils.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/audio_upscaler.egg-info/PKG-INFO` & `audio_upscaler-0.0.8/audio_upscaler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_upscaler
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/IAHispano/Audio-Upscaler
 Author: Aitron Emper
 Author-email: aitronssesin@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audio_upscaler-0.0.7/audio_upscaler.egg-info/SOURCES.txt` & `audio_upscaler-0.0.8/audio_upscaler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.0.7/setup.py` & `audio_upscaler-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audio_upscaler"
 DESCRIPTION = "This package is written for text-to-audio/music generation."
 URL = "https://github.com/IAHispano/Audio-Upscaler"
 EMAIL = "aitronssesin@gmail.com"
 AUTHOR = "Aitron Emper"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

