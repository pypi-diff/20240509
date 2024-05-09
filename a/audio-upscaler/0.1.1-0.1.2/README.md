# Comparing `tmp/audio_upscaler-0.1.1.tar.gz` & `tmp/audio_upscaler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_upscaler-0.1.1.tar", last modified: Thu May  9 18:50:21 2024, max compression
+gzip compressed data, was "audio_upscaler-0.1.2.tar", last modified: Thu May  9 19:32:44 2024, max compression
```

## Comparing `audio_upscaler-0.1.1.tar` & `audio_upscaler-0.1.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.758344 audio_upscaler-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-04-26 20:27:22.000000 audio_upscaler-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4637 2024-05-09 18:50:21.757338 audio_upscaler-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2024-04-26 20:27:22.000000 audio_upscaler-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.651205 audio_upscaler-0.1.1/audio_upscaler/
--rw-rw-rw-   0        0        0       28 2024-05-09 18:22:25.000000 audio_upscaler-0.1.1/audio_upscaler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.658389 audio_upscaler-0.1.1/audio_upscaler/clap/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.674944 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/
--rw-rw-rw-   0        0        0      664 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/__init__.py
--rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-rw-   0        0        0    11261 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/factory.py
--rw-rw-rw-   0        0        0     7369 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/feature_fusion.py
--rw-rw-rw-   0        0        0    49373 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/htsat.py
--rw-rw-rw-   0        0        0    16493 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/loss.py
--rw-rw-rw-   0        0        0    33855 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.696056 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json
--rw-rw-rw-   0        0        0      520 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-10.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json
--rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14.json
--rw-rw-rw-   0        0        0      517 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-6.json
--rw-rw-rw-   0        0        0      409 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN101-quickgelu.json
--rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN101.json
--rw-rw-rw-   0        0        0      411 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50-quickgelu.json
--rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50.json
--rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50x16.json
--rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/RN50x4.json
--rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-B-16.json
--rw-rw-rw-   0        0        0      334 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-B-32.json
--rw-rw-rw-   0        0        0      311 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/ViT-L-14.json
--rw-rw-rw-   0        0        0     5179 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/openai.py
--rw-rw-rw-   0        0        0    24066 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pann_model.py
--rw-rw-rw-   0        0        0     6607 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pretrained.py
--rw-rw-rw-   0        0        0     4444 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/timm_model.py
--rw-rw-rw-   0        0        0     6597 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/tokenizer.py
--rw-rw-rw-   0        0        0     1096 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/transform.py
--rw-rw-rw-   0        0        0    12319 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.701571 audio_upscaler-0.1.1/audio_upscaler/clap/training/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/__init__.py
--rw-rw-rw-   0        0        0    84448 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/audioset_textmap.npy
--rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz
--rw-rw-rw-   0        0        0    30555 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/data.py
--rw-rw-rw-   0        0        0    17765 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/clap/training/params.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.704077 audio_upscaler-0.1.1/audio_upscaler/hifigan/
--rw-rw-rw-   0        0        0      238 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/hifigan/__init__.py
--rw-rw-rw-   0        0        0     5698 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/hifigan/models.py
--rw-rw-rw-   0        0        0    13214 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/hifigan/models_v2.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.705547 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.710064 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/__init__.py
--rw-rw-rw-   0        0        0    17995 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddim.py
--rw-rw-rw-   0        0        0    62616 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddpm.py
--rw-rw-rw-   0        0        0    13214 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/plms.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.713960 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/__init__.py
--rw-rw-rw-   0        0        0    16225 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/attention.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.717474 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/
--rw-rw-rw-   0        0        0     5540 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/__init__.py
--rw-rw-rw-   0        0        0    21728 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py
--rw-rw-rw-   0        0        0     7927 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.727522 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/
--rw-rw-rw-   0        0        0     1406 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py
--rw-rw-rw-   0        0        0     1991 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py
--rw-rw-rw-   0        0        0     2086 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py
--rw-rw-rw-   0        0        0     2521 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py
--rw-rw-rw-   0        0        0      913 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py
--rw-rw-rw-   0        0        0    14970 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py
--rw-rw-rw-   0        0        0     4508 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py
--rw-rw-rw-   0        0        0     8838 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py
--rw-rw-rw-   0        0        0     2335 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.731600 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/__init__.py
--rw-rw-rw-   0        0        0    35531 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py
--rw-rw-rw-   0        0        0    41336 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rw-rw-rw-   0        0        0    10171 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.733601 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/__init__.py
--rw-rw-rw-   0        0        0     3199 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/distributions.py
--rw-rw-rw-   0        0        0     3148 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/ema.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.736081 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/__init__.py
--rw-rw-rw-   0        0        0    26010 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.739596 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/__init__.py
--rw-rw-rw-   0        0        0    15295 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py
--rw-rw-rw-   0        0        0     5121 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py
--rw-rw-rw-   0        0        0     1650 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.742596 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/
--rw-rw-rw-   0        0        0     1693 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py
--rw-rw-rw-   0        0        0     3229 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py
--rw-rw-rw-   0        0        0      651 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py
--rw-rw-rw-   0        0        0     8084 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.744798 audio_upscaler-0.1.1/audio_upscaler/latent_encoder/
--rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/latent_encoder/__init__.py
--rw-rw-rw-   0        0        0    11642 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/latent_encoder/autoencoder.py
--rw-rw-rw-   0        0        0     7668 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/lowpass.py
--rw-rw-rw-   0        0        0     5005 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/pipeline.py
--rw-rw-rw-   0        0        0     1674 2024-05-09 18:39:44.000000 audio_upscaler-0.1.1/audio_upscaler/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.748317 audio_upscaler-0.1.1/audio_upscaler/utilities/
--rw-rw-rw-   0        0        0       65 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.752317 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/
--rw-rw-rw-   0        0        0       76 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/__init__.py
--rw-rw-rw-   0        0        0     2752 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/audio_processing.py
--rw-rw-rw-   0        0        0     6521 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/stft.py
--rw-rw-rw-   0        0        0     2602 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/audio/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.755832 audio_upscaler-0.1.1/audio_upscaler/utilities/data/
--rw-rw-rw-   0        0        0       30 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/data/__init__.py
--rw-rw-rw-   0        0        0    15571 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/data/add_on.py
--rw-rw-rw-   0        0        0    20703 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/data/dataset.py
--rw-rw-rw-   0        0        0     5334 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/model.py
--rw-rw-rw-   0        0        0    20126 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/sampler.py
--rw-rw-rw-   0        0        0    18618 2024-04-27 09:12:21.000000 audio_upscaler-0.1.1/audio_upscaler/utilities/tools.py
--rw-rw-rw-   0        0        0    17174 2024-05-09 18:49:38.000000 audio_upscaler-0.1.1/audio_upscaler/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:50:21.755832 audio_upscaler-0.1.1/audio_upscaler.egg-info/
--rw-rw-rw-   0        0        0     4637 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5399 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      243 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 18:50:21.000000 audio_upscaler-0.1.1/audio_upscaler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 18:50:21.758344 audio_upscaler-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3380 2024-05-09 18:50:13.000000 audio_upscaler-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.067887 audio_upscaler-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-26 20:27:22.000000 audio_upscaler-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4637 2024-05-09 19:32:44.065885 audio_upscaler-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3348 2024-04-26 20:27:22.000000 audio_upscaler-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:43.956682 audio_upscaler-0.1.2/audio_upscaler/
+-rw-rw-rw-   0        0        0       28 2024-05-09 18:22:25.000000 audio_upscaler-0.1.2/audio_upscaler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:43.962189 audio_upscaler-0.1.2/audio_upscaler/clap/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:43.981059 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/
+-rw-rw-rw-   0        0        0      664 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/__init__.py
+-rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-rw-   0        0        0    11261 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/factory.py
+-rw-rw-rw-   0        0        0     7369 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/feature_fusion.py
+-rw-rw-rw-   0        0        0    49373 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/htsat.py
+-rw-rw-rw-   0        0        0    16493 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/loss.py
+-rw-rw-rw-   0        0        0    33855 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.000120 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json
+-rw-rw-rw-   0        0        0      520 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-10.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rw-rw-rw-   0        0        0      518 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rw-rw-rw-   0        0        0      519 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14.json
+-rw-rw-rw-   0        0        0      517 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-6.json
+-rw-rw-rw-   0        0        0      409 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/RN101-quickgelu.json
+-rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/RN101.json
+-rw-rw-rw-   0        0        0      411 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/RN50-quickgelu.json
+-rw-rw-rw-   0        0        0      384 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/RN50.json
+-rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/RN50x16.json
+-rw-rw-rw-   0        0        0      385 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/RN50x4.json
+-rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/ViT-B-16.json
+-rw-rw-rw-   0        0        0      334 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-rw-   0        0        0      309 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/ViT-B-32.json
+-rw-rw-rw-   0        0        0      311 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/ViT-L-14.json
+-rw-rw-rw-   0        0        0     5179 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/openai.py
+-rw-rw-rw-   0        0        0    24066 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/pann_model.py
+-rw-rw-rw-   0        0        0     6607 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/pretrained.py
+-rw-rw-rw-   0        0        0     4444 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/timm_model.py
+-rw-rw-rw-   0        0        0     6597 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/tokenizer.py
+-rw-rw-rw-   0        0        0     1096 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/transform.py
+-rw-rw-rw-   0        0        0    12319 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.008119 audio_upscaler-0.1.2/audio_upscaler/clap/training/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/training/__init__.py
+-rw-rw-rw-   0        0        0    84448 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/training/audioset_textmap.npy
+-rw-rw-rw-   0        0        0  1356917 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-rw-   0        0        0    30555 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/clap/training/data.py
+-rw-rw-rw-   0        0        0    17765 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/clap/training/params.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.010484 audio_upscaler-0.1.2/audio_upscaler/hifigan/
+-rw-rw-rw-   0        0        0      238 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/hifigan/__init__.py
+-rw-rw-rw-   0        0        0     5698 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/hifigan/models.py
+-rw-rw-rw-   0        0        0    13214 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/hifigan/models_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.013492 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.016492 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/__init__.py
+-rw-rw-rw-   0        0        0    17995 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/ddim.py
+-rw-rw-rw-   0        0        0    62616 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/ddpm.py
+-rw-rw-rw-   0        0        0    13214 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/plms.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.018948 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/__init__.py
+-rw-rw-rw-   0        0        0    16225 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/attention.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.022956 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/
+-rw-rw-rw-   0        0        0     5540 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/__init__.py
+-rw-rw-rw-   0        0        0    21728 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py
+-rw-rw-rw-   0        0        0     7927 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.030992 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/
+-rw-rw-rw-   0        0        0     1406 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py
+-rw-rw-rw-   0        0        0     1991 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py
+-rw-rw-rw-   0        0        0     2086 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py
+-rw-rw-rw-   0        0        0     2521 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rw-rw-rw-   0        0        0      913 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rw-rw-rw-   0        0        0    14970 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py
+-rw-rw-rw-   0        0        0     4508 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rw-rw-rw-   0        0        0     8838 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rw-rw-rw-   0        0        0     2335 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.035709 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/__init__.py
+-rw-rw-rw-   0        0        0    35531 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py
+-rw-rw-rw-   0        0        0    41336 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rw-rw-rw-   0        0        0    10171 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.036722 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/distributions/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/distributions/__init__.py
+-rw-rw-rw-   0        0        0     3199 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/distributions/distributions.py
+-rw-rw-rw-   0        0        0     3148 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/ema.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.039251 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/encoders/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/encoders/__init__.py
+-rw-rw-rw-   0        0        0    26010 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/encoders/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.043250 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rw-rw-rw-   0        0        0    15295 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rw-rw-rw-   0        0        0     5121 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py
+-rw-rw-rw-   0        0        0     1650 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.046251 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/
+-rw-rw-rw-   0        0        0     1693 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py
+-rw-rw-rw-   0        0        0     3229 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py
+-rw-rw-rw-   0        0        0      651 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py
+-rw-rw-rw-   0        0        0     8084 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.048251 audio_upscaler-0.1.2/audio_upscaler/latent_encoder/
+-rw-rw-rw-   0        0        0        0 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/latent_encoder/__init__.py
+-rw-rw-rw-   0        0        0    11642 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/latent_encoder/autoencoder.py
+-rw-rw-rw-   0        0        0     7668 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/lowpass.py
+-rw-rw-rw-   0        0        0     5005 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/pipeline.py
+-rw-rw-rw-   0        0        0     1679 2024-05-09 19:23:40.000000 audio_upscaler-0.1.2/audio_upscaler/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.054277 audio_upscaler-0.1.2/audio_upscaler/utilities/
+-rw-rw-rw-   0        0        0       65 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.059888 audio_upscaler-0.1.2/audio_upscaler/utilities/audio/
+-rw-rw-rw-   0        0        0       76 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/audio/__init__.py
+-rw-rw-rw-   0        0        0     2752 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/audio/audio_processing.py
+-rw-rw-rw-   0        0        0     6521 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/audio/stft.py
+-rw-rw-rw-   0        0        0     2602 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/audio/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.063894 audio_upscaler-0.1.2/audio_upscaler/utilities/data/
+-rw-rw-rw-   0        0        0       30 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/data/__init__.py
+-rw-rw-rw-   0        0        0    15571 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/data/add_on.py
+-rw-rw-rw-   0        0        0    20703 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/data/dataset.py
+-rw-rw-rw-   0        0        0     5334 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/model.py
+-rw-rw-rw-   0        0        0    20126 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/sampler.py
+-rw-rw-rw-   0        0        0    18618 2024-04-27 09:12:21.000000 audio_upscaler-0.1.2/audio_upscaler/utilities/tools.py
+-rw-rw-rw-   0        0        0    17174 2024-05-09 18:49:38.000000 audio_upscaler-0.1.2/audio_upscaler/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:32:44.064894 audio_upscaler-0.1.2/audio_upscaler.egg-info/
+-rw-rw-rw-   0        0        0     4637 2024-05-09 19:32:43.000000 audio_upscaler-0.1.2/audio_upscaler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5399 2024-05-09 19:32:43.000000 audio_upscaler-0.1.2/audio_upscaler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 19:32:43.000000 audio_upscaler-0.1.2/audio_upscaler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2024-05-09 19:32:43.000000 audio_upscaler-0.1.2/audio_upscaler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 19:32:43.000000 audio_upscaler-0.1.2/audio_upscaler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 19:32:44.067887 audio_upscaler-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3380 2024-05-09 19:32:31.000000 audio_upscaler-0.1.2/setup.py
```

### Comparing `audio_upscaler-0.1.1/LICENSE` & `audio_upscaler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/PKG-INFO` & `audio_upscaler-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_upscaler
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/IAHispano/Audio-Upscaler
 Author: Aitron Emper
 Author-email: aitronssesin@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audio_upscaler-0.1.1/README.md` & `audio_upscaler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/__init__.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/factory.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/feature_fusion.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/htsat.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/loss.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-base.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-large.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/HTSAT-tiny.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-10.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-10.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-18k.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-tiny-transformer.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14-win-1536.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-14.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-14.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/model_configs/PANN-6.json` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/model_configs/PANN-6.json`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/openai.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pann_model.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/pretrained.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/timm_model.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/tokenizer.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/transform.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/open_clip/utils.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/training/audioset_textmap.npy` & `audio_upscaler-0.1.2/audio_upscaler/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audio_upscaler-0.1.2/audio_upscaler/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/training/data.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/clap/training/params.py` & `audio_upscaler-0.1.2/audio_upscaler/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/hifigan/models.py` & `audio_upscaler-0.1.2/audio_upscaler/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/hifigan/models_v2.py` & `audio_upscaler-0.1.2/audio_upscaler/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddim.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/ddpm.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/ddpm.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/models/plms.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/attention.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/distributions/distributions.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/ema.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/encoders/modules.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/modules/phoneme_encoder/text/symbols.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_diffusion/util.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/latent_encoder/autoencoder.py` & `audio_upscaler-0.1.2/audio_upscaler/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/lowpass.py` & `audio_upscaler-0.1.2/audio_upscaler/lowpass.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/pipeline.py` & `audio_upscaler-0.1.2/audio_upscaler/pipeline.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/predict.py` & `audio_upscaler-0.1.2/audio_upscaler/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             latent_t_per_second=12.8
         )
         out_wav = (waveform[0] * 32767).astype(np.int16).T
         if not output_file:
             output_file = os.path.join(os.path.dirname(input_file), f"{os.path.splitext(os.path.basename(input_file))[0]}" + "_output.wav")
         sf.write(output_file, data=out_wav, samplerate=sr)
 
