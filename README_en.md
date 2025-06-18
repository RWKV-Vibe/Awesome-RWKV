[中文版本](README.md)

---

# Awesome RWKV: A Curated List of Projects

A curated list of awesome projects, tools, and resources in the RWKV ecosystem.

## Table of Contents

- [Official RWKV Links](#official-rwkv-links)
- [RWKV Fine-tuning & Training](#rwkv-fine-tuning--training)
  - [Fine-tuning Projects](#fine-tuning-projects)
  - [Training Projects](#training-projects)
- [Model Architecture & Optimization](#model-architecture--optimization)
- [Image & Graphics](#image--graphics)
  - [Vision-Language](#vision-language)
  - [Vision Backbone](#vision-backbone)
  - [Image Classification](#image-classification)
  - [Image Segmentation](#image-segmentation)
  - [Image Generation](#image-generation)
  - [Object Detection](#object-detection)
  - [Other Image Tasks](#other-image-tasks)
- [Audio](#audio)
- [Time Series](#time-series)
- [Robotics & Embodied AI](#robotics--embodied-ai)
- [RWKV Tokenizers](#rwkv-tokenizers)
- [RWKV RAG Systems](#rwkv-rag-systems)
- [Chatbots & Inference API Servers](#chatbots--inference-api-servers)
- [RWKV Benchmarks](#rwkv-benchmarks)
- [RWKV Inference Frameworks & Operator Libraries](#rwkv-inference-frameworks--operator-libraries)
- [Other RWKV Projects](#other-rwkv-projects)

---

## Official RWKV Links

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-LM | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM) | | The official code repository for RWKV, providing architecture code for RWKV v1 to v7 and corresponding large language model training implementations. |
| RWKV-4 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v4) | [![arXiv:2305.13048](https://img.shields.io/badge/arXiv-2305.13048-b31b1b.svg)](https://arxiv.org/abs/2305.13048) | The architecture paper for RWKV-4. |
| RWKV 5/6 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v5) | [![arXiv:2404.05892](https://img.shields.io/badge/arXiv-2404.05892-b31b1b.svg)](https://arxiv.org/abs/2404.05892) | The architecture paper for RWKV-5/6. |
| RWKV-7 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v7)| [![arXiv:2503.14456](https://img.shields.io/badge/arXiv-2503.14456-b31b1b.svg)](https://arxiv.org/abs/2503.14456) | The architecture paper for RWKV-7. |
| RWKV pip Package | [![PyPI - Downloads](https://img.shields.io/pypi/dm/rwkv.svg)](https://pypi.org/project/rwkv/) | | The official pip package for RWKV. See the [RWKV official website](https://rwkv.com/tutorials/intermediate/RWKVpip) for usage. |
| RWKV-CUDA | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-CUDA.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-CUDA) | | Official CUDA operators for RWKV. |
| Hugging Face Docs | [![Hugging Face Docs](https://img.shields.io/badge/Hugging%20Face-Docs-blue)](https://huggingface.co/docs/transformers/model_doc/rwkv) | | Hugging Face's documentation on RWKV. |
| rwkvcn-docs | [![Star](https://img.shields.io/github/stars/LeoLin4258/rwkvcn-docs.svg?style=social&label=Star)](https://github.com/LeoLin4258/rwkvcn-docs) | | Project link for the Chinese documentation of RWKV. |
| RWKV.com | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV.com.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV.com) | | Project link for the official English website of RWKV. |

---

## RWKV Fine-tuning & Training

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|RWKV-Development-Tools | [![Star](https://img.shields.io/github/stars/Ourboros-Alignment-Team/RWKV-Development-Tools.svg?style=social&label=Star)](https://github.com/Ourboros-Alignment-Team/RWKV-Development-Tools) | | A research platform for RWKV models, a feature-rich integrated toolkit. |

### Fine-tuning Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| **⭐ (Recommended)** RWKV-PEFT | [![Star](https://img.shields.io/github/stars/JL-er/RWKV-PEFT.svg?style=social&label=Star)](https://github.com/JL-er/RWKV-PEFT) | | An efficient fine-tuning repository for RWKV, including methods like LoRA, Pissa, Lisa, and State. |
| RWKV-PEFT-Simple | [![Star](https://img.shields.io/github/stars/Seikaijyu/RWKV-PEFT-Simple.svg?style=social&label=Star)](https://github.com/Seikaijyu/RWKV-PEFT-Simple) | | A simplified version of RWKV-PEFT with convenient scripts and fine-tuning instructions. |
| **🚧 (In Development)** RWKV-LM-RLHF | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-LM-RLHF.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-LM-RLHF) | | A Reinforcement Learning (RLHF) toolkit for RWKV, including SFT and alignment methods (DPO, ORPO). |
| RWKV-LM-RLHF-DPO | [![Star](https://img.shields.io/github/stars/Triang-jyed-driung/RWKV-LM-RLHF-DPO.svg?style=social&label=Star)](https://github.com/Triang-jyed-driung/RWKV-LM-RLHF-DPO) | | An implementation of Direct Preference Optimization (DPO) for RWKV. |
| **⚠️ (Potentially Outdated)** RWKV-LoRA | [![Star](https://img.shields.io/github/stars/Blealtan/RWKV-LM-LoRA.svg?style=social&label=Star)](https://github.com/Blealtan/RWKV-LM-LoRA) | | A LoRA fine-tuning implementation for RWKV, does not support RWKV-6 or newer versions. |

### Training Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| wind_rwkv | [![Star](https://img.shields.io/github/stars/johanwind/wind_rwkv.svg?style=social&label=Star)](https://github.com/johanwind/wind_rwkv) | | A repository containing optimized kernels for RWKV language models, currently focusing on RWKV-7. |
| RWKV-LM-V7 | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/RWKV-LM-V7.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/RWKV-LM-V7) | | RWKV-LM-V7 is a user-friendly training project for RWKV-7 multi-class models, allowing developers to start training in 15 minutes. |
| RWKV-LM-V7-AMD-ROCm | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV-LM-V7-AMD-ROCm.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV-LM-V7-AMD-ROCm7) | | RWKV-LM-V7 adapted for AMD ROCm. |
| RWKV-infctx-trainer | [![Star](https://img.shields.io/github/stars/RWKV/RWKV-infctx-trainer.svg?style=social&label=Star)](https://github.com/RWKV/RWKV-infctx-trainer/) | | An infinite context trainer for RWKV, supporting training contexts of 10k and longer. |
| RWKV-Ouroboros | [![Star](https://img.shields.io/github/stars/neromous/RWKV-Ouroboros.svg?style=social&label=Star)](https://github.com/neromous/RWKV-Ouroboros) | | An API-based rwkv-trainer project that supports alternating between training and inference. |
| nanoRWKV | [![Star](https://img.shields.io/github/stars/Hannibal046/nanoRWKV.svg?style=social&label=Star)](https://github.com/Hannibal046/nanoRWKV) | | A nanoGPT-style implementation of the RWKV model. |
| RWKV_LM_EXT | [![Star](https://img.shields.io/github/stars/yynil/RWKV_LM_EXT.svg?style=social&label=Star)](https://github.com/yynil/RWKV_LM_EXT) | | Implements functional extensions for RWKV, including sequence classification, embedding, PEFT, cross-encoder, bi-encoder, and multi-modality. |
| chunkRWKV6 | [![Star](https://img.shields.io/github/stars/00ffcc/chunkRWKV6.svg?style=social&label=Star)](https://github.com/00ffcc/chunkRWKV6) | | Optimizes RWKV prefill and training speed using chunked parallelism. |

---

## Model Architecture & Optimization

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|RWKVQuant|[![Star](https://img.shields.io/github/stars/xuchen-dev/RWKVQuant.svg?style=social&label=Star)](https://github.com/xuchen-dev/RWKVQuant)| [![arXiv:2505.03803](https://img.shields.io/badge/arXiv-2505.03803-b31b1b.svg)](https://arxiv.org/abs/2505.03803)| Efficient quantization for the RWKV series models. |
|RWKV-X|[![Star](https://img.shields.io/github/stars/howard-hou/RWKV-X.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-X)|[![arXiv:2504.21463](https://img.shields.io/badge/arXiv-2504.21463-b31b1b.svg)](https://arxiv.org/abs/2504.21463)| A linear-complexity mixture-of-experts language model based on the RWKV architecture. |
|ARWKV|[![Star](https://img.shields.io/github/stars/yynil/RWKVInside.svg?style=social&label=Star)](https://github.com/yynil/RWKVInside)|[![arXiv:2501.15570](https://img.shields.io/badge/arXiv-2501.15570-b31b1b.svg)](https://arxiv.org/abs/2501.15570)| A hybrid-attention language model based on RWKV. |

---

## Image & Graphics

### Vision-Language

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| VisualRWKV | [![Star](https://img.shields.io/github/stars/howard-hou/VisualRWKV.svg?style=social&label=Star)](https://github.com/howard-hou/VisualRWKV) | | A vision-language model based on RWKV for handling visual tasks. |
| RWKV-CLIP | [![Star](https://img.shields.io/github/stars/deepglint/RWKV-CLIP.svg?style=social&label=Star)](https://github.com/deepglint/RWKV-CLIP) | [![arXiv:2406.06973](https://img.shields.io/badge/arXiv-2406.06973-b31b1b.svg)](https://arxiv.org/abs/2406.06973) |  [EMNLP 2024] An RWKV-powered CLIP model for vision-language representation learning. |

### Vision Backbone

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Vision-RWKV (New Gen) | [![Star](https://img.shields.io/github/stars/xforcevesa/new-vrwkv.svg?style=social&label=Star)](https://github.com/xforcevesa/new-vrwkv) | | A new generation of RWKV for Vision, based on RWKV-7. |
| Vision-RWKV | [![Star](https://img.shields.io/github/stars/OpenGVLab/Vision-RWKV.svg?style=social&label=Star)](https://github.com/OpenGVLab/Vision-RWKV) | [![arXiv:2403.02308](https://img.shields.io/badge/arXiv-2403.02308-b31b1b.svg)](https://arxiv.org/abs/2403.02308)|  [ICLR 2025 Spotlight] A visual perception model based on RWKV that can smoothly process high-resolution images. |
| PointRWKV | [![Star](https://img.shields.io/github/stars/hithqd/PointRWKV.svg?style=social&label=Star)](https://github.com/hithqd/PointRWKV) |[![arXiv:2405.15214](https://img.shields.io/badge/arXiv-2405.15214-b31b1b.svg)](https://arxiv.org/abs/2405.15214) |  [AAAI 2025] A 3D point cloud learning framework based on RWKV. |

### Image Classification

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|Vision_QRWKV|[![Star](https://img.shields.io/github/stars/ChiShengChen/Vision_QRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/Vision_QRWKV)|[![arXiv:2506.06633](https://img.shields.io/badge/arXiv-2506.06633-b31b1b.svg)](https://arxiv.org/abs/2506.06633)| A Quantum-Enhanced RWKV Model for Image Classification. |

### Image Segmentation

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| U-RWKV | [![Star](https://img.shields.io/github/stars/hbyecoding/U-RWKV.svg?style=social&label=Star)](https://github.com/hbyecoding/U-RWKV) | | An image segmentation model based on RWKV. |
| RWKV-SAM | [![Star](https://img.shields.io/github/stars/HarborYuan/ovsam.svg?style=social&label=Star)](https://github.com/HarborYuan/ovsam) | [![arXiv:2401.02955](https://img.shields.io/badge/arXiv-2401.02955-b31b1b.svg)](https://arxiv.org/abs/2401.02955)|  [ECCV 2024] "RWKV-SAM": An open-vocabulary image segmentation method based on RWKV. |
|MMSegRWKV|[![Star](https://img.shields.io/github/stars/supercyt/MMSegRWKV.svg?style=social&label=Star)](https://github.com/supercyt/MMSegRWKV)|| A multi-modal Magnetic Resonance Imaging (MRI) segmentation model developed on the RWKV architecture. |

### Image Generation

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Diffusion-RWKV | [![Star](https://img.shields.io/github/stars/feizc/Diffusion-RWKV.svg?style=social&label=Star)](https://github.com/feizc/Diffusion-RWKV) |[![arXiv:2404.04478](https://img.shields.io/badge/arXiv-2404.04478-b31b1b.svg)](https://arxiv.org/abs/2404.04478) | An RWKV-based model for image generation tasks, excelling at handling high-resolution images. |

### Object Detection

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| LION | [![Star](https://img.shields.io/github/stars/happinesslz/LION.svg?style=social&label=Star)](https://github.com/happinesslz/LION) | [![arXiv:2407.18232](https://img.shields.io/badge/arXiv-2407.18232-b31b1b.svg)](https://arxiv.org/abs/2407.18232)|  [NeurIPS 2024] Linear Group RNN for 3D Object Detection in Point Clouds (with RWKV support). |
|RWKV-VG| [![Star](https://img.shields.io/github/stars/nianfd/RWKV-VG.svg?style=social&label=Star)](https://github.com/nianfd/RWKV-VG)|[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00530-025-01720-w)| A visual grounding framework based on the RWKV architecture. |

### Other Image Tasks

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| FEAT | [![Star](https://img.shields.io/github/stars/Yaziwel/FEAT.svg?style=social&label=Star)](https://github.com/Yaziwel/FEAT) |[![arXiv:2506.04956](https://img.shields.io/badge/arXiv-2506.04956-b31b1b.svg)](https://arxiv.org/abs/2506.04956) |  [MICCAI 2025 early accepted] RWKV-based medical video generation. |
|LALIC|[![Star](https://img.shields.io/github/stars/sjtu-medialab/RwkvCompress.svg?style=social&label=Star)](https://github.com/sjtu-medialab/RwkvCompress)|[![arXiv:2502.05741](https://img.shields.io/badge/arXiv-2502.05741-b31b1b.svg)](https://arxiv.org/abs/2502.05741)|  [CVOR 2025] An image compression framework based on RWKV. |
| Restore-RWKV | [![Star](https://img.shields.io/github/stars/Yaziwel/Restore-RWKV.svg?style=social&label=Star)](https://github.com/Yaziwel/Restore-RWKV) |[![arXiv:2407.11087](https://img.shields.io/badge/arXiv-2407.11087-b31b1b.svg)](https://arxiv.org/abs/2407.11087) | Efficient and effective medical image restoration using RWKV (PyTorch implementation). |
| LineRWKV | [![Star](https://img.shields.io/github/stars/diegovalsesia/linerwkv.svg?style=social&label=Star)](https://github.com/diegovalsesia/linerwkv) | [![arXiv:2403.17677](https://img.shields.io/badge/arXiv-2403.17677-b31b1b.svg)](https://arxiv.org/abs/2403.17677)| A method for lossless and lossy compression of hyperspectral images using RWKV. |
|OpenPAR|[![Star](https://img.shields.io/github/stars/Event-AHU/OpenPAR.svg?style=social&label=Star)](https://github.com/Event-AHU/OpenPAR)| [![arXiv:2504.10018](https://img.shields.io/badge/arXiv-2504.10018-b31b1b.svg)](https://arxiv.org/abs/2504.10018)| An open-source framework for Pedestrian Attribute Recognition, including RWKV. |

---

## Audio

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|MIDI-RWKV|[![Star](https://img.shields.io/github/stars/christianazinn/MIDI-RWKV.svg?style=social&label=Star)](https://github.com/christianazinn/MIDI-RWKV)|[![arXiv:2506.13001](https://img.shields.io/badge/arXiv-2506.13001-b31b1b.svg)](https://arxiv.org/abs/2506.13001)| Music generation based on RWKV. |
| RWKV-TTS | [![Star](https://img.shields.io/github/stars/yynil/RWKVTTS.svg?style=social&label=Star)](https://github.com/yynil/RWKVTTS) | [![arXiv:2504.03289](https://img.shields.io/badge/arXiv-2504.03289-b31b1b.svg)](https://arxiv.org/abs/2504.03289) | An RWKV-based Text-to-Speech (TTS) model supporting multiple languages. |
| RWKV-ASR | [![Star](https://img.shields.io/github/stars/AGENDD/RWKV-ASR.svg?style=social&label=Star)](https://github.com/AGENDD/RWKV-ASR) | | **Automatic Speech Recognition (ASR)** using a pre-trained RWKV language model. |

---

## Time Series

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| BlackGoose_Rimer | [![Star](https://img.shields.io/github/stars/Alic-Li/BlackGoose_Rimer.svg?style=social&label=Star)](https://github.com/Alic-Li/BlackGoose_Rimer) |[![arXiv:2503.06121](https://img.shields.io/badge/arXiv-2503.06121-b31b1b.svg)](https://arxiv.org/abs/2503.06121) | A time series forecasting model based on RWKV-7, supporting various time series tasks. |
| RWKV-TS | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-TS.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-TS) | | An RWKV-based model for time series tasks with low latency and memory footprint. |

---

## Robotics & Embodied AI

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| DecisionRWKV | [![Star](https://img.shields.io/github/stars/ancorasir/DecisionRWKV.svg?style=social&label=Star)](https://github.com/ancorasir/DecisionRWKV) | [![arXiv:2407.16306](https://img.shields.io/badge/arXiv-2407.16306-b31b1b.svg)](https://arxiv.org/abs/2407.16306)| [JCISE] A lifelong learning algorithm for robots using experience replay + Decision-RWKV. |
| OccRWKV | [![Star](https://img.shields.io/github/stars/jmwang0117/OccRWKV.svg?style=social&label=Star)](https://github.com/jmwang0117/OccRWKV) | [![arXiv:2409.19987](https://img.shields.io/badge/arXiv-2409.19987-b31b1b.svg)](https://arxiv.org/abs/2409.19987)| [ICRA 2025] Efficient 3D semantic occupancy prediction with linear complexity. |

---

## RWKV Tokenizers

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| rwkv-tokenizer | [![Star](https://img.shields.io/github/stars/cahya-wirawan/rwkv-tokenizer.svg?style=social&label=Star)](https://github.com/cahya-wirawan/rwkv-tokenizer) | | A fast RWKV Tokenizer written in Rust, supporting RWKV-V5/6 World models. |
| rwkv_tokenizer.c | [![Star](https://img.shields.io/github/stars/mrsteyk/rwkv_tokenizer.c.svg?style=social&label=Star)](https://github.com/mrsteyk/rwkv_tokenizer.c) | | A Trie-based RWKV tokenizer written in C. |
| rwkv-tokenizer-go | [![Star](https://img.shields.io/github/stars/Ronsor/rwkv-tokenizer-go.svg?style=social&label=Star)](https://github.com/Ronsor/rwkv-tokenizer-go) | | An RWKV tokenizer for the Go language. |
| RWKV-World-Tokenizer-CPP | [![Star](https://img.shields.io/github/stars/m8than/RWKV-World-Tokenizer-CPP.svg?style=social&label=Star)](https://github.com/m8than/RWKV-World-Tokenizer-CPP) | | A highly optimized trie-based tokenizer for RWKV World models, written in C++. |

---

## RWKV RAG Systems

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-RAG | [![Star](https://img.shields.io/github/stars/AIIRWKV/RWKV-RAG.svg?style=social&label=Star)](https://github.com/AIIRWKV/RWKV-RAG) | | A one-click RAG deployment system based on RWKV, enabling easy setup of local knowledge bases, a Q&A bot, and one-click fine-tuning. |

---

## Chatbots & Inference API Servers

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| **⭐ (Chinese Recommended)** RWKV Runner | [![Star](https://img.shields.io/github/stars/josStorer/RWKV-Runner.svg?style=social&label=Star)](https://github.com/josStorer/RWKV-Runner) | | A management and launcher tool for RWKV models with a user-friendly GUI, supporting both training and inference. |
| **⭐ (Chinese Recommended)** AI00 RWKV Server | [![Star](https://img.shields.io/github/stars/cgisky1980/ai00_rwkv_server.svg?style=social&label=Star)](https://github.com/cgisky1980/ai00_rwkv_server) | | An **inference API server** for RWKV models, built on the web-rwkv inference engine. |
|RWKV_APP|[![Star](https://img.shields.io/github/stars/RWKV-APP/RWKV_APP.svg?style=social&label=Star)](https://github.com/RWKV-APP/RWKV_APP)|| An on-device RWKV-LM inference App implemented with Flutter. |
| **🇨🇳 (Chinese)** Wenda Web UI | [![Star](https://img.shields.io/github/stars/wenda-LLM/wenda.svg?style=social&label=Star)](https://github.com/wenda-LLM/wenda) | | An LLM invocation platform for generating content in specific domains, with support for RWKV models. |
| **🇨🇳 (Chinese)** Role Play Chatbot | [![Star](https://img.shields.io/github/stars/shengxia/RWKV_Role_Playing.svg?style=social&label=Star)](https://github.com/shengxia/RWKV_Role_Playing) | | An RWKV-based role-playing WebUI built with Gradio. |
| Easy_RWKV_webui | [![Star](https://img.shields.io/github/stars/No-22-Github/Easy_RWKV_webui.svg?style=social&label=Star)](https://github.com/No-22-Github/Easy_RWKV_webui) | | An online chat room for RWKV models, built with PyWebIO. |
| Mini Model Daemon | [![Star](https://img.shields.io/github/stars/recursal/minmodmon.svg?style=social&label=Star)](https://github.com/recursal/minmodmon) | | An inference tool for RWKV models, using the web-rwkv backend. |
| LocalAI | [![Star](https://img.shields.io/github/stars/go-skynet/LocalAI.svg?style=social&label=Star)](https://github.com/go-skynet/LocalAI) | | An open-source OpenAI alternative with RWKV support. |
| GPT Academic | [![Star](https://img.shields.io/github/stars/binary-husky/gpt_academic.svg?style=social&label=Star)](https://github.com/binary-husky/gpt_academic) | | A practical interface for LLMs like GPT/GLM, with support for RWKV. |
| LLMFarm | [![Star](https://img.shields.io/github/stars/guinmoon/LLMFarm.svg?style=social&label=Star)](https://github.com/guinmoon/LLMFarm) | | Run large language models offline on iOS and macOS using the GGML library, with RWKV support. |

---

## RWKV Benchmarks

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Uncheatable Eval | [![Star](https://img.shields.io/github/stars/Jellyfish042/uncheatable_eval.svg?style=social&label=Star)](https://github.com/Jellyfish042/uncheatable_eval) | | A benchmark for testing LLM performance with up-to-date dynamic data, including RWKV. |
| RULER_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/RULER_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/RULER_RWKV) | | [RULER](https://arxiv.org/abs/2404.06654) benchmark scores for RWKV models. |
| LongBench_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/LongBench_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/LongBench_RWKV) | | [LongBench](https://arxiv.org/abs/2308.14508) benchmark scores for RWKV models. |
| rwkv_mmlu | [![Star](https://img.shields.io/github/stars/Jellyfish042/rwkv_mmlu.svg?style=social&label=Star)](https://github.com/Jellyfish042/rwkv_mmlu) | | MMLU benchmark scores for RWKV models. |

---

## RWKV Inference Frameworks & Operator Libraries

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|cann-ops-rwkv|[![Star](https://img.shields.io/github/stars/appleinsky/rwkv_Ascend.svg?style=social&label=Star)](https://github.com/appleinsky/rwkv_Ascend)||Operator repository for Ascend, co-developed with RWKV.|
| rwkv7.c | [![Star](https://img.shields.io/github/stars/KevlarKanou/rwkv7.c.svg?style=social&label=Star)](https://github.com/KevlarKanou/rwkv7.c) | | A C implementation for RWKV-7 model inference. |
| rwkv.cpp | [![Star](https://img.shields.io/github/stars/RWKV/rwkv.cpp.svg?style=social&label=Star)](https://github.com/RWKV/rwkv.cpp) | | Inference for RWKV models on CPU, supporting FP16 and INT4/INT5/INT8 quantization. |
| RWKVSharp | [![Star](https://img.shields.io/github/stars/imxcstar/RWKVSharp.svg?style=social&label=Star)](https://github.com/imxcstar/RWKVSharp) | | A C# wrapper for RWKV inference based on rwkv.cpp, supporting RWKV4/RWKV5/RWKV6/RWKV7 World models. |
| RWKV_Pytorch | [![Star](https://img.shields.io/github/stars/yuunnn-w/RWKV_Pytorch.svg?style=social&label=Star)](https://github.com/yuunnn-w/RWKV_Pytorch) | | An RWKV model inference framework implemented purely in native PyTorch. |
| rwkv-kit | [![Star](https://img.shields.io/github/stars/TorchRWKV/rwkv-kit.svg?style=social&label=Star)](https://github.com/TorchRWKV/rwkv-kit) | | An RWKV model inference framework supporting batch inference, parallel training, and more. |
| web-rwkv | [![Star](https://img.shields.io/github/stars/cryscan/web-rwkv.svg?style=social&label=Star)](https://github.com/cryscan/web-rwkv) | | An implementation of RWKV model inference in pure WebGPU/Rust. |
| candle-rwkv | [![Star](https://img.shields.io/github/stars/nkypy/candle-rwkv.svg?style=social&label=Star)](https://github.com/nkypy/candle-rwkv) | | An implementation of RWKV model inference in Candle, a minimalist ML framework for Rust (with quantization support). |
| **🚧 (Under Construction)** RWKV7-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV7-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV7-Keras) | | A Keras implementation of the RWKV model, supporting training and inference. |
| RWKV6-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV6-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV6-Keras) | | A Keras implementation of the RWKV model, supporting training and inference. |
| rwkv-burn| [![Star](https://img.shields.io/github/stars/dymat/rwkv-burn.svg?style=social&label=Star)](https://github.com/dymat/rwkv-burn) | | A Burn implementation of the RWKV language model. |
| jaxrwkv | [![Star](https://img.shields.io/github/stars/bsarkar321/jaxrwkv.svg?style=social&label=Star)](https://github.com/bsarkar321/jaxrwkv) | | A JAX implementation of the RWKV language model. |
| **🚧 (In Development)** rwkv-mobile | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-mobile.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-mobile) | | An on-device mobile inference engine for RWKV. |
| rwkv-qualcomm | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-qualcomm.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-qualcomm) | | RWKV model inference using the Qualcomm AI Engine Direct SDK. |
| rwkv-by-hand-excel | [![Star](https://img.shields.io/github/stars/playaswd/rwkv-by-hand-excel.svg?style=social&label=Star)](https://github.com/playaswd/rwkv-by-hand-excel) | | An implementation of RWKV in Excel to help developers understand its principles. |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) | | RWKV-V6/V7 inference using FLA, supporting inference with multiple combined states. |
| MLC LLM | [![Star](https://img.shields.io/github/stars/mlc-ai/mlc-llm.svg?style=social&label=Star)](https://github.com/mlc-ai/mlc-llm) | | A machine learning compiler and high-performance deployment engine with support for RWKV models. |

---

## Other RWKV Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|SocialDeductionLLM|[![Star](https://img.shields.io/github/stars/SocialDeductionLLM/SocialDeductionLLM.svg?style=social&label=Star)](https://github.com/SocialDeductionLLM/SocialDeductionLLM)|[![arXiv:2502.06060](https://img.shields.io/badge/arXiv-2502.06060-b31b1b.svg)](https://arxiv.org/abs/2502.06060)| [AAMAS 2025] Multi-Agent Reinforcement Learning. |
|ARIES|[![Star](https://img.shields.io/github/stars/Chieko-Seren/ARIES.svg?style=social&label=Star)](https://github.com/Chieko-Seren/ARIES)|| An automated operations system with RWKV support. |
| SpikeGPT | [![Star](https://img.shields.io/github/stars/ridgerchu/SpikeGPT.svg?style=social&label=Star)](https://github.com/ridgerchu/SpikeGPT) | | A novel model inspired by RWKV. |
| JSONL to binidx | [![Star](https://img.shields.io/github/stars/Abel2076/json2binidx_tool.svg?style=social&label=Star)](https://github.com/Abel2076/json2binidx_tool) | | A tool to convert `.jsonl` files to the `.bin`/`.idx` (binidx) format suitable for RWKV training. |
| AI Town - RWKV Proxy | [![Star](https://img.shields.io/github/stars/recursal/ai-town-rwkv-proxy.svg?style=social&label=Star)](https://github.com/recursal/ai-town-rwkv-proxy?tab=readme-ov-file) | | Run a large-scale AI Town locally with RWKV! |
| Bot-Ani-RWKV | [![Star](https://img.shields.io/github/stars/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection.svg?style=social&label=Star)](https://github.com/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection) | | An RWKV-based Twitter bot detection tool. |
| RWKVInverseFolding | [![Star](https://img.shields.io/github/stars/Lyttr/RWKVInverseFolding.svg?style=social&label=Star)](https://github.com/Lyttr/RWKVInverseFolding) | | Inverse protein folding using RWKV. |
| poker-ai-rwkv | [![Star](https://img.shields.io/github/stars/meraline/poker-ai-rwkv.svg?style=social&label=Star)](https://github.com/meraline/poker-ai-rwkv) | | An AI poker playing system with RWKV. |
|Muon-RMS-Norm|[![Star](https://img.shields.io/github/stars/xTimeCrystal/Muon-RMS-Norm.svg?style=social&label=Star)](https://github.com/xTimeCrystal/Muon-RMS-Norm)|||