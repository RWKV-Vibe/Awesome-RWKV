[中文版](README.md)

---

# Awesome RWKV

A curated list of awesome projects, tools, and resources in the RWKV ecosystem.

## Table of Contents

- [Official RWKV Links](#official-rwkv-links)
- [RWKV Fine-tuning & Training](#rwkv-fine-tuning--training)
  - [Fine-tuning Projects](#fine-tuning-projects)
  - [Training Projects](#training-projects)
- [Natural Language Processing / Large Models](#natural-language-processing--large-language-models)
  - [Model Architecture & Optimization](#model-architecture--optimization)
  - [Natural Language Processing](#natural-language-processing)
  - [Multimodality](#multimodality)
- [Image & Graphics](#image--graphics)
  - [Vision-Language](#vision-language)
  - [Vision Backbone](#vision-backbone)
  - [Image Classification](#image-classification)
  - [Image Segmentation](#image-segmentation)
  - [Image Generation](#image-generation)
  - [Object Detection](#object-detection)
  - [Super-Resolution](#super-resolution)
  - [Image Denoising / Enhancement](#image-denoising--enhancement)
  - [Other Image Tasks](#other-image-tasks)
- [3D & Video Processing](#3d--video-processing)
- [Audio Related](#audio-related)
- [Time Series](#time-series)
- [Robotics & Embodied AI](#robotics--embodied-ai)
- [RWKV Tokenizers](#rwkv-tokenizers)
- [RAG Systems for RWKV](#rag-systems-for-rwkv)
- [Chatbots & Inference API Servers](#chatbots--inference-api-servers)
- [RWKV Benchmarks](#rwkv-benchmarks)
- [Inference Frameworks & Operator Libraries](#inference-frameworks--operator-libraries)
- [Other RWKV Projects](#other-rwkv-projects)

---

## Official RWKV Links

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-LM | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM) | | The official code repository for RWKV, providing architecture code for versions v1 to v7, along with implementations for large language model training. |
| RWKV-4 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v4) | [![arXiv:2305.13048](https://img.shields.io/badge/arXiv-2305.13048-b31b1b.svg)](https://arxiv.org/abs/2305.13048) | The architecture paper for RWKV-4. |
| RWKV 5/6 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v5) | [![arXiv:2404.05892](https://img.shields.io/badge/arXiv-2404.05892-b31b1b.svg)](https://arxiv.org/abs/2404.05892) | The architecture paper for RWKV-5/6. |
| RWKV-7 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v7)| [![arXiv:2503.14456](https://img.shields.io/badge/arXiv-2503.14456-b31b1b.svg)](https://arxiv.org/abs/2503.14456) | The architecture paper for RWKV-7. |
| RWKV pip Package | [![PyPI](https://img.shields.io/pypi/v/rwkv.svg)](https://pypi.org/project/rwkv/)| | The pip package for RWKV. For usage, see the [official RWKV website](https://rwkv.com/tutorials/intermediate/RWKVpip). |
| RWKV-CUDA | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-CUDA.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-CUDA) | | Official CUDA operators for RWKV. |
| Hugging Face Docs | [![🤗 RWKV](https://img.shields.io/badge/🤗%20RWKV-blue)](https://huggingface.co/docs/transformers/model_doc/rwkv) | | Hugging Face's introduction to RWKV. |
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
| **⭐ (Recommended)** RWKV-PEFT | [![Star](https://img.shields.io/github/stars/JL-er/RWKV-PEFT.svg?style=social&label=Star)](https://github.com/JL-er/RWKV-PEFT) | | An efficient fine-tuning repository for RWKV, including various methods like LoRA, Pissa, DiSHA, and State. |
| RWKV-PEFT-Simple | [![Star](https://img.shields.io/github/stars/Seikaijyu/RWKV-PEFT-Simple.svg?style=social&label=Star)](https://github.com/Seikaijyu/RWKV-PEFT-Simple) | | A simplified version of RWKV-PEFT, providing convenient scripts and fine-tuning instructions. |
| **🚧 (In Development)** RWKV-LM-RLHF | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-LM-RLHF.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-LM-RLHF) | | A Reinforcement Learning (RLHF) toolkit for RWKV, including SFT, alignment (DPO, ORPO), etc. |

### Training Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| wind_rwkv | [![Star](https://img.shields.io/github/stars/johanwind/wind_rwkv.svg?style=social&label=Star)](https://github.com/johanwind/wind_rwkv) | | A repository containing optimized kernels for the RWKV language model. Currently focused on RWKV-7. |
| RWKV-LM-V7 | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/RWKV-LM-V7.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/RWKV-LM-V7) | | RWKV-LM-V7 is a user-friendly RWKV-7 multi-class model training project, allowing developers to start training RWKV-7 models within 15 minutes. |
| RWKV-LM-V7-AMD-ROCm | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV-LM-V7-AMD-ROCm.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV-LM-V7-AMD-ROCm) | | RWKV-LM-V7 for AMD. |
| RWKV-infctx-trainer | [![Star](https://img.shields.io/github/stars/RWKV/RWKV-infctx-trainer.svg?style=social&label=Star)](https://github.com/RWKV/RWKV-infctx-trainer/) | | RWKV infinite context trainer, supporting training contexts of 10k and longer. |
| RWKV-Ouroboros | [![Star](https://img.shields.io/github/stars/neromous/RWKV-Ouroboros.svg?style=social&label=Star)](https://github.com/neromous/RWKV-Ouroboros) | | An API-based rwkv-trainer project that supports alternating between training and inference. |
| nanoRWKV | [![Star](https://img.shields.io/github/stars/Hannibal046/nanoRWKV.svg?style=social&label=Star)](https://github.com/Hannibal046/nanoRWKV) | | A nanoGPT-style implementation of the RWKV model. |
| RWKV_LM_EXT | [![Star](https://img.shields.io/github/stars/yynil/RWKV_LM_EXT.svg?style=social&label=Star)](https://github.com/yynil/RWKV_LM_EXT) | | Implements functional extensions for RWKV, including sequence classification/embedding/peft/cross-encoder/bi-encoder/multimodality, etc. |
| chunkRWKV6 | [![Star](https://img.shields.io/github/stars/00ffcc/chunkRWKV6.svg?style=social&label=Star)](https://github.com/00ffcc/chunkRWKV6) | | Optimizes RWKV prefill and training speed using chunk-wise parallelism. |

---

## Natural Language Processing / Large Language Models

### Model Architecture & Optimization

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|RWKVQuant|[![Star](https://img.shields.io/github/stars/xuchen-dev/RWKVQuant.svg?style=social&label=Star)](https://github.com/xuchen-dev/RWKVQuant)| [![arXiv:2505.03803](https://img.shields.io/badge/arXiv-2505.03803-b31b1b.svg)](https://arxiv.org/abs/2505.03803)| Efficient quantization for RWKV series models. |
|RWKV-X|[![Star](https://img.shields.io/github/stars/howard-hou/RWKV-X.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-X)|[![arXiv:2504.21463](https://img.shields.io/badge/arXiv-2504.21463-b31b1b.svg)](https://arxiv.org/abs/2504.21463)| A linear-complexity hybrid language model based on the RWKV architecture. |
|ARWKV|[![Star](https://img.shields.io/github/stars/yynil/RWKVInside.svg?style=social&label=Star)](https://github.com/yynil/RWKVInside)|[![arXiv:2501.15570](https://img.shields.io/badge/arXiv-2501.15570-b31b1b.svg)](https://arxiv.org/abs/2501.15570)| A language model with RWKV hybrid attention. |
|TemporalRNNs|[![Star](https://img.shields.io/github/stars/RazvanDu/TemporalRNNs.svg?style=social&label=Star)](https://github.com/RazvanDu/TemporalRNNs)|[![arXiv:2402.02625](https://img.shields.io/badge/arXiv-2402.02625-b31b1b.svg)](https://arxiv.org/abs/2402.02625)| [ICML 2024 workshop] A method for optimizing architecture from multiple temporal perspectives. |
|GoldFinch||[![arXiv:2407.12077](https://img.shields.io/badge/arXiv-2407.12077-b31b1b.svg)](https://arxiv.org/abs/2407.12077)| An RWKV/Transformer hybrid model. |
|RWKV-Lite||[![arXiv](https://img.shields.io/badge/arXiv-2412.10856-b31b1b)](https://arxiv.org/abs/2412.10856)| An efficient deep compression scheme for RWKV models. |
|RADLADS|[![Star](https://img.shields.io/github/stars/recursal/RADLADS-paper.svg?style=social&label=Star)](https://github.com/recursal/RADLADS-paper)|[![arXiv](https://img.shields.io/badge/arXiv-2505.03005-b31b1b)](https://arxiv.org/abs/2505.03005)| Efficiently converts Transformer architecture models to RWKV architecture models. |

### Natural Language Processing

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|L3TC|[![Star](https://img.shields.io/github/stars/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression.svg?style=social&label=Star)](https://github.com/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression)|[![arXiv:2412.16642](https://img.shields.io/badge/arXiv-2412.16642-b31b1b.svg)](https://arxiv.org/abs/2412.16642)| Efficient lossless text compression. |
|CMGN||[![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0925231225004837)| Fake news detection based on RWKV. |
|RCME||[![Paper](https://img.shields.io/badge/Paper-PDF-blue)](https://www.engineeringletters.com/issues_v33/issue_6/EL_33_6_28.pdf)| Knowledge graph completion with a hybrid architecture. |

### Multimodality

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|ModRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2505.14505-b31b1b)](https://arxiv.org/abs/2505.14505)| A multimodal fusion framework based on RWKV-7. |

---

## Image & Graphics

### Vision-Language

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| VisualRWKV | [![Star](https://img.shields.io/github/stars/howard-hou/VisualRWKV.svg?style=social&label=Star)](https://github.com/howard-hou/VisualRWKV) | [![arXiv:2406.13362](https://img.shields.io/badge/arXiv-2406.13362-b31b1b.svg)](https://arxiv.org/abs/2406.13362)| [COLING 2025] A vision-language model based on RWKV, capable of handling visual tasks. |
| RWKV-CLIP | [![Star](https://img.shields.io/github/stars/deepglint/RWKV-CLIP.svg?style=social&label=Star)](https://github.com/deepglint/RWKV-CLIP) | [![arXiv:2406.06973](https://img.shields.io/badge/arXiv-2406.06973-b31b1b.svg)](https://arxiv.org/abs/2406.06973) | [EMNLP 2024] An RWKV-powered CLIP (vision-language representation learning) model. |
|RWKV-UI||[![arXiv](https://img.shields.io/badge/arXiv-2502.03971-b31b1b)](https://arxiv.org/abs/2502.03971)| A vision-language model based on RWKV, focusing on UI understanding and design. |

### Vision Backbone

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Vision-RWKV (New Gen) | [![Star](https://img.shields.io/github/stars/xforcevesa/new-vrwkv.svg?style=social&label=Star)](https://github.com/xforcevesa/new-vrwkv) | | The new generation of RWKV for Vision, based on RWKV-7. |
| Vision-RWKV | [![Star](https://img.shields.io/github/stars/OpenGVLab/Vision-RWKV.svg?style=social&label=Star)](https://github.com/OpenGVLab/Vision-RWKV) | [![arXiv:2403.02308](https://img.shields.io/badge/arXiv-2403.02308-b31b1b.svg)](https://arxiv.org/abs/2403.02308)| [ICLR 2025 Spotlight] A vision perception model based on RWKV, capable of smoothly processing high-resolution images. |
| PointRWKV | [![Star](https://img.shields.io/github/stars/hithqd/PointRWKV.svg?style=social&label=Star)](https://github.com/hithqd/PointRWKV) |[![arXiv:2405.15214](https://img.shields.io/badge/arXiv-2405.15214-b31b1b.svg)](https://arxiv.org/abs/2405.15214) | [AAAI 2025] A 3D point cloud learning framework based on RWKV. |
|RSRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2503.20382-b31b1b)](https://arxiv.org/abs/2503.20382)| High-resolution remote sensing analysis, suitable for tasks like classification, object detection, and segmentation. |

### Image Classification

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|Vision_QRWKV|[![Star](https://img.shields.io/github/stars/ChiShengChen/Vision_QRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/Vision_QRWKV)|[![arXiv:2506.06633](https://img.shields.io/badge/arXiv-2506.06633-b31b1b.svg)](https://arxiv.org/abs/2506.06633)| A quantum-enhanced RWKV model for image classification. |

### Image Segmentation

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| U-RWKV | [![Star](https://img.shields.io/github/stars/hbyecoding/U-RWKV.svg?style=social&label=Star)](https://github.com/hbyecoding/U-RWKV) | | An image segmentation model based on RWKV. |
| RWKV-SAM | [![Star](https://img.shields.io/github/stars/HarborYuan/ovsam.svg?style=social&label=Star)](https://github.com/HarborYuan/ovsam) | [![arXiv:2406.19369](https://img.shields.io/badge/arXiv-2406.19369-b31b1b.svg)](https://arxiv.org/abs/2406.19369)| An open-vocabulary image segmentation method "RWKV-SAM" based on RWKV. |
|MMSegRWKV|[![Star](https://img.shields.io/github/stars/supercyt/MMSegRWKV.svg?style=social&label=Star)](https://github.com/supercyt/MMSegRWKV)|| A multimodal Magnetic Resonance Imaging (MRI) segmentation model developed based on the RWKV architecture. |
|BSBP-RWKV|| [![PDF](https://img.shields.io/badge/PDF-OpenReview-red)](https://openreview.net/pdf?id=ULD5RCk0oo)| RWKV for medical image segmentation. |
|RWKV-UNet||[![arXiv](https://img.shields.io/badge/arXiv-2501.08458-b31b1b)](https://arxiv.org/abs/2501.08458)| An improved U-Net with RWKV for medical image segmentation. |
|HFE-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888300)| [ICASSP 2025] RWKV for medical image segmentation by enhancing high-frequency components. |
|Zig-RiR||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Document-orange)](https://ieeexplore.ieee.org/document/10969076)| [IEEE TMI] Nested RWKV for medical image segmentation. |
|Diet-Seg||[![bioRxiv](https://img.shields.io/badge/bioRxiv-2025.05.31.657149-b31b1b.svg)](https://www.biorxiv.org/content/10.1101/2025.05.31.657149v1)| Medical image segmentation. |
|Med-URWKV||[![arXiv:2506.10858](https://img.shields.io/badge/arXiv-2506.10858-b31b1b.svg)](https://arxiv.org/abs/2506.10858)| A pure RWKV model for medical image segmentation, pre-trained on ImageNet. |

### Image Generation

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Diffusion-RWKV | [![Star](https://img.shields.io/github/stars/feizc/Diffusion-RWKV.svg?style=social&label=Star)](https://github.com/feizc/Diffusion-RWKV) |[![arXiv:2404.04478](https://img.shields.io/badge/arXiv-2404.04478-b31b1b.svg)](https://arxiv.org/abs/2404.04478) | An image generation model based on RWKV, adept at handling high-resolution images. |
|SDiT||[![arXiv:2402.11588](https://img.shields.io/badge/arXiv-2402.11588-b31b1b.svg)](https://arxiv.org/abs/2402.11588)| Image generation combining Spiking Neural Networks with RWKV. |

### Object Detection

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| LION | [![Star](https://img.shields.io/github/stars/happinesslz/LION.svg?style=social&label=Star)](https://github.com/happinesslz/LION) | [![arXiv:2407.18232](https://img.shields.io/badge/arXiv-2407.18232-b31b1b.svg)](https://arxiv.org/abs/2407.18232)| [NeurIPS 2024] Linear Group RNN (with RWKV support) for 3D object detection in point clouds. |
|RWKV-VG| [![Star](https://img.shields.io/github/stars/nianfd/RWKV-VG.svg?style=social&label=Star)](https://github.com/nianfd/RWKV-VG)|[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00530-025-01720-w)| A visual grounding framework based on the RWKV architecture. |
|Substation equipment||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11760-025-03852-y)| Substation defect detection. |

### Super-Resolution

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|OmniRWKVSR||[![arXiv](https://img.shields.io/badge/arXiv-2502.00404-b31b1b)](https://arxiv.org/abs/2502.00404)| [IJCNN] Single image super-resolution based on RWKV. |
|Geometry-Aware RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10943155)| Heterogeneous light field super-resolution. |
|Delta-WKV||[![arXiv](https://img.shields.io/badge/arXiv-2502.20852-b31b1b)](https://arxiv.org/abs/2502.20852)| [MICCAI 2025] A super-resolution model for Magnetic Resonance Imaging. |
|MSB-RWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s13042-025-02644-7)| Infrared image super-resolution. |

### Image Denoising / Enhancement

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|CRWKV|[![Star](https://img.shields.io/github/stars/Seeker98/CRWKV.svg?style=social&label=Star)](https://github.com/Seeker98/CRWKV)|[![arXiv:2505.02705](https://img.shields.io/badge/arXiv-2505.02705-b31b1b.svg)](https://arxiv.org/abs/2505.02705)| [IJCAI 2025] Efficient image denoising by introducing a bidirectional WKV mechanism. |
|RWKV-IR||[![arXiv:2412.03814](https://img.shields.io/badge/arXiv-2412.03814-b31b1b.svg)](https://arxiv.org/abs/2412.03814)| Image restoration based on RWKV. |
| Restore-RWKV | [![Star](https://img.shields.io/github/stars/Yaziwel/Restore-RWKV.svg?style=social&label=Star)](https://github.com/Yaziwel/Restore-RWKV) |[![arXiv:2407.11087](https://img.shields.io/badge/arXiv-2407.11087-b31b1b.svg)](https://arxiv.org/abs/2407.11087) | Efficient and effective medical image restoration using RWKV (PyTorch implementation). |
|SRCNet||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888780)| [ICASSP 2025] Underwater image enhancement based on RWKV. |
|ID-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10889384)| [ICASSP 2025] Efficient image deraining based on RWKV. |
|Flare-Aware RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888487)| [ICASSP 2025] Efficient image de-flaring based on RWKV. |
|URWKV||[![arXiv:2505.23068](https://img.shields.io/badge/arXiv-2505.23068-b31b1b.svg)](https://arxiv.org/abs/2505.23068)| [CVPR 2025] Low-light image restoration. |
|Pan-Sharpening||[![IEEE](https://img.shields.io/badge/IEEE-11023855-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11023855)| [IEEE TGRS] Pansharpening based on RWKV. |
|DiffRWKVIR||[![arXiv:2506.14541](https://img.shields.io/badge/arXiv-2506.14541-b31b1b.svg)](https://arxiv.org/abs/2506.14541)| Image restoration combining RWKV and diffusion models. |

### Other Image Tasks

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|LALIC|[![Star](https://img.shields.io/github/stars/sjtu-medialab/RwkvCompress.svg?style=social&label=Star)](https://github.com/sjtu-medialab/RwkvCompress)|[![arXiv:2502.05741](https://img.shields.io/badge/arXiv-2502.05741-b31b1b.svg)](https://arxiv.org/abs/2502.05741)| [CVPR 2025] An image compression framework based on RWKV. |
| LineRWKV | [![Star](https://img.shields.io/github/stars/diegovalsesia/linerwkv.svg?style=social&label=Star)](https://github.com/diegovalsesia/linerwkv) | [![arXiv:2403.17677](https://img.shields.io/badge/arXiv-2403.17677-b31b1b.svg)](https://arxiv.org/abs/2403.17677)| LineRWKV is a method for lossless and lossy compression of hyperspectral images. |
|OpenPAR|[![Star](https://img.shields.io/github/stars/Event-AHU/OpenPAR.svg?style=social&label=Star)](https://github.com/Event-AHU/OpenPAR)| [![arXiv:2504.10018](https://img.shields.io/badge/arXiv-2504.10018-b31b1b.svg)](https://arxiv.org/abs/2504.10018)| An open-source pedestrian attribute recognition framework, including RWKV. |
|PathRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2503.03199-b31b1b)](https://arxiv.org/abs/2503.03199)| Whole-slide image analysis. |
|RWKVMatch||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888484)| [ICASSP 2025] Medical image registration with a global and cross-fusion mechanism based on vision-RWKV. |
|EVA||[![arXiv:2505.11165](https://img.shields.io/badge/arXiv-2505.11165-b31b1b.svg)](https://arxiv.org/abs/2505.11165)| Asynchronous detection for event cameras using an asynchronous encoder built with RWKV-6. |
|RWKV-DPA||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Document-orange)](https://ieeexplore.ieee.org/document/10779439)| Efficient depth estimation based on RWKV. |

---

## 3D & Video Processing

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| FEAT | [![Star](https://img.shields.io/github/stars/Yaziwel/FEAT.svg?style=social&label=Star)](https://github.com/Yaziwel/FEAT) |[![arXiv:2506.04956](https://img.shields.io/badge/arXiv-2506.04956-b31b1b.svg)](https://arxiv.org/abs/2506.04956) | [MICCAI 2025 early accepted] Medical video generation based on RWKV. |
|TLS-RWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11063-024-11540-0)| Online Action Detection (OAD) based on RWKV. |
|Video RWKV||[![arXiv:2411.05636](https://img.shields.io/badge/arXiv-2411.05636-b31b1b.svg)](https://arxiv.org/abs/2411.05636)| Video action recognition based on RWKV. |
|TCVADS||[![arXiv:2412.20201](https://img.shields.io/badge/arXiv-2412.20201-b31b1b.svg)](https://arxiv.org/abs/2412.20201)| Video anomaly detection based on RWKV. |
|StyleRWKV||[![arXiv:2412.19535](https://img.shields.io/badge/arXiv-2412.19535-b31b1b.svg)](https://arxiv.org/abs/2412.19535)| Efficient video style transfer based on an RWKV-like architecture. |
|RainRWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00371-025-03965-y)| Efficient video deraining based on RWKV. |

---

## Audio Related

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|MIDI-RWKV|[![Star](https://img.shields.io/github/stars/christianazinn/MIDI-RWKV.svg?style=social&label=Star)](https://github.com/christianazinn/MIDI-RWKV)|[![arXiv:2506.13001](https://img.shields.io/badge/arXiv-2506.13001-b31b1b.svg)](https://arxiv.org/abs/2506.13001)| Music generation based on RWKV. |
| RWKV-TTS | [![Star](https://img.shields.io/github/stars/yynil/RWKVTTS.svg?style=social&label=Star)](https://github.com/yynil/RWKVTTS) | [![arXiv:2504.03289](https://img.shields.io/badge/arXiv-2504.03289-b31b1b.svg)](https://arxiv.org/abs/2504.03289) | An RWKV speech synthesis model, supporting text-to-speech in multiple languages. |
| RWKV-ASR | [![Star](https://img.shields.io/github/stars/AGENDD/RWKV-ASR.svg?style=social&label=Star)](https://github.com/AGENDD/RWKV-ASR) | | **Speech recognition** using a pre-trained RWKV language model. |
|Rate-Aware||[![arXiv](https://img.shields.io/badge/arXiv-2501.11999-b31b1b)](https://arxiv.org/abs/2501.11999)| A speech compression scheme based on RWKV. |

---

## Time Series

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| BlackGoose_Rimer | [![Star](https://img.shields.io/github/stars/Alic-Li/BlackGoose_Rimer.svg?style=social&label=Star)](https://github.com/Alic-Li/BlackGoose_Rimer) |[![arXiv:2503.06121](https://img.shields.io/badge/arXiv-2503.06121-b31b1b.svg)](https://arxiv.org/abs/2503.06121) | A time series forecasting model based on RWKV-7, supporting various time series tasks. |
| RWKV-TS | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-TS.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-TS) | | A time series task model based on RWKV, with low latency and memory usage. |
|MSRWKV-2DTCN ||[![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0360544224028433)| Short-term photovoltaic power forecasting with multi-scale RWKV. |
|AutoGMM-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10729884)| A selective forwarding attack detection scheme for wireless sensor networks based on RWKV. |
|DFT||[![arXiv:2411.06065](https://img.shields.io/badge/arXiv-2411.06065-b31b1b.svg)](https://arxiv.org/abs/2411.06065)| Stock price prediction based on RWKV. |
|MATCC||[![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3627673.3679715)| Stock price prediction based on RWKV. |
|ET_MGNN||[![Paper](https://img.shields.io/badge/Paper-SSRN-orange)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5114041)| A brain science diagnostic model using RWKV for temporal modeling. |
|TabulaTime||[![arXiv](https://img.shields.io/badge/arXiv-2502.17049-b31b1b)](https://arxiv.org/abs/2502.17049)| A time series model for ACS prediction. |
|LASTGCN||[![Scientific Reports](https://img.shields.io/badge/Scientific%20Reports-2025-green)](https://www.nature.com/articles/s41598-025-93179-y)| Spatio-temporal multi-graph traffic flow prediction based on RWKV. |
|DREMnet||[![arXiv](https://img.shields.io/badge/arXiv-2503.22223-b31b1b)](https://arxiv.org/abs/2503.22223)| Denoising of electromagnetic signals. |
|RWKV-TDR7||[![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.22544)| Motion trajectory planning for inverse kinematics. |
|MolRWKV||[![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.70100)| Conditional molecular generation in biology. |
|QuantumRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2505.13524-b31b1b)](https://arxiv.org/abs/2505.13524)| Quantum-enhanced time series forecasting based on RWKV. |
|STWGRL||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-11002535-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11002535)| [IEEE IoT-J] Time series anomaly detection using RWKV as a core module. |

---

## Robotics & Embodied AI

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| DecisionRWKV | [![Star](https://img.shields.io/github/stars/ancorasir/DecisionRWKV.svg?style=social&label=Star)](https://github.com/ancorasir/DecisionRWKV) | [![arXiv:2407.16306](https://img.shields.io/badge/arXiv-2407.16306-b31b1b.svg)](https://arxiv.org/abs/2407.16306)| [JCISE] A lifelong learning algorithm for robots using experience replay + Decision-RWKV model. |
| OccRWKV | [![Star](https://img.shields.io/github/stars/jmwang0117/OccRWKV.svg?style=social&label=Star)](https://github.com/jmwang0117/OccRWKV) | [![arXiv:2409.19987](https://img.shields.io/badge/arXiv-2409.19987-b31b1b.svg)](https://arxiv.org/abs/2409.19987)| [ICRA 2025] Efficient 3D semantic occupancy prediction with linear complexity. |

---

## RWKV Tokenizers

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| rwkv-tokenizer | [![Star](https://img.shields.io/github/stars/cahya-wirawan/rwkv-tokenizer.svg?style=social&label=Star)](https://github.com/cahya-wirawan/rwkv-tokenizer) | | A fast RWKV Tokenizer written in Rust, supporting RWKV-V5/6 World models. |
| rwkv_tokenizer.c | [![Star](https://img.shields.io/github/stars/mrsteyk/rwkv_tokenizer.c.svg?style=social&label=Star)](https://github.com/mrsteyk/rwkv_tokenizer.c) | | An RWKV Trie tokenizer written in C. |
| rwkv-tokenizer-go | [![Star](https://img.shields.io/github/stars/Ronsor/rwkv-tokenizer-go.svg?style=social&label=Star)](https://github.com/Ronsor/rwkv-tokenizer-go) | | An RWKV tokenizer for the Go language. |
| RWKV-World-Tokenizer-CPP | [![Star](https://img.shields.io/github/stars/m8than/RWKV-World-Tokenizer-CPP.svg?style=social&label=Star)](https://github.com/m8than/RWKV-World-Tokenizer-CPP) | | A highly optimized trie tokenizer for RWKV World models, written in C++. |

---

## RAG Systems for RWKV

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-RAG | [![Star](https://img.shields.io/github/stars/AIIRWKV/RWKV-RAG.svg?style=social&label=Star)](https://github.com/AIIRWKV/RWKV-RAG) | | A one-click RAG deployment system based on RWKV models, allowing easy setup and management of local knowledge bases, along with a Q&A bot and one-click fine-tuning for RWKV. |

---

## Chatbots & Inference API Servers

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| **⭐ (Recommended)** RWKV Runner | [![Star](https://img.shields.io/github/stars/josStorer/RWKV-Runner.svg?style=social&label=Star)](https://github.com/josStorer/RWKV-Runner) | | RWKV Runner is a management and launcher tool for RWKV models, with a user-friendly GUI, supporting both training and inference. |
| **⭐ (Recommended)** AI00 RWKV Server | [![Star](https://img.shields.io/github/stars/cgisky1980/ai00_rwkv_server.svg?style=social&label=Star)](https://github.com/cgisky1980/ai00_rwkv_server) | | Ai00 Server is an **inference API server** for RWKV models, based on the web-rwkv inference engine. |
|RWKV_APP|[![Star](https://img.shields.io/github/stars/RWKV-APP/RWKV_APP.svg?style=social&label=Star)](https://github.com/RWKV-APP/RWKV_APP)|| An on-device inference App for RWKV-LM implemented with Flutter. |
| **🇨🇳 (Chinese)** Wenda Web UI | [![Star](https://img.shields.io/github/stars/wenda-LLM/wenda.svg?style=social&label=Star)](https://github.com/wenda-LLM/wenda) | | An LLM calling platform for content generation in specific contexts, with support for RWKV models. |
| **🇨🇳 (Chinese)** Role Play Chatbot | [![Star](https://img.shields.io/github/stars/shengxia/RWKV_Role_Playing.svg?style=social&label=Star)](https://github.com/shengxia/RWKV_Role_Playing) | | A role-playing WebUI based on RWKV, built with Gradio. |
| Easy_RWKV_webui | [![Star](https://img.shields.io/github/stars/No-22-Github/Easy_RWKV_webui.svg?style=social&label=Star)](https://github.com/No-22-Github/Easy_RWKV_webui) | | An online chat room for RWKV models based on PyWebIO. |
| Mini Model Daemon | [![Star](https://img.shields.io/github/stars/recursal/minmodmon.svg?style=social&label=Star)](https://github.com/recursal/minmodmon) | | An inference tool for RWKV models based on the web-rwkv inference backend. |
| LocalAI | [![Star](https://img.shields.io/github/stars/go-skynet/LocalAI.svg?style=social&label=Star)](https://github.com/go-skynet/LocalAI) | | An open-source OpenAI alternative that supports RWKV. |
| GPT Academic | [![Star](https://img.shields.io/github/stars/binary-husky/gpt_academic.svg?style=social&label=Star)](https://github.com/binary-husky/gpt_academic) | | Provides a practical interactive interface for LLMs like GPT/GLM, with support for RWKV. |
| LLMFarm | [![Star](https://img.shields.io/github/stars/guinmoon/LLMFarm.svg?style=social&label=Star)](https://github.com/guinmoon/LLMFarm) | | Use large language models offline on iOS and MacOS with the GGML library, with support for RWKV. |

---

## RWKV Benchmarks

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Uncheatable Eval | [![Star](https://img.shields.io/github/stars/Jellyfish042/uncheatable_eval.svg?style=social&label=Star)](https://github.com/Jellyfish042/uncheatable_eval) | | Tests LLM performance using the latest dynamic data, including RWKV. |
| RULER_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/RULER_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/RULER_RWKV) | | [RULER](https://arxiv.org/abs/2404.06654) test scores for RWKV models. |
| LongBench_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/LongBench_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/LongBench_RWKV) | | [LongBench](https://arxiv.org/abs/2308.14508) test scores for RWKV. |
| rwkv_mmlu | [![Star](https://img.shields.io/github/stars/Jellyfish042/rwkv_mmlu.svg?style=social&label=Star)](https://github.com/Jellyfish042/rwkv_mmlu) | | MMLU test scores for RWKV models. |

---

## Inference Frameworks & Operator Libraries

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|rwkv_Ascend|[![Star](https://img.shields.io/github/stars/appleinsky/rwkv_Ascend.svg?style=social&label=Star)](https://github.com/appleinsky/rwkv_Ascend)|| An operator repository co-developed by Ascend and RWKV. |
| rwkv7.c | [![Star](https://img.shields.io/github/stars/KevlarKanou/rwkv7.c.svg?style=social&label=Star)](https://github.com/KevlarKanou/rwkv7.c) | | A C implementation for RWKV-7, supporting inference for RWKV-7 models. |
| rwkv.cpp | [![Star](https://img.shields.io/github/stars/RWKV/rwkv.cpp.svg?style=social&label=Star)](https://github.com/RWKV/rwkv.cpp) | | Infers RWKV models on the CPU, supporting FP16, and quantized INT4, INT5, and INT8 inference. |
| RWKVSharp | [![Star](https://img.shields.io/github/stars/imxcstar/RWKVSharp.svg?style=social&label=Star)](https://github.com/imxcstar/RWKVSharp) | | An RWKV inference tool wrapped in C#, based on rwkv.cpp, supporting RWKV4/RWKV5/RWKV6/RWKV7 World models. |
| RWKV_Pytorch | [![Star](https://img.shields.io/github/stars/yuunnn-w/RWKV_Pytorch.svg?style=social&label=Star)](https://github.com/yuunnn-w/RWKV_Pytorch) | | An RWKV model inference framework implemented purely in native PyTorch. |
| rwkv-kit | [![Star](https://img.shields.io/github/stars/TorchRWKV/rwkv-kit.svg?style=social&label=Star)](https://github.com/TorchRWKV/rwkv-kit) | | An RWKV model inference framework supporting batch inference, parallel inference training, and other features. |
| web-rwkv | [![Star](https://img.shields.io/github/stars/cryscan/web-rwkv.svg?style=social&label=Star)](https://github.com/cryscan/web-rwkv) | | Implements RWKV model inference in pure WebGPU/Rust. |
| candle-rwkv | [![Star](https://img.shields.io/github/stars/nkypy/candle-rwkv.svg?style=social&label=Star)](https://github.com/nkypy/candle-rwkv) | | Implements RWKV model inference (with quantization support) in candle, a minimalist ML framework for Rust. |
| **🚧 (In Development)** RWKV7-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV7-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV7-Keras) | | A Keras implementation of the RWKV model, supporting training and inference. |
| RWKV6-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV6-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV6-Keras) | | A Keras implementation of the RWKV model, supporting training and inference. |
| rwkv-burn| [![Star](https://img.shields.io/github/stars/dymat/rwkv-burn.svg?style=social&label=Star)](https://github.com/dymat/rwkv-burn) | | A burn implementation of the RWKV language model. |
| jaxrwkv | [![Star](https://img.shields.io/github/stars/bsarkar321/jaxrwkv.svg?style=social&label=Star)](https://github.com/bsarkar321/jaxrwkv) | | A JAX implementation of the RWKV language model. |
| rwkv-mobile | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-mobile.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-mobile) | | An RWKV mobile inference engine. |
| rwkv-qualcomm | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-qualcomm.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-qualcomm) | | Infers RWKV models using the Qualcomm AI Engine Direct SDK. |
| rwkv-by-hand-excel | [![Star](https://img.shields.io/github/stars/playaswd/rwkv-by-hand-excel.svg?style=social&label=Star)](https://github.com/playaswd/rwkv-by-hand-excel) | | Implements RWKV in Excel to help developers explore its principles. |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) | | Infers RWKV-V6/V7 using FLA, supporting inference with combined multiple states. |
| MLC LLM | [![Star](https://img.shields.io/github/stars/mlc-ai/mlc-llm.svg?style=social&label=Star)](https://github.com/mlc-ai/mlc-llm) | | A machine learning compiler and high-performance deployment engine that supports RWKV models. |

---

## Other RWKV Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
|SocialDeductionLLM|[![Star](https://img.shields.io/github/stars/SocialDeductionLLM/SocialDeductionLLM.svg?style=social&label=Star)](https://github.com/SocialDeductionLLM/SocialDeductionLLM)|[![arXiv:2502.06060](https://img.shields.io/badge/arXiv-2502.06060-b31b1b.svg)](https://arxiv.org/abs/2502.06060)| [AAMAS 2025] Multi-agent reinforcement learning. |
|ARIES|[![Star](https://img.shields.io/github/stars/Chieko-Seren/ARIES.svg?style=social&label=Star)](https://github.com/Chieko-Seren/ARIES)|| An automated operations system with RWKV support. |
| SpikeGPT | [![Star](https://img.shields.io/github/stars/ridgerchu/SpikeGPT.svg?style=social&label=Star)](https://github.com/ridgerchu/SpikeGPT) | | A new model inspired by RWKV. |
| JSONL to binidx | [![Star](https://img.shields.io/github/stars/Abel2076/json2binidx_tool.svg?style=social&label=Star)](https://github.com/Abel2076/json2binidx_tool) | | A tool to convert `.jsonl` files to the `.bin /.idx` (binidx) format suitable for RWKV training. |
| AI Town - RWKV Proxy | [![Star](https://img.shields.io/github/stars/recursal/ai-town-rwkv-proxy.svg?style=social&label=Star)](https://github.com/recursal/ai-town-rwkv-proxy?tab=readme-ov-file) | | Run a large-scale AI town locally with RWKV! |
| Bot-Ani-RWKV | [![Star](https://img.shields.io/github/stars/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection.svg?style=social&label=Star)](https://github.com/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection) | | A Twitter bot detection tool based on RWKV. |
| RWKV-IF | [![Star](https://img.shields.io/github/stars/Lyttr/RWKVInverseFolding.svg?style=social&label=Star)](https://github.com/Lyttr/RWKVInverseFolding) | [![bioRxiv](https://img.shields.io/badge/bioRxiv-green)](https://www.biorxiv.org/content/10.1101/2025.06.13.659654v1.full.pdf)| An efficient and controllable RNA inverse folding design framework based on RWKV. |
| poker-ai-rwkv | [![Star](https://img.shields.io/github/stars/meraline/poker-ai-rwkv.svg?style=social&label=Star)](https://github.com/meraline/poker-ai-rwkv) | | An AI poker game system with RWKV. |
|Muon-RMS-Norm|[![Star](https://img.shields.io/github/stars/xTimeCrystal/Muon-RMS-Norm.svg?style=social&label=Star)](https://github.com/xTimeCrystal/Muon-RMS-Norm)|| A novel normalization method. |
|PCF-RWKV||[![Paper](https://img.shields.io/badge/Paper-Preprint-yellow)](https://www.preprints.org/manuscript/202412.1705/v1)| A product carbon footprint estimation system based on the RWKV model. |
|ChemRB||[![Paper](https://img.shields.io/badge/Paper-SNNU-orange)](https://jsnu.magtech.com.cn/CN/10.15983/j.cnki.jsnu.2025005)| Medical molecular generation. |
|DualComp||[![arXiv:2505.16256](https://img.shields.io/badge/arXiv-2505.16256-b31b1b.svg)](https://arxiv.org/abs/2505.16256)| Lossless data compression based on RWKV-7. |