-def upscale(input_file, output_file, sr=48000, ddim_steps=50, guidance_scale=3.5, model_name="basic", device="auto", seed=None):
+def upscale(input_file, output_file=None, sr=48000, ddim_steps=50, guidance_scale=3.5, model_name="basic", device="auto", seed=None):
     p = Predictor()
     p.setup(model_name, device)
     p.predict(
         input_file,
         output_file,
         sr=sr,
         ddim_steps=ddim_steps,
```

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/audio/audio_processing.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/audio/stft.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/audio/tools.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/data/add_on.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/data/dataset.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/model.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/sampler.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utilities/tools.py` & `audio_upscaler-0.1.2/audio_upscaler/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler/utils.py` & `audio_upscaler-0.1.2/audio_upscaler/utils.py`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/audio_upscaler.egg-info/PKG-INFO` & `audio_upscaler-0.1.2/audio_upscaler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_upscaler
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/IAHispano/Audio-Upscaler
 Author: Aitron Emper
 Author-email: aitronssesin@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audio_upscaler-0.1.1/audio_upscaler.egg-info/SOURCES.txt` & `audio_upscaler-0.1.2/audio_upscaler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audio_upscaler-0.1.1/setup.py` & `audio_upscaler-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audio_upscaler"
 DESCRIPTION = "This package is written for text-to-audio/music generation."
 URL = "https://github.com/IAHispano/Audio-Upscaler"
 EMAIL = "aitronssesin@gmail.com"
 AUTHOR = "Aitron Emper"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

