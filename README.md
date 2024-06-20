# Auto Installers : https://www.patreon.com/posts/105251204
# This repo is for premium scripts : https://www.patreon.com/posts/105251204

---
tags:
  - text-to-image
  - stable-diffusion
  - audio-to-video
license: apache-2.0
language:
  - en
library_name: diffusers
---

# V-Express Model Card

<div align="center">

[**Project Page**](https://tenvence.github.io/p/v-express/) **|** [**Paper**](https://arxiv.org/abs/2406.02511) **|** [**Code**](https://github.com/tencent-ailab/V-Express)

</div>

---

## Introduction

## Models

### Audio Encoder

- [model_ckpts/wav2vec2-base-960h](https://huggingface.co/tk93/V-Express/tree/main/model_ckpts/wav2vec2-base-960h). (It is also available from the original model card [facebook/wav2vec2-base-960h](https://huggingface.co/facebook/wav2vec2-base-960h))

### Face Analysis

- [model_ckpts/insightface_models/models/buffalo_l](https://huggingface.co/tk93/V-Express/tree/main/model_ckpts/insightface_models/models/buffalo_l). (It is also available from the original repository [insightface/buffalo_l](https://github.com/deepinsight/insightface/releases/download/v0.7/buffalo_l.zip))

### V-Express

- [model_ckpts/sd-vae-ft-mse](https://huggingface.co/tk93/V-Express/tree/main/model_ckpts/sd-vae-ft-mse). VAE encoder. (original model card [stabilityai/sd-vae-ft-mse](https://huggingface.co/stabilityai/sd-vae-ft-mse))
- [model_ckpts/stable-diffusion-v1-5](https://huggingface.co/tk93/V-Express/tree/main/model_ckpts/stable-diffusion-v1-5). Only the model configuration file for unet is needed here. (original model card [runwayml/stable-diffusion-v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5))
- [model_ckpts/v-express](https://huggingface.co/tk93/V-Express/tree/main/model_ckpts/v-express). The video generation model conditional on audio and V-kps we call V-Express.
- You should download and put all `.bin` model to `model_ckpts/v-express` directory, which includes `audio_projection.bin`, `denoising_unet.bin`, `motion_module.bin`, `reference_net.bin`, and `v_kps_guider.bin`.
