# Comparing `tmp/audio_upscaler-0.1.0.tar.gz` & `tmp/audio_upscaler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_upscaler-0.1.0.tar", last modified: Thu May  9 18:40:47 2024, max compression
+gzip compressed data, was "audio_upscaler-0.1.1.tar", last modified: Thu May  9 18:50:21 2024, max compression
```

## Comparing `audio_upscaler-0.1.0.tar` & `audio_upscaler-0.1.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.349045 audio_upscaler-0.1.0/
--rw-rw-rw-   0        0        0     1092 2024-04-26 20:27:22.000000 audio_upscaler-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4637 2024-05-09 18:40:47.348045 audio_upscaler-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2024-04-26 20:27:22.000000 audio_upscaler-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.265953 audio_upscaler-0.1.0/audio_upscaler/
--rw-rw-rw-   0        0        0       28 2024-05-09 18:22:25.000000 audio_upscaler-0.1.0/audio_upscaler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.271241 audio_upscaler-0.1.0/audio_upscaler/clap/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.283231 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/
--rw-rw-rw-   0        0        0      664 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/__init__.py
--rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-rw-   0        0        0    11261 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/factory.py
--rw-rw-rw-   0        0        0     7369 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/feature_fusion.py
--rw-rw-rw-   0        0        0    49373 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/htsat.py
--rw-rw-rw-   0        0        0    16493 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/loss.py
--rw-rw-rw-   0        0        0    33855 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.300064 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json
--rw-rw-rw-   0        0        0      520 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-10.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14.json
--rw-rw-rw-   0        0        0      517 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-6.json
--rw-rw-rw-   0        0        0      409 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/RN101-quickgelu.json
--rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/RN101.json
--rw-rw-rw-   0        0        0      411 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/RN50-quickgelu.json
--rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/RN50.json
--rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/RN50x16.json
--rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/RN50x4.json
--rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/ViT-B-16.json
--rw-rw-rw-   0        0        0      334 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/ViT-B-32.json
--rw-rw-rw-   0        0        0      311 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/ViT-L-14.json
--rw-rw-rw-   0        0        0     5179 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/openai.py
--rw-rw-rw-   0        0        0    24066 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/pann_model.py
--rw-rw-rw-   0        0        0     6607 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/pretrained.py
--rw-rw-rw-   0        0        0     4444 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/timm_model.py
--rw-rw-rw-   0        0        0     6597 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/tokenizer.py
--rw-rw-rw-   0        0        0     1096 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/transform.py
--rw-rw-rw-   0        0        0    12319 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.305064 audio_upscaler-0.1.0/audio_upscaler/clap/training/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/training/__init__.py
--rw-rw-rw-   0        0        0    84448 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/training/audioset_textmap.npy
--rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz
--rw-rw-rw-   0        0        0    30558 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/training/data.py
--rw-rw-rw-   0        0        0    17765 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/clap/training/params.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.307567 audio_upscaler-0.1.0/audio_upscaler/hifigan/
--rw-rw-rw-   0        0        0      238 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/hifigan/__init__.py
--rw-rw-rw-   0        0        0     5698 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/hifigan/models.py
--rw-rw-rw-   0        0        0    13214 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/hifigan/models_v2.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.308570 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.312573 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/__init__.py
--rw-rw-rw-   0        0        0    17996 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/ddim.py
--rw-rw-rw-   0        0        0    62623 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/ddpm.py
--rw-rw-rw-   0        0        0    13215 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/plms.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.314573 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/__init__.py
--rw-rw-rw-   0        0        0    16226 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/attention.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.317077 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/
--rw-rw-rw-   0        0        0     5542 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/__init__.py
--rw-rw-rw-   0        0        0    21730 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py
--rw-rw-rw-   0        0        0     7927 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.324489 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/
--rw-rw-rw-   0        0        0     1406 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py
--rw-rw-rw-   0        0        0     1991 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py
--rw-rw-rw-   0        0        0     2086 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py
--rw-rw-rw-   0        0        0     2521 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py
--rw-rw-rw-   0        0        0      913 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py
--rw-rw-rw-   0        0        0    14970 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py
--rw-rw-rw-   0        0        0     4508 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py
--rw-rw-rw-   0        0        0     8838 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py
--rw-rw-rw-   0        0        0     2335 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.327996 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/__init__.py
--rw-rw-rw-   0        0        0    35533 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py
--rw-rw-rw-   0        0        0    41338 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rw-rw-rw-   0        0        0    10172 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.328997 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/distributions/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/distributions/__init__.py
--rw-rw-rw-   0        0        0     3199 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/distributions/distributions.py
--rw-rw-rw-   0        0        0     3148 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/ema.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.330997 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/encoders/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/encoders/__init__.py
--rw-rw-rw-   0        0        0    26015 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/encoders/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.333996 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/__init__.py
--rw-rw-rw-   0        0        0    15296 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py
--rw-rw-rw-   0        0        0     5121 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py
--rw-rw-rw-   0        0        0     1652 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.337029 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/
--rw-rw-rw-   0        0        0     1695 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py
--rw-rw-rw-   0        0        0     3229 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py
--rw-rw-rw-   0        0        0      651 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py
--rw-rw-rw-   0        0        0     8084 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.338536 audio_upscaler-0.1.0/audio_upscaler/latent_encoder/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_encoder/__init__.py
--rw-rw-rw-   0        0        0    11648 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/latent_encoder/autoencoder.py
--rw-rw-rw-   0        0        0     7668 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/lowpass.py
--rw-rw-rw-   0        0        0     5010 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/pipeline.py
--rw-rw-rw-   0        0        0     1674 2024-05-09 18:39:44.000000 audio_upscaler-0.1.0/audio_upscaler/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.341538 audio_upscaler-0.1.0/audio_upscaler/utilities/
--rw-rw-rw-   0        0        0       65 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.344539 audio_upscaler-0.1.0/audio_upscaler/utilities/audio/
--rw-rw-rw-   0        0        0       76 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/audio/__init__.py
--rw-rw-rw-   0        0        0     2752 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/audio/audio_processing.py
--rw-rw-rw-   0        0        0     6522 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/audio/stft.py
--rw-rw-rw-   0        0        0     2603 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/audio/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.347106 audio_upscaler-0.1.0/audio_upscaler/utilities/data/
--rw-rw-rw-   0        0        0       30 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/data/__init__.py
--rw-rw-rw-   0        0        0    15571 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/data/add_on.py
--rw-rw-rw-   0        0        0    20705 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/data/dataset.py
--rw-rw-rw-   0        0        0     5335 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/model.py
--rw-rw-rw-   0        0        0    20126 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/sampler.py
--rw-rw-rw-   0        0        0    18618 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utilities/tools.py
--rw-rw-rw-   0        0        0    17182 2024-04-27 09:12:21.000000 audio_upscaler-0.1.0/audio_upscaler/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:40:47.348045 audio_upscaler-0.1.0/audio_upscaler.egg-info/
--rw-rw-rw-   0        0        0     4637 2024-05-09 18:40:47.000000 audio_upscaler-0.1.0/audio_upscaler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5399 2024-05-09 18:40:47.000000 audio_upscaler-0.1.0/audio_upscaler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:40:47.000000 audio_upscaler-0.1.0/audio_upscaler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      243 2024-05-09 18:40:47.000000 audio_upscaler-0.1.0/audio_upscaler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 18:40:47.000000 audio_upscaler-0.1.0/audio_upscaler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 18:40:47.349045 audio_upscaler-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3380 2024-05-09 18:39:12.000000 audio_upscaler-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.758344 audio_upscaler-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2024-04-26 20:27:22.000000 audio_upscaler-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4637 2024-05-09 18:50:21.757338 audio_upscaler-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3348 2024-04-26 20:27:22.000000 audio_upscaler-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.651205 audio_upscaler-0.1.1/audio_upscaler/
+-rw-rw-rw-   0        0        0       28 2024-05-09 18:22:25.000000 audio_upscaler-0.1.1/audio_upscaler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.658389 audio_upscaler-0.1.1/audio_upscaler/clap/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.674944 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/
+-rw-rw-rw-   0        0        0      664 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/__init__.py
+-rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-rw-   0        0        0    11261 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/factory.py
+-rw-rw-rw-   0        0        0     7369 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/feature_fusion.py
+-rw-rw-rw-   0        0        0    49373 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/htsat.py
+-rw-rw-rw-   0        0        0    16493 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/loss.py
+-rw-rw-rw-   0        0        0    33855 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.696056 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json
+-rw-rw-rw-   0        0        0      520 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-10.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14.json
+-rw-rw-rw-   0        0        0      517 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-6.json
+-rw-rw-rw-   0        0        0      409 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN101-quickgelu.json
+-rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN101.json
+-rw-rw-rw-   0        0        0      411 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50-quickgelu.json
+-rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50.json
+-rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50x16.json
+-rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50x4.json
+-rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-B-16.json
+-rw-rw-rw-   0        0        0      334 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-B-32.json
+-rw-rw-rw-   0        0        0      311 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-L-14.json
+-rw-rw-rw-   0        0        0     5179 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/openai.py
+-rw-rw-rw-   0        0        0    24066 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pann_model.py
+-rw-rw-rw-   0        0        0     6607 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pretrained.py
+-rw-rw-rw-   0        0        0     4444 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/timm_model.py
+-rw-rw-rw-   0        0        0     6597 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/tokenizer.py
+-rw-rw-rw-   0        0        0     1096 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/transform.py
+-rw-rw-rw-   0        0        0    12319 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.701571 audio_upscaler-0.1.1/audio_upscaler/clap/training/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/__init__.py
+-rw-rw-rw-   0        0        0    84448 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/audioset_textmap.npy
+-rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-rw-   0        0        0    30555 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/data.py
+-rw-rw-rw-   0        0        0    17765 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/params.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.704077 audio_upscaler-0.1.1/audio_upscaler/hifigan/
+-rw-rw-rw-   0        0        0      238 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/hifigan/__init__.py
+-rw-rw-rw-   0        0        0     5698 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/hifigan/models.py
+-rw-rw-rw-   0        0        0    13214 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/hifigan/models_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.705547 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.710064 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/__init__.py
+-rw-rw-rw-   0        0        0    17995 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddim.py
+-rw-rw-rw-   0        0        0    62616 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddpm.py
+-rw-rw-rw-   0        0        0    13214 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/plms.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.713960 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/__init__.py
+-rw-rw-rw-   0        0        0    16225 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/attention.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.717474 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/
+-rw-rw-rw-   0        0        0     5540 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/__init__.py
+-rw-rw-rw-   0        0        0    21728 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py
+-rw-rw-rw-   0        0        0     7927 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.727522 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/
+-rw-rw-rw-   0        0        0     1406 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py
+-rw-rw-rw-   0        0        0     1991 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py
+-rw-rw-rw-   0        0        0     2086 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py
+-rw-rw-rw-   0        0        0     2521 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rw-rw-rw-   0        0        0      913 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rw-rw-rw-   0        0        0    14970 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py
+-rw-rw-rw-   0        0        0     4508 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rw-rw-rw-   0        0        0     8838 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rw-rw-rw-   0        0        0     2335 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.731600 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/__init__.py
+-rw-rw-rw-   0        0        0    35531 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py
+-rw-rw-rw-   0        0        0    41336 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rw-rw-rw-   0        0        0    10171 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.733601 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/__init__.py
+-rw-rw-rw-   0        0        0     3199 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/distributions.py
+-rw-rw-rw-   0        0        0     3148 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/ema.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.736081 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/__init__.py
+-rw-rw-rw-   0        0        0    26010 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.739596 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rw-rw-rw-   0        0        0    15295 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rw-rw-rw-   0        0        0     5121 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py
+-rw-rw-rw-   0        0        0     1650 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.742596 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/
+-rw-rw-rw-   0        0        0     1693 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py
+-rw-rw-rw-   0        0        0     3229 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py
+-rw-rw-rw-   0        0        0      651 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py
+-rw-rw-rw-   0        0        0     8084 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.744798 audio_upscaler-0.1.1/audio_upscaler/latent_encoder/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_encoder/__init__.py
+-rw-rw-rw-   0        0        0    11642 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_encoder/autoencoder.py
+-rw-rw-rw-   0        0        0     7668 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/lowpass.py
+-rw-rw-rw-   0        0        0     5005 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/pipeline.py
+-rw-rw-rw-   0        0        0     1674 2024-05-09 18:39:44.000000 audio_upscaler-0.1.1/audio_upscaler/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.748317 audio_upscaler-0.1.1/audio_upscaler/utilities/
+-rw-rw-rw-   0        0        0       65 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.752317 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/
+-rw-rw-rw-   0        0        0       76 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/__init__.py
+-rw-rw-rw-   0        0        0     2752 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/audio_processing.py
+-rw-rw-rw-   0        0        0     6521 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/stft.py
+-rw-rw-rw-   0        0        0     2602 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.755832 audio_upscaler-0.1.1/audio_upscaler/utilities/data/
+-rw-rw-rw-   0        0        0       30 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/data/__init__.py
+-rw-rw-rw-   0        0        0    15571 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/data/add_on.py
+-rw-rw-rw-   0        0        0    20703 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/data/dataset.py
+-rw-rw-rw-   0        0        0     5334 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/model.py
+-rw-rw-rw-   0        0        0    20126 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/sampler.py
+-rw-rw-rw-   0        0        0    18618 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/tools.py
+-rw-rw-rw-   0        0        0    17174 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.755832 audio_upscaler-0.1.1/audio_upscaler.egg-info/
+-rw-rw-rw-   0        0        0     4637 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5399 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 18:50:21.758344 audio_upscaler-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3380 2024-05-09 18:50:13.000000 audio_upscaler-0.1.1/setup.py
```

### Comparing `audio_upscaler-0.1.0/LICENSE` & `audio_upscaler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/PKG-INFO` & `audio_upscaler-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_upscaler
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/IAHispano/Audio-Upscaler
 Author: Aitron Emper
 Author-email: aitronssesin@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audio_upscaler-0.1.0/README.md` & `audio_upscaler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/__init__.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/factory.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/feature_fusion.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/htsat.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/loss.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-10.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-10.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-14.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/model_configs/PANN-6.json` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-6.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/openai.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/pann_model.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/pretrained.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/timm_model.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/tokenizer.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/transform.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/open_clip/utils.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/training/audioset_textmap.npy` & `audio_upscaler-0.1.1/audio_upscaler/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audio_upscaler-0.1.1/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/training/data.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/training/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 from torch.utils.data.distributed import DistributedSampler
 import soundfile as sf
 import io
 from pathlib import Path
 
 # import wget
 
-from audiosr_package.clap.open_clip.utils import get_tar_path_from_dataset_name
-from audiosr_package.clap.open_clip.utils import load_class_label
+from audio_upscaler.clap.open_clip.utils import get_tar_path_from_dataset_name
+from audio_upscaler.clap.open_clip.utils import load_class_label
 
 try:
     import horovod.torch as hvd
 except ImportError:
     hvd = None
 
 try:
     import torchaudio
 except ImportError:
     torchaudio = None
 
-from audiosr_package.clap.open_clip import tokenize
+from audio_upscaler.clap.open_clip import tokenize
 
 
 def tokenizer(text):
     return tokenize(text).squeeze(0)
 
 
 from transformers import RobertaTokenizer
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/clap/training/params.py` & `audio_upscaler-0.1.1/audio_upscaler/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/hifigan/models.py` & `audio_upscaler-0.1.1/audio_upscaler/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/hifigan/models_v2.py` & `audio_upscaler-0.1.1/audio_upscaler/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/ddim.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """SAMPLING ONLY."""
 
 import torch
 import numpy as np
 from tqdm import tqdm
 
-from audiosr_package.latent_diffusion.modules.diffusionmodules.util import (
+from audio_upscaler.latent_diffusion.modules.diffusionmodules.util import (
     make_ddim_sampling_parameters,
     make_ddim_timesteps,
     noise_like,
     extract_into_tensor,
 )
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/ddpm.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import torch.nn as nn
 import numpy as np
 from einops import rearrange, repeat
 from contextlib import contextmanager
 from functools import partial
 from tqdm import tqdm
 from torchvision.utils import make_grid
-from audiosr_package.latent_diffusion.modules.encoders.modules import *
+from audio_upscaler.latent_diffusion.modules.encoders.modules import *
 
-from audiosr_package.latent_diffusion.util import (
+from audio_upscaler.latent_diffusion.util import (
     exists,
     default,
     count_params,
     instantiate_from_config,
 )
-from audiosr_package.latent_diffusion.modules.ema import LitEma
-from audiosr_package.latent_diffusion.modules.distributions.distributions import (
+from audio_upscaler.latent_diffusion.modules.ema import LitEma
+from audio_upscaler.latent_diffusion.modules.distributions.distributions import (
     DiagonalGaussianDistribution,
 )
 
-from audiosr_package.latent_diffusion.modules.diffusionmodules.util import (
+from audio_upscaler.latent_diffusion.modules.diffusionmodules.util import (
     make_beta_schedule,
     extract_into_tensor,
     noise_like,
 )
 
-from audiosr_package.latent_diffusion.models.ddim import DDIMSampler
-from audiosr_package.latent_diffusion.models.plms import PLMSSampler
+from audio_upscaler.latent_diffusion.models.ddim import DDIMSampler
+from audio_upscaler.latent_diffusion.models.plms import PLMSSampler
 import soundfile as sf
 import os
 
 __conditioning_keys__ = {"concat": "c_concat", "crossattn": "c_crossattn", "adm": "y"}
 
 
 def disabled_train(self, mode=True):
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/models/plms.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/plms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """SAMPLING ONLY."""
 
 import torch
 import numpy as np
 from tqdm import tqdm
 
-from audiosr_package.latent_diffusion.modules.diffusionmodules.util import (
+from audio_upscaler.latent_diffusion.modules.diffusionmodules.util import (
     make_ddim_sampling_parameters,
     make_ddim_timesteps,
     noise_like,
 )
 
 
 class PLMSSampler(object):
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/attention.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inspect import isfunction
 import math
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 from einops import rearrange, repeat
 
-from audiosr_package.latent_diffusion.modules.diffusionmodules.util import checkpoint
+from audio_upscaler.latent_diffusion.modules.diffusionmodules.util import checkpoint
 
 
 def exists(val):
     return val is not None
 
 
 def uniq(arr):
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Reference Repo: https://github.com/facebookresearch/AudioMAE
 """
 
 import torch
 import torch.nn as nn
 from timm.models.layers import to_2tuple
-import audiosr_package.latent_diffusion.modules.audiomae.models_vit as models_vit
-import audiosr_package.latent_diffusion.modules.audiomae.models_mae as models_mae
+import audio_upscaler.latent_diffusion.modules.audiomae.models_vit as models_vit
+import audio_upscaler.latent_diffusion.modules.audiomae.models_mae as models_mae
 
 # model = mae_vit_base_patch16(in_chans=1, audio_exp=True, img_size=(1024, 128))
 
 
 class PatchEmbed_new(nn.Module):
     """Flexible Image to Patch Embedding"""
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 from functools import partial
 
 import torch
 import torch.nn as nn
 
 from timm.models.vision_transformer import Block
-from audiosr_package.latent_diffusion.modules.audiomae.util.pos_embed import (
+from audio_upscaler.latent_diffusion.modules.audiomae.util.pos_embed import (
     get_2d_sincos_pos_embed,
     get_2d_sincos_pos_embed_flexible,
 )
-from audiosr_package.latent_diffusion.modules.audiomae.util.patch_embed import (
+from audio_upscaler.latent_diffusion.modules.audiomae.util.patch_embed import (
     PatchEmbed_new,
     PatchEmbed_org,
 )
 
 
 class MaskedAutoencoderViT(nn.Module):
     """Masked Autoencoder with VisionTransformer backbone"""
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pytorch_diffusion + derived encoder decoder
 import math
 import torch
 import torch.nn as nn
 import numpy as np
 from einops import rearrange
 
-from audiosr_package.latent_diffusion.util import instantiate_from_config
-from audiosr_package.latent_diffusion.modules.attention import LinearAttention
+from audio_upscaler.latent_diffusion.util import instantiate_from_config
+from audio_upscaler.latent_diffusion.modules.attention import LinearAttention
 
 
 def get_timestep_embedding(timesteps, embedding_dim):
     """
     This matches the implementation in Denoising Diffusion Probabilistic Models:
     From Fairseq.
     Build sinusoidal embeddings.
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import math
 
 import numpy as np
 import torch as th
 import torch.nn as nn
 import torch.nn.functional as F
 
-from audiosr_package.latent_diffusion.modules.diffusionmodules.util import (
+from audio_upscaler.latent_diffusion.modules.diffusionmodules.util import (
     checkpoint,
     conv_nd,
     linear,
     avg_pool_nd,
     zero_module,
     normalization,
     timestep_embedding,
 )
-from audiosr_package.latent_diffusion.modules.attention import SpatialTransformer
+from audio_upscaler.latent_diffusion.modules.attention import SpatialTransformer
 
 
 # dummy replace
 def convert_module_to_f16(x):
     pass
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import math
 import torch
 import torch.nn as nn
 import numpy as np
 from einops import repeat
 
-from audiosr_package.latent_diffusion.util import instantiate_from_config
+from audio_upscaler.latent_diffusion.util import instantiate_from_config
 
 
 def make_beta_schedule(
     schedule, n_timestep, linear_start=1e-4, linear_end=2e-2, cosine_s=8e-3
 ):
     if schedule == "linear":
         betas = (
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/distributions/distributions.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/ema.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/encoders/modules.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import torch
 import logging
 import torch.nn as nn
-from audiosr_package.clap.open_clip import create_model
-from audiosr_package.clap.training.data import get_audio_features
+from audio_upscaler.clap.open_clip import create_model
+from audio_upscaler.clap.training.data import get_audio_features
 import torchaudio
 from transformers import RobertaTokenizer, AutoTokenizer, T5EncoderModel
 import torch.nn.functional as F
-from audiosr_package.latent_diffusion.modules.audiomae.AudioMAE import Vanilla_AudioMAE
-from audiosr_package.latent_diffusion.modules.phoneme_encoder.encoder import TextEncoder
-from audiosr_package.latent_diffusion.util import instantiate_from_config
+from audio_upscaler.latent_diffusion.modules.audiomae.AudioMAE import Vanilla_AudioMAE
+from audio_upscaler.latent_diffusion.modules.phoneme_encoder.encoder import TextEncoder
+from audio_upscaler.latent_diffusion.util import instantiate_from_config
 
 from transformers import AutoTokenizer, T5Config
 
 
 import numpy as np
 
 """
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import torch
 from torch import nn
 from torch.nn import functional as F
 
-import audiosr_package.latent_diffusion.modules.phoneme_encoder.commons as commons
+import audio_upscaler.latent_diffusion.modules.phoneme_encoder.commons as commons
 
 LRELU_SLOPE = 0.1
 
 
 class LayerNorm(nn.Module):
     def __init__(self, channels, eps=1e-5):
         super().__init__()
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import torch
 from torch import nn
 
-import audiosr_package.latent_diffusion.modules.phoneme_encoder.commons as commons
-import audiosr_package.latent_diffusion.modules.phoneme_encoder.attentions as attentions
+import audio_upscaler.latent_diffusion.modules.phoneme_encoder.commons as commons
+import audio_upscaler.latent_diffusion.modules.phoneme_encoder.attentions as attentions
 
 
 class TextEncoder(nn.Module):
     def __init__(
         self,
         n_vocab,
         out_channels=192,
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ from https://github.com/keithito/tacotron """
-from audiosr_package.latent_diffusion.modules.phoneme_encoder.text import cleaners
-from audiosr_package.latent_diffusion.modules.phoneme_encoder.text.symbols import symbols
+from audio_upscaler.latent_diffusion.modules.phoneme_encoder.text import cleaners
+from audio_upscaler.latent_diffusion.modules.phoneme_encoder.text.symbols import symbols
 
 
 # Mappings from symbol to numeric ID and vice versa:
 _symbol_to_id = {s: i for i, s in enumerate(symbols)}
 _id_to_symbol = {i: s for i, s in enumerate(symbols)}
 
 cleaner = getattr(cleaners, "english_cleaners2")
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_diffusion/util.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/latent_encoder/autoencoder.py` & `audio_upscaler-0.1.1/audio_upscaler/latent_encoder/autoencoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import torch
 import os
 
 import torch.nn.functional as F
 import numpy as np
-from audiosr_package.latent_diffusion.modules.ema import *
+from audio_upscaler.latent_diffusion.modules.ema import *
 
-from audiosr_package.latent_diffusion.modules.diffusionmodules.model import Encoder, Decoder
-from audiosr_package.latent_diffusion.modules.distributions.distributions import (
+from audio_upscaler.latent_diffusion.modules.diffusionmodules.model import Encoder, Decoder
+from audio_upscaler.latent_diffusion.modules.distributions.distributions import (
     DiagonalGaussianDistribution,
 )
 import soundfile as sf
 
-from audiosr_package.utilities.model import get_vocoder
-from audiosr_package.utilities.tools import synth_one_sample
+from audio_upscaler.utilities.model import get_vocoder
+from audio_upscaler.utilities.tools import synth_one_sample
 
 
 class AutoencoderKL(nn.Module):
     def __init__(
         self,
         ddconfig=None,
         lossconfig=None,
@@ -113,15 +113,15 @@
         dec = self.decoder(z)
         # bs, ch, shuffled_timesteps, fbins = dec.size()
         # dec = self.time_unshuffle_operation(dec, bs, int(ch*shuffled_timesteps), fbins)
         # dec = self.freq_merge_subband(dec)
         return dec
 
     def decode_to_waveform(self, dec):
-        from audiosr_package.utilities.model import vocoder_infer
+        from audio_upscaler.utilities.model import vocoder_infer
 
         if self.image_key == "fbank":
             dec = dec.squeeze(1).permute(0, 2, 1)
             wav_reconstruction = vocoder_infer(dec, self.vocoder)
         elif self.image_key == "stft":
             dec = dec.squeeze(1).permute(0, 2, 1)
             wav_reconstruction = self.wave_decoder(dec)
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/lowpass.py` & `audio_upscaler-0.1.1/audio_upscaler/lowpass.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/pipeline.py` & `audio_upscaler-0.1.1/audio_upscaler/pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import re
 
 import yaml
 import torch
 import torchaudio
 import numpy as np
 
-import audiosr_package.latent_diffusion.modules.phoneme_encoder.text as text
-from audiosr_package.latent_diffusion.models.ddpm import LatentDiffusion
-from audiosr_package.latent_diffusion.util import get_vits_phoneme_ids_no_padding
-from audiosr_package.utils import (
+import audio_upscaler.latent_diffusion.modules.phoneme_encoder.text as text
+from audio_upscaler.latent_diffusion.models.ddpm import LatentDiffusion
+from audio_upscaler.latent_diffusion.util import get_vits_phoneme_ids_no_padding
+from audio_upscaler.utils import (
     default_audioldm_config,
     download_checkpoint,
     read_audio_file,
     lowpass_filtering_prepare_inference,
     wav_feature_extraction,
 )
 import os
@@ -116,15 +116,15 @@
         if torch.cuda.is_available():
             device = torch.device("cuda:0")
         elif torch.backends.mps.is_available():
             device = torch.device("mps")
         else:
             device = torch.device("cpu")
 
-    print("Loading audiosr_package: %s" % model_name)
+    print("Loading audio_upscaler: %s" % model_name)
     print("Loading model on %s" % device)
 
     ckpt_path = download_checkpoint(model_name)
 
     if config is not None:
         assert type(config) is str
         config = yaml.load(open(config, "r"), Loader=yaml.FullLoader)
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/predict.py` & `audio_upscaler-0.1.1/audio_upscaler/predict.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/audio/audio_processing.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/audio/stft.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/audio/stft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import torch.nn.functional as F
 import numpy as np
 from scipy.signal import get_window
 from librosa.util import pad_center, tiny
 from librosa.filters import mel as librosa_mel_fn
 
-from audiosr_package.utilities.audio.audio_processing import (
+from audio_upscaler.utilities.audio.audio_processing import (
     dynamic_range_compression,
     dynamic_range_decompression,
     window_sumsquare,
 )
 
 
 class STFT(torch.nn.Module):
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/audio/tools.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/audio/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import numpy as np
 from scipy.io.wavfile import write
 import torchaudio
 
-from audiosr_package.utilities.audio.audio_processing import griffin_lim
+from audio_upscaler.utilities.audio.audio_processing import griffin_lim
 
 
 def pad_wav(waveform, segment_length):
     waveform_length = waveform.shape[-1]
     assert waveform_length > 100, "Waveform is too short, %s" % waveform_length
     if segment_length is None or waveform_length == segment_length:
         return waveform
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/data/add_on.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/data/dataset.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import pandas as pd
 
-import audiosr_package.utilities.audio as Audio
-from audiosr_package.utilities.tools import load_json
+import audio_upscaler.utilities.audio as Audio
+from audio_upscaler.utilities.tools import load_json
 
 import random
 from torch.utils.data import Dataset
 import torch.nn.functional
 import torch
 import numpy as np
 import torchaudio
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/model.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-import audiosr_package.hifigan as hifigan
+import audio_upscaler.hifigan as hifigan
 
 
 def get_vocoder_config():
     return {
         "resblock": "1",
         "num_gpus": 6,
         "batch_size": 16,
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/sampler.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utilities/tools.py` & `audio_upscaler-0.1.1/audio_upscaler/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/audio_upscaler/utils.py` & `audio_upscaler-0.1.1/audio_upscaler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import wget
 import soundfile as sf
 import time
 import wave
 import torchaudio
 import progressbar
 from librosa.filters import mel as librosa_mel_fn
-from audiosr_package.lowpass import lowpass
+from audio_upscaler.lowpass import lowpass
 
 hann_window = {}
 mel_basis = {}
 
 
 def dynamic_range_compression_torch(x, C=1, clip_val=1e-5):
     return torch.log(torch.clamp(x, min=clip_val) * C)
@@ -187,15 +187,15 @@
     return waveform * 0.5
 
 def read_wav_file(filename):
     waveform, sr = torchaudio.load(filename)
     duration = waveform.size(-1) / sr
 
     if(duration > 10.24):
-        print("\033[93m {}\033[00m" .format("Warning: audio is longer than 10.24 seconds, may degrade the model performance. It's recommand to truncate your audio to 5.12 seconds before input to audiosr_package to get the best performance."))
+        print("\033[93m {}\033[00m" .format("Warning: audio is longer than 10.24 seconds, may degrade the model performance. It's recommand to truncate your audio to 5.12 seconds before input to audio_upscaler to get the best performance."))
 
     if(duration % 5.12 != 0):
         pad_duration = duration + (5.12 - duration % 5.12)
     else:
         pad_duration = duration
 
     target_frame = int(pad_duration * 100)
@@ -306,15 +306,15 @@
             )
             # Avoid the file name too long to be saved
             if len(fname) > 255:
                 fname = f"{hex(hash(fname))}.wav"
 
         save_path = os.path.join(savepath, fname)
         temp_path = os.path.join(tempfile.gettempdir(), fname)
-        print("\033[98m {}\033[00m" .format("Don't forget to try different seeds by setting --seed <int> so that audiosr_package can have optimal performance on your hardware."))
+        print("\033[98m {}\033[00m" .format("Don't forget to try different seeds by setting --seed <int> so that audio_upscaler can have optimal performance on your hardware."))
         print("Save audio to %s." % save_path)
         sf.write(temp_path, waveform[i, 0], samplerate=samplerate)
         strip_silence(inputpath, temp_path, save_path)
 
 
 def exists(x):
     return x is not None
@@ -400,19 +400,19 @@
                 "duration": 10.24,
             },
             "stft": {"filter_length": 2048, "hop_length": 480, "win_length": 2048},
             "mel": {"n_mel_channels": 256, "mel_fmin": 20, "mel_fmax": 24000},
         },
         "augmentation": {"mixup": 0.5},
         "model": {
-            "target": "audiosr_package.latent_diffusion.models.ddpm.LatentDiffusion",
+            "target": "audio_upscaler.latent_diffusion.models.ddpm.LatentDiffusion",
             "params": {
                 "first_stage_config": {
                     "base_learning_rate": 0.000008,
-                    "target": "audiosr_package.latent_encoder.autoencoder.AutoencoderKL",
+                    "target": "audio_upscaler.latent_encoder.autoencoder.AutoencoderKL",
                     "params": {
                         "reload_from_ckpt": "/mnt/bn/lqhaoheliu/project/audio_generation_diffusion/log/vae/vae_48k_256/ds_8_kl_1/checkpoints/ckpt-checkpoint-484999.ckpt",
                         "sampling_rate": 48000,
                         "batchsize": 4,
                         "monitor": "val/rec_loss",
                         "image_key": "fbank",
                         "subband": 1,
@@ -450,15 +450,15 @@
                 "first_stage_key": "fbank",
                 "latent_t_size": 128,
                 "latent_f_size": 32,
                 "channels": 16,
                 "monitor": "val/loss_simple_ema",
                 "scale_by_std": True,
                 "unet_config": {
-                    "target": "audiosr_package.latent_diffusion.modules.diffusionmodules.openaimodel.UNetModel",
+                    "target": "audio_upscaler.latent_diffusion.modules.diffusionmodules.openaimodel.UNetModel",
                     "params": {
                         "image_size": 64,
                         "in_channels": 32,
                         "out_channels": 16,
                         "model_channels": 128,
                         "attention_resolutions": [8, 4, 2],
                         "num_res_blocks": 2,
@@ -474,19 +474,19 @@
                     "ddim_sampling_steps": 200,
                     "n_candidates_per_samples": 1,
                 },
                 "cond_stage_config": {
                     "concat_lowpass_cond": {
                         "cond_stage_key": "lowpass_mel",
                         "conditioning_key": "concat",
-                        "target": "audiosr_package.latent_diffusion.modules.encoders.modules.VAEFeatureExtract",
+                        "target": "audio_upscaler.latent_diffusion.modules.encoders.modules.VAEFeatureExtract",
                         "params": {
                             "first_stage_config": {
                                 "base_learning_rate": 0.000008,
-                                "target": "audiosr_package.latent_encoder.autoencoder.AutoencoderKL",
+                                "target": "audio_upscaler.latent_encoder.autoencoder.AutoencoderKL",
                                 "params": {
                                     "sampling_rate": 48000,
                                     "batchsize": 4,
                                     "monitor": "val/rec_loss",
                                     "image_key": "fbank",
                                     "subband": 1,
                                     "embed_dim": 16,
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler.egg-info/PKG-INFO` & `audio_upscaler-0.1.1/audio_upscaler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_upscaler
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/IAHispano/Audio-Upscaler
 Author: Aitron Emper
 Author-email: aitronssesin@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audio_upscaler-0.1.0/audio_upscaler.egg-info/SOURCES.txt` & `audio_upscaler-0.1.1/audio_upscaler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.0/setup.py` & `audio_upscaler-0.1.1/setup.py`

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
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

