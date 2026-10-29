---

[Chinese Version](README.md)

---

# RWKV Ecosystem Projects

A curated list of outstanding projects, tools, and resources in the RWKV ecosystem.

## Table of Contents

- [Official RWKV Links](#official-rwkv-links)
- [RWKV Fine-Tuning and Training](#rwkv-fine-tuning-and-training)
  - [Fine-Tuning Projects](#fine-tuning-projects)
  - [Training Projects](#training-projects)
- [Model Architecture and Optimization](#model-architecture-and-optimization)
- [Natural Language Processing](#natural-language-processing)
- [Multimodal Fusion](#multimodal-fusion)
- [Images and Graphics](#images-and-graphics)
  - [Vision-Language Models](#vision-language-models)
  - [Vision Backbones](#vision-backbones)
  - [Image Classification](#image-classification)
  - [Image Segmentation](#image-segmentation)
  - [Image Generation](#image-generation)
  - [Object Detection](#object-detection)
  - [Super-Resolution](#super-resolution)
  - [Image Denoising and Enhancement](#image-denoising-and-enhancement)
  - [Other Image Tasks](#other-image-tasks)
- [3D and Video Processing](#3d-and-video-processing)
- [Audio](#audio)
- [Time Series](#time-series)
- [Robotics and Embodied Intelligence](#robotics-and-embodied-intelligence)
- [RWKV Tokenizers](#rwkv-tokenizers)
- [RAG Systems for RWKV](#rag-systems-for-rwkv)
- [Chatbots and Inference API Servers](#chatbots-and-inference-api-servers)
- [RWKV Benchmarks](#rwkv-benchmarks)
- [RWKV Inference Frameworks and Kernel Libraries](#rwkv-inference-frameworks-and-kernel-libraries)
- [Other RWKV Projects](#other-rwkv-projects)

---

## Official RWKV Links

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-LM | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM) |  | The official RWKV code repository, with architecture implementations from RWKV v1 through v7 and accompanying large language model training code. |
| RWKV-4 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v4) | [![arXiv:2305.13048](https://img.shields.io/badge/arXiv-2305.13048-b31b1b.svg)](https://arxiv.org/abs/2305.13048) | The RWKV-4 architecture paper. |
| RWKV 5/6 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v5) | [![arXiv:2404.05892](https://img.shields.io/badge/arXiv-2404.05892-b31b1b.svg)](https://arxiv.org/abs/2404.05892) | The RWKV-5/6 architecture paper. |
| RWKV-7 Architecture Paper | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v7) | [![arXiv:2503.14456](https://img.shields.io/badge/arXiv-2503.14456-b31b1b.svg)](https://arxiv.org/abs/2503.14456) | The RWKV-7 architecture paper. |
| RWKV pip Package | [![PyPI](https://img.shields.io/pypi/v/rwkv.svg)](https://pypi.org/project/rwkv/) |  | The RWKV pip package. See the [RWKV website](https://rwkv.cn/tutorials/intermediate/RWKVpip) for usage instructions. |
| RWKV-CUDA | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-CUDA.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-CUDA) |  | Official CUDA kernels for RWKV. |
| Hugging Face Documentation | [![🤗 RWKV](https://img.shields.io/badge/🤗%20RWKV-blue)](https://huggingface.co/docs/transformers/model_doc/rwkv) |  | Hugging Face documentation for RWKV. |
| rwkvcn-docs | [![Star](https://img.shields.io/github/stars/LeoLin4258/rwkvcn-docs.svg?style=social&label=Star)](https://github.com/LeoLin4258/rwkvcn-docs) |  | The Chinese documentation project for RWKV. |
| RWKV.com | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV.com.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV.com) |  | The project repository for the English RWKV website. |

---

## RWKV Fine-Tuning and Training

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-Development-Tools | [![Star](https://img.shields.io/github/stars/Ourboros-Alignment-Team/RWKV-Development-Tools.svg?style=social&label=Star)](https://github.com/Ourboros-Alignment-Team/RWKV-Development-Tools) |  | A research platform for RWKV models with a comprehensive, integrated toolkit. |

### Fine-Tuning Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| **⭐ (Recommended)** RWKV-PEFT | [![Star](https://img.shields.io/github/stars/Joluck/RWKV-PEFT.svg?style=social&label=Star)](https://github.com/Joluck/RWKV-PEFT) |  | A repository for parameter-efficient RWKV fine-tuning, supporting LoRA, Pissa, DiSHA, State tuning, and other methods. |
| RWKV-PEFT-Simple | [![Star](https://img.shields.io/github/stars/Seikaijyu/RWKV-PEFT-Simple.svg?style=social&label=Star)](https://github.com/Seikaijyu/RWKV-PEFT-Simple) |  | A simplified version of RWKV-PEFT with convenient scripts and fine-tuning instructions. |
| RWKV-LM-RLHF | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-LM-RLHF.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-LM-RLHF) |  | A reinforcement learning from human feedback (RLHF) toolkit for RWKV, including supervised fine-tuning (SFT) and alignment methods such as DPO and ORPO. |
| stateswap | [![Star](https://img.shields.io/github/stars/Nice0o0/stateswap.svg?style=social&label=Star)](https://github.com/Nice0o0/stateswap) |  | Freezes RWKV-7 model weights and trains only the initial recurrent state to preserve personas or task modes; provides state hot-swapping, blending, compression, and a chat interface. |
| Preen | [![Star](https://img.shields.io/github/stars/No-22-Github/Preen.svg?style=social&label=Star)](https://github.com/No-22-Github/Preen) |  | An RWKV-7 state fine-tuning tool for Apple Silicon Macs, with a SwiftUI graphical interface and a command-line entry point; imports JSONL data and exports loadable initial-state files. |
| rwkvtune | [![Star](https://img.shields.io/github/stars/aierwiki/rwkvtune.svg?style=social&label=Star)](https://github.com/aierwiki/rwkvtune) |  | An RWKV training toolkit with Config, Trainer, and Dataset workflows similar to Hugging Face TRL, covering supervised fine-tuning and preference optimization. |

### Training Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| wind_rwkv | [![Star](https://img.shields.io/github/stars/johanwind/wind_rwkv.svg?style=social&label=Star)](https://github.com/johanwind/wind_rwkv) |  | A repository of optimized kernels for RWKV language models, currently focused on RWKV-7. |
| RWKV-LM-V7 | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/RWKV-LM-V7.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/RWKV-LM-V7) |  | An easy-to-use training project for multiple types of RWKV-7 models, designed to help developers get started with RWKV-7 training in 15 minutes. |
| RWKV-LM-V7-AMD-ROCm | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV-LM-V7-AMD-ROCm.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV-LM-V7-AMD-ROCm) |  | An AMD-compatible version of RWKV-LM-V7. |
| RWKV-infctx-trainer | [![Star](https://img.shields.io/github/stars/RWKV/RWKV-infctx-trainer.svg?style=social&label=Star)](https://github.com/RWKV/RWKV-infctx-trainer/) |  | An infinite-context RWKV trainer supporting context lengths of 10k tokens and beyond. |
| RWKV-Ouroboros | [![Star](https://img.shields.io/github/stars/neromous/RWKV-Ouroboros.svg?style=social&label=Star)](https://github.com/neromous/RWKV-Ouroboros) |  | An API-based rwkv-trainer project that supports alternating between training and inference. |
| nanoRWKV | [![Star](https://img.shields.io/github/stars/Hannibal046/nanoRWKV.svg?style=social&label=Star)](https://github.com/Hannibal046/nanoRWKV) |  | A nanoGPT-style implementation of RWKV. |
| RWKV_LM_EXT | [![Star](https://img.shields.io/github/stars/yynil/RWKV_LM_EXT.svg?style=social&label=Star)](https://github.com/yynil/RWKV_LM_EXT) |  | RWKV extensions for sequence classification, embeddings, parameter-efficient fine-tuning (PEFT), cross-encoders, bi-encoders, multimodal tasks, and more. |
| chunkRWKV6 | [![Star](https://img.shields.io/github/stars/00ffcc/chunkRWKV6.svg?style=social&label=Star)](https://github.com/00ffcc/chunkRWKV6) |  | Uses chunkwise parallelism to accelerate RWKV prefill and training. |
| Mini_RWKV_7 | [![Star](https://img.shields.io/github/stars/Alic-Li/Mini_RWKV_7.svg?style=social&label=Star)](https://github.com/Alic-Li/Mini_RWKV_7) |  | A complete, lightweight workflow for training RWKV-7 language models. |
| RWKV-Megatron | [![Star](https://img.shields.io/github/stars/TimeMobius/RWKV-Megatron.svg?style=social&label=Star)](https://github.com/TimeMobius/RWKV-Megatron) |  | A distributed RWKV-6/RWKV-7 training framework based on NVIDIA Megatron-Core, integrating tensor, pipeline, sequence, and data parallelism, with mixed-precision training and checkpoint conversion. |
| rwkv-metal | [![Star](https://img.shields.io/github/stars/RafaelUI/rwkv-metal.svg?style=social&label=Star)](https://github.com/RafaelUI/rwkv-metal) |  | An Apple Silicon training framework built on MLX and custom Metal WKV-7 kernels, supporting RWKV-7 pretraining, LoRA/QLoRA fine-tuning, state fine-tuning, and inference. |
| transformers-rwkv7 | [![Star](https://img.shields.io/github/stars/dfytensor/transformers-rwkv7.svg?style=social&label=Star)](https://github.com/dfytensor/transformers-rwkv7) |  | A self-contained, Hugging Face-compatible implementation of RWKV-7 Goose in pure PyTorch, integrating with Trainer, PEFT, and related training tools, with a recurrent-state inference path. |

---

## Model Architecture and Optimization

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKVQuant | [![Star](https://img.shields.io/github/stars/xuchen-dev/RWKVQuant.svg?style=social&label=Star)](https://github.com/xuchen-dev/RWKVQuant) | [![arXiv:2505.03803](https://img.shields.io/badge/arXiv-2505.03803-b31b1b.svg)](https://arxiv.org/abs/2505.03803) | Efficient quantization for RWKV models. |
| RWKV-X | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-X.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-X) | [![arXiv:2504.21463](https://img.shields.io/badge/arXiv-2504.21463-b31b1b.svg)](https://arxiv.org/abs/2504.21463) | A hybrid language model based on RWKV with linear computational complexity. |
| ARWKV | [![Star](https://img.shields.io/github/stars/yynil/RWKVInside.svg?style=social&label=Star)](https://github.com/yynil/RWKVInside) | [![arXiv:2501.15570](https://img.shields.io/badge/arXiv-2501.15570-b31b1b.svg)](https://arxiv.org/abs/2501.15570) | A language model using RWKV hybrid attention. |
| TemporalRNNs | [![Star](https://img.shields.io/github/stars/RazvanDu/TemporalRNNs.svg?style=social&label=Star)](https://github.com/RazvanDu/TemporalRNNs) | [![arXiv:2402.02625](https://img.shields.io/badge/arXiv-2402.02625-b31b1b.svg)](https://arxiv.org/abs/2402.02625) | (ICML 2024 Workshop) Architecture optimization using multiple temporal perspectives. |
| GoldFinch | [![Star](https://img.shields.io/github/stars/recursal/GoldFinch-paper.svg?style=social&label=Star)](https://github.com/recursal/GoldFinch-paper) | [![arXiv:2407.12077](https://img.shields.io/badge/arXiv-2407.12077-b31b1b.svg)](https://arxiv.org/abs/2407.12077) | A hybrid RWKV/Transformer model. |
| RWKV-edge |  | [![arXiv](https://img.shields.io/badge/arXiv-2412.10856-b31b1b)](https://arxiv.org/abs/2412.10856) | An efficient deep-compression approach for RWKV models. |
| RADLADS | [![Star](https://img.shields.io/github/stars/recursal/RADLADS-paper.svg?style=social&label=Star)](https://github.com/recursal/RADLADS-paper) | [![arXiv](https://img.shields.io/badge/arXiv-2505.03005-b31b1b)](https://arxiv.org/abs/2505.03005) | Efficient conversion of Transformer models into RWKV models. |
| RWKV-Depth-recurrence | [![Star](https://img.shields.io/github/stars/EricZhang1412/RWKV-Depth-recurrence.svg?style=social&label=Star)](https://github.com/EricZhang1412/RWKV-Depth-recurrence) |  | An RWKV implementation with depth recurrence through cross-layer parameter sharing. |
| ROSA-Soft | [![Star](https://img.shields.io/github/stars/wjie98/rosa_soft.svg?style=social&label=Star)](https://github.com/wjie98/rosa_soft) |  | A PyTorch extension for the ROSA suffix-retrieval operator, providing exact matching on CUDA, surrogate gradients for training, and stateful CPU inference based on a C++ suffix automaton. |
| ROSA-Tuning | [![Star](https://img.shields.io/github/stars/zyaaa-ux/ROSA-Tuning.svg?style=social&label=Star)](https://github.com/zyaaa-ux/ROSA-Tuning) | [![arXiv:2602.02499](https://img.shields.io/badge/arXiv-2602.02499-b31b1b.svg)](https://arxiv.org/abs/2602.02499) | Combines ROSA suffix-matching memory with a window-attention language model for long-context modeling; provides training code and Qwen3-based experiment configurations. |
| B3D-RWKV | [![Star](https://img.shields.io/github/stars/leonardodalinky/B3D-RWKV.svg?style=social&label=Star)](https://github.com/leonardodalinky/B3D-RWKV) | [![arXiv:2605.25969](https://img.shields.io/badge/arXiv-2605.25969-b31b1b.svg)](https://arxiv.org/abs/2605.25969) | A ternary block discrete diffusion language model based on RWKV-7, trained with combinations of masked and clean blocks for text infilling; provides training, inference, and evaluation code. |

## Natural Language Processing

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| L3TC | [![Star](https://img.shields.io/github/stars/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression.svg?style=social&label=Star)](https://github.com/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression) | [![arXiv:2412.16642](https://img.shields.io/badge/arXiv-2412.16642-b31b1b.svg)](https://arxiv.org/abs/2412.16642) | Efficient lossless text compression. |
| CMGN |  | [![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0925231225004837) | RWKV-based fake news detection. |
| RCME |  | [![Paper](https://img.shields.io/badge/Paper-PDF-blue)](https://www.engineeringletters.com/issues_v33/issue_6/EL_33_6_28.pdf) | Knowledge graph completion with a hybrid architecture. |
| TongShunLM | [![Star](https://img.shields.io/github/stars/ovo-Tim/TongShunLM.svg?style=social&label=Star)](https://github.com/ovo-Tim/TongShunLM) |  | A lightweight RWKV-7 model for scoring wording fluency. |
| rwkv-jev | [![Star](https://img.shields.io/github/stars/XingQiPan/rwkv-jev.svg?style=social&label=Star)](https://github.com/XingQiPan/rwkv-jev) |  | A structured decision service based on RWKV-7 that outputs probability distributions over a fixed set of candidate labels; compatible with TypeSafe's `/v1/systemone` interface for classification and constrained decision-making. |
| RWKV_document-term-translator | [![Star](https://img.shields.io/github/stars/LuckySongXiao/RWKV_document-term-translator.svg?style=social&label=Star)](https://github.com/LuckySongXiao/RWKV_document-term-translator) |  | A Windows document terminology translation assistant built with C# and WPF, supporting Word and Excel documents and terminology database management, with rwkv_lightning or llama.cpp inference backends. |
| rwkv-code-completion | [![Star](https://img.shields.io/github/stars/xun082/rwkv-code-completion.svg?style=social&label=Star)](https://github.com/xun082/rwkv-code-completion) |  | An RWKV-based VS Code code completion extension with real-time suggestions, multiple candidates, and fill-in-the-middle (FIM) completion; requires a self-hosted RWKV inference backend. |

## Multimodal Fusion

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| ModRWKV | [![Star](https://img.shields.io/github/stars/Joluck/mod-rwkv.svg?style=social&label=Star)](https://github.com/Joluck/mod-rwkv) | [![arXiv:2505.14505](https://img.shields.io/badge/arXiv-2505.14505-b31b1b.svg)](https://arxiv.org/abs/2505.14505) | A multimodal fusion framework based on RWKV-7. |

---

## Images and Graphics

### Vision-Language Models

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| VisualRWKV | [![Star](https://img.shields.io/github/stars/howard-hou/VisualRWKV.svg?style=social&label=Star)](https://github.com/howard-hou/VisualRWKV) | [![arXiv:2406.13362](https://img.shields.io/badge/arXiv-2406.13362-b31b1b.svg)](https://arxiv.org/abs/2406.13362) | (COLING 2025) An RWKV-based vision-language model for visual tasks. |
| RWKV-CLIP | [![Star](https://img.shields.io/github/stars/deepglint/RWKV-CLIP.svg?style=social&label=Star)](https://github.com/deepglint/RWKV-CLIP) | [![arXiv:2406.06973](https://img.shields.io/badge/arXiv-2406.06973-b31b1b.svg)](https://arxiv.org/abs/2406.06973) | (EMNLP 2024) An RWKV-powered CLIP model for vision-language representation learning. |
| RWKV-UI |  | [![arXiv](https://img.shields.io/badge/arXiv-2502.03971-b31b1b)](https://arxiv.org/abs/2502.03971) | An RWKV-based vision-language model focused on UI understanding and design. |
| PestVL-Net |  | [![CVPR 2026 Findings](https://img.shields.io/badge/CVPR-2026%20Findings-blue)](https://openaccess.thecvf.com/content/CVPR2026F/html/Li_PestVL-Net_Enabling_Multimodal_Pest_Learning_Via_Fine-grained_Vision-Language_Interaction_CVPRF_2026_paper.html) | (CVPR 2026 Findings) A vision-language framework for fine-grained pest recognition. The visual branch combines RWKV with saliency-guided adaptive window partitioning; the language branch uses a multimodal large language model (MLLM) to generate descriptions from agricultural expert knowledge and multimodal chain-of-thought reasoning. |
| MCUVLM-RWKV |  | [![Paper](https://img.shields.io/badge/Paper-NSTL-orange)](https://opaj.napstic.cn/periodicalArticle/0120260300988014) | A lightweight vision-language model for STM32 microcontrollers, comprising a lightweight visual encoder, a feature mapper, and an RWKV decoder for image captioning under microcontroller resource constraints. |

### Vision Backbones

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Vision-RWKV (New Gen) | [![Star](https://img.shields.io/github/stars/xforcevesa/new-vrwkv.svg?style=social&label=Star)](https://github.com/xforcevesa/new-vrwkv) |  | A new generation of RWKV for vision, based on RWKV-7. |
| Vision-RWKV | [![Star](https://img.shields.io/github/stars/OpenGVLab/Vision-RWKV.svg?style=social&label=Star)](https://github.com/OpenGVLab/Vision-RWKV) | [![arXiv:2403.02308](https://img.shields.io/badge/arXiv-2403.02308-b31b1b.svg)](https://arxiv.org/abs/2403.02308) | (ICLR 2025 Spotlight) An RWKV-based visual perception model that scales smoothly to high-resolution images. |
| PointRWKV | [![Star](https://img.shields.io/github/stars/hithqd/PointRWKV.svg?style=social&label=Star)](https://github.com/hithqd/PointRWKV) | [![arXiv:2405.15214](https://img.shields.io/badge/arXiv-2405.15214-b31b1b.svg)](https://arxiv.org/abs/2405.15214) | (AAAI 2025) An RWKV-based framework for 3D point cloud learning. |
| RSRWKV | [![Star](https://img.shields.io/github/stars/Ling-yunchi/RSRWKV.svg?style=social&label=Star)](https://github.com/Ling-yunchi/RSRWKV) | [![arXiv:2503.20382](https://img.shields.io/badge/arXiv-2503.20382-b31b1b.svg)](https://arxiv.org/abs/2503.20382) | A high-resolution remote sensing framework for classification, object detection, segmentation, and other tasks. |
### Image Classification

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Vision_QRWKV | [![Star](https://img.shields.io/github/stars/ChiShengChen/Vision_QRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/Vision_QRWKV) | [![arXiv:2506.06633](https://img.shields.io/badge/arXiv-2506.06633-b31b1b.svg)](https://arxiv.org/abs/2506.06633) | A quantum-enhanced RWKV model for image classification. |
| Hi-RWKV | [![Star](https://img.shields.io/github/stars/HSI-Lab/Hi-RWKV.svg?style=social&label=Star)](https://github.com/HSI-Lab/Hi-RWKV) | [![IEEE TIP 2026](https://img.shields.io/badge/IEEE%20TIP-2026-blue)](https://doi.org/10.1109/TIP.2025.3648554) | (IEEE TIP 2026) A hierarchical RWKV model for hyperspectral image classification; the paper has been published and its code is publicly available. |

### Image Segmentation

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| U-RWKV | [![Star](https://img.shields.io/github/stars/hbyecoding/U-RWKV.svg?style=social&label=Star)](https://github.com/hbyecoding/U-RWKV) | [![arXiv:2507.11415](https://img.shields.io/badge/arXiv-2507.11415-b31b1b.svg)](https://arxiv.org/abs/2507.11415) | An RWKV-based image segmentation model. |
| RWKV-SAM | [![Star](https://img.shields.io/github/stars/HarborYuan/ovsam.svg?style=social&label=Star)](https://github.com/HarborYuan/ovsam) | [![arXiv:2406.19369](https://img.shields.io/badge/arXiv-2406.19369-b31b1b.svg)](https://arxiv.org/abs/2406.19369) | RWKV-SAM, an RWKV-based method for open-vocabulary image segmentation. |
| MMSegRWKV | [![Star](https://img.shields.io/github/stars/supercyt/MMSegRWKV.svg?style=social&label=Star)](https://github.com/supercyt/MMSegRWKV) |  | A multimodal magnetic resonance imaging (MRI) segmentation model based on the RWKV architecture. |
| BSBP-RWKV |  | [![ACM](https://img.shields.io/badge/ACM-Paper-red)](https://doi.org/10.1145/3664647.3681033) | RWKV-based medical image segmentation with background suppression and boundary preservation. |
| RWKV-UNet | [![Star](https://img.shields.io/github/stars/juntaoJianggavin/RWKV-UNet.svg?style=social&label=Star)](https://github.com/juntaoJianggavin/RWKV-UNet) | [![arXiv:2501.08458](https://img.shields.io/badge/arXiv-2501.08458-b31b1b.svg)](https://arxiv.org/abs/2501.08458) | A U-Net medical image segmentation model that uses RWKV to model long-range dependencies. |
| HFE-RWKV | [![Star](https://img.shields.io/github/stars/yezizi1022/HFE-RWKV.svg?style=social&label=Star)](https://github.com/yezizi1022/HFE-RWKV) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://doi.org/10.1109/ICASSP49660.2025.10888300) | (ICASSP 2025) A High-Frequency Enhanced RWKV model for medical image segmentation. |
| Zig-RiR | [![Star](https://img.shields.io/github/stars/txchen-USTC/Zig-RiR.svg?style=social&label=Star)](https://github.com/txchen-USTC/Zig-RiR) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://doi.org/10.1109/TMI.2025.3561797) | A medical image segmentation model combining zigzag scanning with an RWKV-in-RWKV architecture. |
| Diet-Seg |  | [![bioRxiv](https://img.shields.io/badge/bioRxiv-2025.05.31.657149-b31b1b.svg)](https://www.biorxiv.org/content/10.1101/2025.05.31.657149v1) | Medical image segmentation. |
| Med-URWKV |  | [![arXiv:2506.10858](https://img.shields.io/badge/arXiv-2506.10858-b31b1b.svg)](https://arxiv.org/abs/2506.10858) | A pure RWKV model pretrained on ImageNet for medical image segmentation. |
| SCRWKV | [![Star](https://img.shields.io/github/stars/zhxhzy/SCRWKV.svg?style=social&label=Star)](https://github.com/zhxhzy/SCRWKV) | [![arXiv:2605.14926](https://img.shields.io/badge/arXiv-2605.14926-b31b1b.svg)](https://arxiv.org/abs/2605.14926) | A structure-calibrated Vision-RWKV network for crack segmentation, combining multiscale texture modeling with a lightweight decoder; provides training, testing, and evaluation code. |
| SRWKV | [![Star](https://img.shields.io/github/stars/ukeLin/SRWKV.svg?style=social&label=Star)](https://github.com/ukeLin/SRWKV) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/11676832) | (IEEE TNNLS) A shape-guided RWKV network for medical image segmentation, using shape priors to guide sequence traversal and adaptive shifts to adjust the receptive field; the official implementation includes training and testing scripts and instructions for downloading weights. |
| RWKVFUSE | [![Star](https://img.shields.io/github/stars/alqurri/rwkv.svg?style=social&label=Star)](https://github.com/alqurri/rwkv) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/11515577) | (ISBI 2026) A medical image segmentation network with parallel VRWKV and CNN encoders, fusing local spatial features and long-range dependencies; the repository provides training and testing scripts for Synapse and ACDC. |
| FreRWKV-Net | [![Star](https://img.shields.io/github/stars/Stu-Ziyang-Zhang/FreRWKV-Net.svg?style=social&label=Star)](https://github.com/Stu-Ziyang-Zhang/FreRWKV-Net) | [![Springer](https://img.shields.io/badge/Springer-Article-red)](https://doi.org/10.1007/978-981-92-3495-0_14) | A frequency-guided retinal vessel segmentation network combining vessel differential attention (VDAM), frequency-domain direction prediction-driven FGD-RWKV, and multiscale frequency-spatial cross-attention (MS-FSCA); provides model, training, and testing code, but no pretrained weights. |
| SegRWKV | [![Star](https://img.shields.io/github/stars/luminescentfrr/SegRWKV.svg?style=social&label=Star)](https://github.com/luminescentfrr/SegRWKV) | [![JCDE 2026](https://img.shields.io/badge/Oxford-JCDE%202026-blue)](https://doi.org/10.1093/jcde/qwag065) | (JCDE) A biomedical segmentation framework with a URWKV backbone following the nnU-Net pipeline, covering abdominal MRI, endoscopy, and microscopy tasks; includes preprocessing, training, and evaluation scripts. |
| RWKVSegDiT | [![Star](https://img.shields.io/github/stars/alqurri/RWKVSegDiT.svg?style=social&label=Star)](https://github.com/alqurri/RWKVSegDiT) |  | A medical segmentation implementation with a hierarchical RWKV backbone that models segmentation as image-conditioned mask diffusion; includes ISIC data preparation, training, sampling, and evaluation scripts. |
| CropRWKV | [![Star](https://img.shields.io/github/stars/Shutong-Hou/CropRWKV.svg?style=social&label=Star)](https://github.com/Shutong-Hou/CropRWKV) |  | A study of linear-complexity RWKV segmentation for crop leaf lesion phenotyping, including a unified training protocol, multi-seed benchmarks, mixed-precision training failure diagnostics, and all source data tables; the manuscript has been submitted to *Plants*. |


### Image Generation

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Diffusion-RWKV | [![Star](https://img.shields.io/github/stars/feizc/Diffusion-RWKV.svg?style=social&label=Star)](https://github.com/feizc/Diffusion-RWKV) | [![arXiv:2404.04478](https://img.shields.io/badge/arXiv-2404.04478-b31b1b.svg)](https://arxiv.org/abs/2404.04478) | An RWKV-based image generation model suited to high-resolution images. |

### Object Detection

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| LION | [![Star](https://img.shields.io/github/stars/happinesslz/LION.svg?style=social&label=Star)](https://github.com/happinesslz/LION) | [![arXiv:2407.18232](https://img.shields.io/badge/arXiv-2407.18232-b31b1b.svg)](https://arxiv.org/abs/2407.18232) | (NeurIPS 2024) A Linear Group RNN for 3D object detection in point clouds, with RWKV support. |
| RWKV-VG | [![Star](https://img.shields.io/github/stars/nianfd/RWKV-VG.svg?style=social&label=Star)](https://github.com/nianfd/RWKV-VG) | [![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00530-025-01720-w) | A visual grounding framework based on the RWKV architecture. |
| Titanium-Strip-Defect |  | [![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0952197626003799) | An RWKV-inspired approach to context modeling and hierarchical differential fusion for titanium strip surface defect detection, replacing self-attention with linear-complexity context modules for industrial visual inspection. |

### Super-Resolution

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| OmniRWKVSR | [![Star](https://img.shields.io/github/stars/question110/omnirwkvsr.svg?style=social&label=Star)](https://github.com/question110/omnirwkvsr) | [![arXiv:2502.00404](https://img.shields.io/badge/arXiv-2502.00404-b31b1b.svg)](https://arxiv.org/abs/2502.00404) | An RWKV-based single-image super-resolution model. |
| Geometry-Aware RWKV | [![Star](https://img.shields.io/github/stars/chenzean/LF-RWKVNet.svg?style=social&label=Star)](https://github.com/chenzean/LF-RWKVNet) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://doi.org/10.1109/LSP.2025.3555445) | An RWKV-based geometry-aware model for light field image super-resolution. |
| Delta-WKV |  | [![arXiv](https://img.shields.io/badge/arXiv-2502.20852-b31b1b)](https://arxiv.org/abs/2502.20852) | (MICCAI 2025) An MRI super-resolution model. |
| MSB-RWKV |  | [![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s13042-025-02644-7) | Infrared image super-resolution. |

### Image Denoising and Enhancement

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| CRWKV | [![Star](https://img.shields.io/github/stars/Seeker98/CRWKV.svg?style=social&label=Star)](https://github.com/Seeker98/CRWKV) | [![arXiv:2505.02705](https://img.shields.io/badge/arXiv-2505.02705-b31b1b.svg)](https://arxiv.org/abs/2505.02705) | (IJCAI 2025) Efficient image denoising with a bidirectional WKV mechanism. |
| RWKV-IR | [![Star](https://img.shields.io/github/stars/YuzhenD/Resyn.svg?style=social&label=Star)](https://github.com/YuzhenD/Resyn) | [![arXiv:2412.03814](https://img.shields.io/badge/arXiv-2412.03814-b31b1b.svg)](https://arxiv.org/abs/2412.03814) | An RWKV-based image restoration method. |
| Restore-RWKV | [![Star](https://img.shields.io/github/stars/Yaziwel/Restore-RWKV.svg?style=social&label=Star)](https://github.com/Yaziwel/Restore-RWKV) | [![arXiv:2407.11087](https://img.shields.io/badge/arXiv-2407.11087-b31b1b.svg)](https://arxiv.org/abs/2407.11087) | Efficient and effective medical image restoration with RWKV, implemented in PyTorch. |
| SRCNet |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888780) | (ICASSP 2025) RWKV-based underwater image enhancement. |
| ID-RWKV |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10889384) | (ICASSP 2025) Efficient RWKV-based image deraining. |
| Flare-Aware RWKV |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888487) | (ICASSP 2025) Efficient RWKV-based image flare removal. |
| URWKV | [![Star](https://img.shields.io/github/stars/FZU-N/URWKV.svg?style=social&label=Star)](https://github.com/FZU-N/URWKV) | [![arXiv:2505.23068](https://img.shields.io/badge/arXiv-2505.23068-b31b1b.svg)](https://arxiv.org/abs/2505.23068) | (CVPR 2025) A unified RWKV model for low-light image restoration based on multi-state modeling. |
| Pan-Sharpening |  | [![IEEE](https://img.shields.io/badge/IEEE-11023855-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11023855) | (IEEE TGRS) RWKV-based pan-sharpening. |
| RetinexRWKV | [![Star](https://img.shields.io/github/stars/Alic-Li/RetinexRWKV.svg?style=social&label=Star)](https://github.com/Alic-Li/RetinexRWKV) |  | An RWKV-based model for low-light image enhancement. |
| DRWKV | [![Star](https://img.shields.io/github/stars/Bai-Xuecheng/DRWKV.svg?style=social&label=Star)](https://github.com/Bai-Xuecheng/DRWKV) | [![arXiv:2507.18594](https://img.shields.io/badge/arXiv-2507.18594-b31b1b.svg)](https://arxiv.org/abs/2507.18594) | Low-light image enhancement focused on object edges. |
| Fourier-RWKV | [![Star](https://img.shields.io/github/stars/Dilizlr/Fourier-RWKV.svg?style=social&label=Star)](https://github.com/Dilizlr/Fourier-RWKV) | [![arXiv:2512.08161](https://img.shields.io/badge/arXiv-2512.08161-b31b1b.svg)](https://arxiv.org/abs/2512.08161) | A multi-state-aware image dehazing network that extends WKV modeling to the frequency domain and combines deformable four-directional shifts with a semantic bridging module; provides training and testing code and downloadable weights. |
| CLUIE | [![Star](https://img.shields.io/github/stars/geekpool/CLUIE.svg?style=social&label=Star)](https://github.com/geekpool/CLUIE) | [![arXiv:2607.21467](https://img.shields.io/badge/arXiv-2607.21467-b31b1b.svg)](https://arxiv.org/abs/2607.21467) | (IEEE TIP) A clustering-aware RWKV framework for underwater image enhancement, using semantic dynamic reordering to construct content-adaptive recurrent trajectories and dark-response modulation to compensate for local structure; provides a PyTorch implementation. |
| EvRWKV | [![Star](https://img.shields.io/github/stars/Echo0517/EvRWKV.svg?style=social&label=Star)](https://github.com/Echo0517/EvRWKV) | [![arXiv:2507.03184](https://img.shields.io/badge/arXiv-2507.03184-b31b1b.svg)](https://arxiv.org/abs/2507.03184) | An event-guided low-light image enhancement framework that continually exchanges information between event streams and image features through Cross-RWKV and spectral fusion modules; the official implementation is open source. |

### Other Image Tasks

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| LALIC | [![Star](https://img.shields.io/github/stars/sjtu-medialab/RwkvCompress.svg?style=social&label=Star)](https://github.com/sjtu-medialab/RwkvCompress) | [![arXiv:2502.05741](https://img.shields.io/badge/arXiv-2502.05741-b31b1b.svg)](https://arxiv.org/abs/2502.05741) | (CVPR 2025) An RWKV-based image compression framework. |
| LineRWKV | [![Star](https://img.shields.io/github/stars/diegovalsesia/linerwkv.svg?style=social&label=Star)](https://github.com/diegovalsesia/linerwkv) | [![arXiv:2403.17677](https://img.shields.io/badge/arXiv-2403.17677-b31b1b.svg)](https://arxiv.org/abs/2403.17677) | A method for lossless and lossy compression of hyperspectral images. |
| OpenPAR | [![Star](https://img.shields.io/github/stars/Event-AHU/OpenPAR.svg?style=social&label=Star)](https://github.com/Event-AHU/OpenPAR) | [![arXiv:2504.10018](https://img.shields.io/badge/arXiv-2504.10018-b31b1b.svg)](https://arxiv.org/abs/2504.10018) | An open-source pedestrian attribute recognition framework that includes RWKV. |
| PathRWKV | [![Star](https://img.shields.io/github/stars/Puzzle-Logic/PathRWKV.svg?style=social&label=Star)](https://github.com/Puzzle-Logic/PathRWKV) | [![arXiv:2503.03199](https://img.shields.io/badge/arXiv-2503.03199-b31b1b.svg)](https://arxiv.org/abs/2503.03199) | An RWKV-based model for pathology whole-slide image analysis. |
| RWKVMatch |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888484) | (ICASSP 2025) Medical image registration using global and cross-fusion mechanisms based on Vision-RWKV. |
| EVA | [![Star](https://img.shields.io/github/stars/haohq19/eva.svg?style=social&label=Star)](https://github.com/haohq19/eva) | [![arXiv:2505.11165](https://img.shields.io/badge/arXiv-2505.11165-b31b1b.svg)](https://arxiv.org/abs/2505.11165) | An event vision framework with an asynchronous RWKV-6 encoder for recognition and detection using event camera data. |
| ChangeRWKV | [![Star](https://img.shields.io/github/stars/ChangeRWKV/ChangeRWKV.svg?style=social&label=Star)](https://github.com/ChangeRWKV/ChangeRWKV) | [![AAAI 2026](https://img.shields.io/badge/AAAI-2026-blue)](https://ojs.aaai.org/index.php/AAAI/article/view/38167) | (AAAI 2026) An RWKV-based change detection method with linear time complexity. |
| RWKV-CD |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/11456675) | A Vision-RWKV framework for building change detection in remote sensing, using dual-branch encoding, feature fusion, and noise suppression to process bi-temporal imagery. |
| MRT | [![Star](https://img.shields.io/github/stars/luke1453lh/MRT.svg?style=social&label=Star)](https://github.com/luke1453lh/MRT) | [![AAAI 2026](https://img.shields.io/badge/AAAI-2026-blue)](https://doi.org/10.1609/aaai.v40i9.37650) | (AAAI 2026) An extremely low-bitrate image compression model combining local Transformer attention within windows, bidirectional RWKV modeling across windows, an RWKV compression model, and a generative decoder; provides complete training, encoding, decoding, and evaluation scripts. |

---

## 3D and Video Processing

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| FEAT | [![Star](https://img.shields.io/github/stars/Yaziwel/FEAT.svg?style=social&label=Star)](https://github.com/Yaziwel/FEAT) | [![arXiv:2506.04956](https://img.shields.io/badge/arXiv-2506.04956-b31b1b.svg)](https://arxiv.org/abs/2506.04956) | (MICCAI 2025, early accepted) RWKV-based medical video generation. |
| TLS-RWKV |  | [![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11063-024-11540-0) | RWKV-based online action detection (OAD). |
| Video RWKV |  | [![arXiv:2411.05636](https://img.shields.io/badge/arXiv-2411.05636-b31b1b.svg)](https://arxiv.org/abs/2411.05636) | RWKV-based video action recognition. |
| StyleRWKV |  | [![arXiv:2412.19535](https://img.shields.io/badge/arXiv-2412.19535-b31b1b.svg)](https://arxiv.org/abs/2412.19535) | Efficient video style transfer with an RWKV-like architecture. |
| RainRWKV |  | [![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00371-025-03965-y) | Efficient RWKV-based video deraining. |
| RWKV3D |  | [![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3746027.3755658) | (ACM MM 2025) An RWKV model for point cloud analysis, combining local feature mixing with bidirectional multi-head shifts; supports training from scratch and both unimodal and cross-modal pretraining. |
| RWKV-PCSSC | [![Star](https://img.shields.io/github/stars/shuaiqianende/RWKVPCSSC.svg?style=social&label=Star)](https://github.com/shuaiqianende/RWKVPCSSC) | [![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3746027.3754908) | (ACM MM 2025) A point cloud semantic scene completion network that reconstructs scenes with an RWKV seed generator and progressive point deconvolution, using approximately 1/4.18 as many parameters as PointSSC; the official repository is open source. |
| PointDGRWKV |  | [![arXiv:2508.20835](https://img.shields.io/badge/arXiv-2508.20835-b31b1b.svg)](https://arxiv.org/abs/2508.20835) | An RWKV framework for point cloud classification in unseen domains, combining geometry-aware shifts with cross-domain feature alignment; the author's repository exists, but the code has not yet been released. |
| P-RWKV / PointER |  | [![arXiv:2606.10395](https://img.shields.io/badge/arXiv-2606.10395-b31b1b.svg)](https://arxiv.org/abs/2606.10395) | A P-RWKV module for point clouds and the PointER self-supervised representation learning framework, modeling irregular 3D geometry through local perception expansion and spatial context enhancement; the paper states that code will be released upon acceptance. |
| Otter |  | [![AAAI 2026](https://img.shields.io/badge/AAAI-2026-blue)](https://ojs.aaai.org/index.php/AAAI/article/view/37428) | (AAAI 2026 Oral) An enhanced RWKV model for wide-view few-shot action recognition, suppressing background interference through subject emphasis and temporal reconstruction. |
| MG-RWKV |  | [![arXiv:2607.00902](https://img.shields.io/badge/arXiv-2607.00902-b31b1b.svg)](https://arxiv.org/abs/2607.00902) | (ECCV 2026) A multigranular RWKV framework for temporal forgery localization in audio and video, combining bidirectional RWKV, multigranular expert routing, and cross-granularity consistency constraints to locate manipulated segments with O(T) complexity. |
| VRWKV-Editor | [![Star](https://img.shields.io/github/stars/abdo-RG/VRWKV-Editor.svg?style=social&label=Star)](https://github.com/abdo-RG/VRWKV-Editor) | [![Springer](https://img.shields.io/badge/Springer-Multimedia%20Systems-red)](https://doi.org/10.1007/s00530-026-02649-4) | (Multimedia Systems 2026) Replaces quadratic spatiotemporal attention in diffusion-based video editing with linear 3D-VRWKV aggregation using bidirectional Bi-WKV; supports object replacement, background modification, and style transfer within a Tune-A-Video pipeline, with training and editing code. |

---

## Audio

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| MIDI-RWKV | [![Star](https://img.shields.io/github/stars/christianazinn/MIDI-RWKV.svg?style=social&label=Star)](https://github.com/christianazinn/MIDI-RWKV) | [![arXiv:2506.13001](https://img.shields.io/badge/arXiv-2506.13001-b31b1b.svg)](https://arxiv.org/abs/2506.13001) | RWKV-based music generation. |
| RWKV-TTS | [![Star](https://img.shields.io/github/stars/yynil/RWKVTTS.svg?style=social&label=Star)](https://github.com/yynil/RWKVTTS) | [![arXiv:2504.03289](https://img.shields.io/badge/arXiv-2504.03289-b31b1b.svg)](https://arxiv.org/abs/2504.03289) | An RWKV speech synthesis model supporting multilingual text-to-speech. |
| RWKV-ASR | [![Star](https://img.shields.io/github/stars/AGENDD/RWKV-ASR.svg?style=social&label=Star)](https://github.com/AGENDD/RWKV-ASR) |  | **Speech recognition** using a pretrained RWKV language model. |
| Rate-Aware |  | [![arXiv](https://img.shields.io/badge/arXiv-2501.11999-b31b1b)](https://arxiv.org/abs/2501.11999) | An RWKV-based speech compression method. |
| Con-RWKV | [![Star](https://img.shields.io/github/stars/NYCU-MLLab/Con-RWKV.svg?style=social&label=Star)](https://github.com/NYCU-MLLab/Con-RWKV) |  | An RWKV-based speech recognition model. |
| AudioRWKV | [![Star](https://img.shields.io/github/stars/Jiayu-Xiong/AudioRWKV.svg?style=social&label=Star)](https://github.com/Jiayu-Xiong/AudioRWKV) | [![arXiv:2509.02167](https://img.shields.io/badge/arXiv-2509.02167-b31b1b.svg)](https://arxiv.org/abs/2509.02167) | A bidirectional audio pattern recognition model based on RWKV-7. |

---

## Time Series

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| BlackGoose_Rimer | [![Star](https://img.shields.io/github/stars/Alic-Li/BlackGoose_Rimer.svg?style=social&label=Star)](https://github.com/Alic-Li/BlackGoose_Rimer) | [![arXiv:2503.06121](https://img.shields.io/badge/arXiv-2503.06121-b31b1b.svg)](https://arxiv.org/abs/2503.06121) | An RWKV-7 time series forecasting model supporting a variety of time series tasks. |
| RWKV-TS | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-TS.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-TS) | [![arXiv:2401.09093](https://img.shields.io/badge/arXiv-2401.09093-b31b1b.svg)](https://arxiv.org/abs/2401.09093) | An RWKV-based time series model supporting forecasting, classification, anomaly detection, imputation, and other tasks. |
| MSRWKV-2DTCN |  | [![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0360544224028433) | Short-term photovoltaic power forecasting using multiscale RWKV. |
| AutoGMM-RWKV |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10729884) | An RWKV-based approach to detecting selective forwarding attacks in wireless sensor networks. |
| DFT | [![Star](https://img.shields.io/github/stars/cq-dong/DFT_25.svg?style=social&label=Star)](https://github.com/cq-dong/DFT_25) | [![arXiv:2411.06065](https://img.shields.io/badge/arXiv-2411.06065-b31b1b.svg)](https://arxiv.org/abs/2411.06065) | An RWKV-based stock price prediction method. |
| MATCC | [![Star](https://img.shields.io/github/stars/dyccolin/MATCC.svg?style=social&label=Star)](https://github.com/dyccolin/MATCC) | [![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3627673.3679715) | A stock price prediction framework that combines market trends and cross-time correlations with RWKV modeling. |
| ET_MGNN | [![Star](https://img.shields.io/github/stars/BrainFC/ET_MGNN.svg?style=social&label=Star)](https://github.com/BrainFC/ET_MGNN) | [![Paper](https://img.shields.io/badge/Paper-SSRN-orange)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5114041) | A multimodal dynamic brain graph representation learning model that uses RWKV for temporal modeling and brain disorder diagnosis. |
| TabulaTime |  | [![arXiv](https://img.shields.io/badge/arXiv-2502.17049-b31b1b)](https://arxiv.org/abs/2502.17049) | A time series model for ACS prediction. |
| LASTGCN |  | [![Scientific Reports](https://img.shields.io/badge/Scientific%20Reports-2025-green)](https://www.nature.com/articles/s41598-025-93179-y) | Spatiotemporal multi-graph traffic flow forecasting with RWKV. |
| DREMnet |  | [![arXiv](https://img.shields.io/badge/arXiv-2503.22223-b31b1b)](https://arxiv.org/abs/2503.22223) | Electromagnetic signal denoising. |
| RWKV-TDR7 |  | [![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.22544) | Motion trajectory planning for inverse kinematics. |
| MolRWKV | [![Star](https://img.shields.io/github/stars/bigwestHan/MolRWKV.svg?style=social&label=Star)](https://github.com/bigwestHan/MolRWKV) | [![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.70100) | An RWKV conditional molecular generation model combining local and graph enhancement. |
| QuantumRWKV | [![Star](https://img.shields.io/github/stars/ChiShengChen/QuantumRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/QuantumRWKV) | [![arXiv:2505.13524](https://img.shields.io/badge/arXiv-2505.13524-b31b1b.svg)](https://arxiv.org/abs/2505.13524) | An RWKV model using quantum-enhanced channel mixing for time series forecasting. |
| STWGRL |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-11002535-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11002535) | (IEEE IoT-J) Time series anomaly detection with RWKV as a core module. |
| MP-RWKV |  | [![MDPI](https://img.shields.io/badge/MDPI-Article-green)](https://www.mdpi.com/2673-4591/97/1/26) | RWKV-based long-term electrical load forecasting. |

---

## Robotics and Embodied Intelligence

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| DecisionRWKV | [![Star](https://img.shields.io/github/stars/ancorasir/DecisionRWKV.svg?style=social&label=Star)](https://github.com/ancorasir/DecisionRWKV) | [![arXiv:2407.16306](https://img.shields.io/badge/arXiv-2407.16306-b31b1b.svg)](https://arxiv.org/abs/2407.16306) | (JCISE) Combines experience replay with Decision-RWKV for lifelong learning in robotics. |
| OccRWKV | [![Star](https://img.shields.io/github/stars/jmwang0117/OccRWKV.svg?style=social&label=Star)](https://github.com/jmwang0117/OccRWKV) | [![arXiv:2409.19987](https://img.shields.io/badge/arXiv-2409.19987-b31b1b.svg)](https://arxiv.org/abs/2409.19987) | (ICRA 2025) Efficient 3D semantic occupancy prediction with linear complexity. |

---

## RWKV Tokenizers

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| rwkv-tokenizer | [![Star](https://img.shields.io/github/stars/cahya-wirawan/rwkv-tokenizer.svg?style=social&label=Star)](https://github.com/cahya-wirawan/rwkv-tokenizer) |  | A fast RWKV tokenizer written in Rust, supporting RWKV-V5/6 World models. |
| rwkv_tokenizer.c | [![Star](https://img.shields.io/github/stars/mrsteyk/rwkv_tokenizer.c.svg?style=social&label=Star)](https://github.com/mrsteyk/rwkv_tokenizer.c) |  | An RWKV trie tokenizer written in C. |
| rwkv-tokenizer-go | [![Star](https://img.shields.io/github/stars/Ronsor/rwkv-tokenizer-go.svg?style=social&label=Star)](https://github.com/Ronsor/rwkv-tokenizer-go) |  | An RWKV tokenizer written in Go. |
| RWKV-World-Tokenizer-CPP | [![Star](https://img.shields.io/github/stars/m8than/RWKV-World-Tokenizer-CPP.svg?style=social&label=Star)](https://github.com/m8than/RWKV-World-Tokenizer-CPP) |  | A highly optimized trie tokenizer for RWKV World models, written in C++. |

---

## RAG Systems for RWKV

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| RWKV-RAG | [![Star](https://img.shields.io/github/stars/AIIRWKV/RWKV-RAG.svg?style=social&label=Star)](https://github.com/AIIRWKV/RWKV-RAG) |  | A one-click retrieval-augmented generation (RAG) deployment system based on RWKV, with local knowledge base creation and management, a knowledge-based question-answering chatbot, and one-click RWKV fine-tuning. |

---

## Chatbots and Inference API Servers

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| **⭐ (Recommended for Chinese Users)** RWKV Runner | [![Star](https://img.shields.io/github/stars/josStorer/RWKV-Runner.svg?style=social&label=Star)](https://github.com/josStorer/RWKV-Runner) |  | A tool for managing and launching RWKV models, with a user-friendly graphical interface and support for training and inference. |
| **⭐ (Recommended for Chinese Users)** AI00 RWKV Server | [![Star](https://img.shields.io/github/stars/Ai00-X/ai00_server.svg?style=social&label=Star)](https://github.com/Ai00-X/ai00_server) |  | An RWKV **inference API server** built on the web-rwkv inference engine. |
| RWKV_APP | [![Star](https://img.shields.io/github/stars/RWKV-APP/RWKV_APP.svg?style=social&label=Star)](https://github.com/RWKV-APP/RWKV_APP) |  | An on-device RWKV-LM inference app built with Flutter. |
| **🇨🇳 (Chinese)** Role Play Chatbot | [![Star](https://img.shields.io/github/stars/shengxia/RWKV_Role_Playing.svg?style=social&label=Star)](https://github.com/shengxia/RWKV_Role_Playing) |  | A Gradio-based role-playing WebUI powered by RWKV. |
| Easy_RWKV_webui | [![Star](https://img.shields.io/github/stars/No-22-Github/Easy_RWKV_webui.svg?style=social&label=Star)](https://github.com/No-22-Github/Easy_RWKV_webui) |  | An online chat room for RWKV models, built with PyWebIO. |
| Mini Model Daemon | [![Star](https://img.shields.io/github/stars/recursal/minmodmon.svg?style=social&label=Star)](https://github.com/recursal/minmodmon) |  | An RWKV inference tool using the web-rwkv backend. |
| frank_esp32 | [![Star](https://img.shields.io/github/stars/lsk-china/frank_esp32.svg?style=social&label=Star)](https://github.com/lsk-china/frank_esp32) |  | A hardware implementation of the RWKV-powered Firefly chatbot. |
| RWKV State Agent | [![Star](https://img.shields.io/github/stars/123123213weqw/rwkv-agent.svg?style=social&label=Star)](https://github.com/123123213weqw/rwkv-agent) |  | A local agent runtime centered on RWKV recurrent states, supporting state reuse across turns, structured tool calls, and state isolation across tasks; provides web search, command, and file tools. |
| rwkv_lightning | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/rwkv_lightning.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/rwkv_lightning) |  | An RWKV batch inference backend built on Albatross and FastAPI, with NVIDIA CUDA and AMD ROCm execution paths, quantized inference, and serving interfaces. |
| RWKV-Server | [![Star](https://img.shields.io/github/stars/AUXStar/RWKV-Server.svg?style=social&label=Star)](https://github.com/AUXStar/RWKV-Server) |  | An RWKV batch inference server for concurrent requests, with an OpenAI-compatible API, server-sent events (SSE) streaming, recurrent-state reuse, and dynamic batching. |
| RWKV-Router | [![Star](https://img.shields.io/github/stars/cgisky1980/rwkv-router.svg?style=social&label=Star)](https://github.com/cgisky1980/rwkv-router) |  | A request-routing gateway using rules and a small RWKV classifier to categorize requests and route them to local models or cloud APIs; provides OpenAI- and Anthropic-compatible interfaces and bindings for multiple languages. |
| RWKV-Scout | [![Star](https://img.shields.io/github/stars/rwkv-rs/RWKV-Scout.svg?style=social&label=Star)](https://github.com/rwkv-rs/RWKV-Scout) |  | A web-search agent with RWKV at its decision-making core, covering task decomposition, query and tool selection, evidence review, and answer generation while recording evidence and execution traces. |
| rwkv_lightning_cuda | [![Star](https://img.shields.io/github/stars/Alic-Li/rwkv_lightning_cuda.svg?style=social&label=Star)](https://github.com/Alic-Li/rwkv_lightning_cuda) |  | An RWKV-7 inference service for NVIDIA CUDA with an additional AMD HIP path, providing OpenAI-compatible and native batch APIs, streaming, state caching, state fine-tuning, and quantization. |
| RWKV-LH | [![Star](https://img.shields.io/github/stars/rwkv-rs/RWKV-LH.svg?style=social&label=Star)](https://github.com/rwkv-rs/RWKV-LH) |  | An experimental coding agent for RWKV state-continuation models, combining decision and execution models with an on-demand planning model; supports tool execution, completion-condition checks, and recovery after interruption. |
| RWKV_Role_Playing_with_GPT-SoVITS | [![Star](https://img.shields.io/github/stars/v3ucn/RWKV_Role_Playing_with_GPT-SoVITS.svg?style=social&label=Star)](https://github.com/v3ucn/RWKV_Role_Playing_with_GPT-SoVITS) |  | Adds GPT-SoVITS voice conversations to an RWKV role-playing WebUI, with character configuration and local execution; suited to single-user use. |
| RWKV-Agent | [![Star](https://img.shields.io/github/stars/No-22-Github/RWKV-Agent.svg?style=social&label=Star)](https://github.com/No-22-Github/RWKV-Agent) |  | A local-first RWKV workspace agent for Apple Silicon, using Go and MLX inference, with command-line, terminal UI, desktop, and browser interfaces; its current tools primarily support read-only operations. |

---

## RWKV Benchmarks

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| Uncheatable Eval | [![Star](https://img.shields.io/github/stars/Jellyfish042/uncheatable_eval.svg?style=social&label=Star)](https://github.com/Jellyfish042/uncheatable_eval) | [![arXiv:2609.27510](https://img.shields.io/badge/arXiv-2609.27510-b31b1b.svg)](https://arxiv.org/abs/2609.27510) | Evaluates language models, including RWKV, using continually updated text and lossless compression rates. |
| RULER_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/RULER_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/RULER_RWKV) |  | [RULER](https://arxiv.org/abs/2404.06654) benchmark scores for RWKV models. |
| LongBench_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/LongBench_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/LongBench_RWKV) |  | [LongBench](https://arxiv.org/abs/2308.14508) benchmark scores for RWKV. |
| rwkv_mmlu | [![Star](https://img.shields.io/github/stars/Jellyfish042/rwkv_mmlu.svg?style=social&label=Star)](https://github.com/Jellyfish042/rwkv_mmlu) |  | MMLU benchmark scores for RWKV models. |

---

## RWKV Inference Frameworks and Kernel Libraries

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| rwkv_Ascend | [![Star](https://img.shields.io/github/stars/appleinsky/rwkv_Ascend.svg?style=social&label=Star)](https://github.com/appleinsky/rwkv_Ascend) |  | A kernel repository jointly developed by Ascend and RWKV. |
| rwkv7.c | [![Star](https://img.shields.io/github/stars/KevlarKanou/rwkv7.c.svg?style=social&label=Star)](https://github.com/KevlarKanou/rwkv7.c) |  | A C implementation of RWKV-7 for model inference. |
| rwkv.cpp | [![Star](https://img.shields.io/github/stars/RWKV/rwkv.cpp.svg?style=social&label=Star)](https://github.com/RWKV/rwkv.cpp) |  | CPU inference for RWKV models, supporting FP16 and quantized INT4, INT5, and INT8 inference. |
| RWKVSharp | [![Star](https://img.shields.io/github/stars/imxcstar/RWKVSharp.svg?style=social&label=Star)](https://github.com/imxcstar/RWKVSharp) |  | A C# wrapper for RWKV inference based on rwkv.cpp, supporting RWKV4/RWKV5/RWKV6/RWKV7 World models. |
| RWKV_Pytorch | [![Star](https://img.shields.io/github/stars/yuunnn-w/RWKV_Pytorch.svg?style=social&label=Star)](https://github.com/yuunnn-w/RWKV_Pytorch) |  | An RWKV model inference framework implemented in pure PyTorch. |
| rwkv-kit | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/rwkv-kit.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/rwkv-kit) |  | An RWKV inference framework supporting batch inference, parallel inference and training, and other features. |
| web-rwkv | [![Star](https://img.shields.io/github/stars/cryscan/web-rwkv.svg?style=social&label=Star)](https://github.com/cryscan/web-rwkv) |  | RWKV inference implemented entirely in WebGPU and Rust. |
| candle-rwkv | [![Star](https://img.shields.io/github/stars/nkypy/candle-rwkv.svg?style=social&label=Star)](https://github.com/nkypy/candle-rwkv) |  | RWKV inference with quantization support in Candle, a minimalist machine learning framework for Rust. |
| **🚧 (In Development)** RWKV7-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV7-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV7-Keras) |  | A Keras implementation of RWKV with training and inference support. |
| jaxrwkv | [![Star](https://img.shields.io/github/stars/bsarkar321/jaxrwkv.svg?style=social&label=Star)](https://github.com/bsarkar321/jaxrwkv) |  | A JAX implementation of the RWKV language model. |
| rwkv-mobile | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-mobile.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-mobile) |  | An RWKV inference engine for mobile devices. |
| rwkv-qualcomm | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-qualcomm.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-qualcomm) |  | RWKV inference using the Qualcomm AI Engine Direct SDK. |
| rwkv-by-hand-excel | [![Star](https://img.shields.io/github/stars/playaswd/rwkv-by-hand-excel.svg?style=social&label=Star)](https://github.com/playaswd/rwkv-by-hand-excel) |  | An Excel implementation of RWKV that helps developers explore how RWKV works. |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) |  | RWKV-V6/V7 inference using FLA, with support for combining multiple states. |
| RWKV-DeepEmbed-mmap | [![Star](https://img.shields.io/github/stars/Beortext/RWKV-DeepEmbed-mmap.svg?style=social&label=Star)](https://github.com/Beortext/RWKV-DeepEmbed-mmap) |  | An efficient RWKV DeepEmbed inference approach using mmap. |
| wkvm | [![Star](https://img.shields.io/github/stars/xiaol/wkvm.svg?style=social&label=Star)](https://github.com/xiaol/wkvm) |  | A state-based inference framework for linear and hybrid models such as RWKV-7, GDN, and Mamba2; manages requests through fixed-size state slots and supports state snapshots, branching, hibernation, and restoration. |
| RWKV-7 Hugging Face Reference | [![Star](https://img.shields.io/github/stars/rwkv-rs/hf-adapter.svg?style=social&label=Star)](https://github.com/rwkv-rs/hf-adapter) |  | A pure PyTorch RWKV-7 reference implementation for Hugging Face Transformers, with separate model configuration, recurrent caches, and kernels; provides weight conversion tools and optional interfaces to NVIDIA-accelerated kernels. |
| FlashRWKV2 | [![Star](https://img.shields.io/github/stars/rwkv-rs/FlashRWKV2.svg?style=social&label=Star)](https://github.com/rwkv-rs/FlashRWKV2) |  | A TileLang-based RWKV-7 GPU kernel library, with a BF16 forward path shared by training and inference, FP32 accumulation and recurrent states, and fused kernel interfaces for inference. |
| RWKV-MUSA | [![Star](https://img.shields.io/github/stars/KakaruHayate/RWKV-MUSA.svg?style=social&label=Star)](https://github.com/KakaruHayate/RWKV-MUSA) |  | RWKV-7 recurrent kernels and model integration for Moore Threads GPUs, with an optional `torch_musa` backend, Hugging Face integration, and a PyTorch reference computation path. |
| rwkv-hf-kernels | [![Star](https://img.shields.io/github/stars/Hakureirm/rwkv-hf-kernels.svg?style=social&label=Star)](https://github.com/Hakureirm/rwkv-hf-kernels) |  | Optional fused CUDA kernels for the RWKV-7 model in Hugging Face Transformers, with a portable PyTorch implementation as the reference path. |
| rwkv-quant | [![Star](https://img.shields.io/github/stars/RafaelUI/rwkv-quant.svg?style=social&label=Star)](https://github.com/RafaelUI/rwkv-quant) |  | An RWKV-7 quantization toolkit and Metal inference backend for Apple Silicon, with a portable `.rwkvq` checkpoint format, calibration, and GPU kernels that read quantized weights directly. |
| RWKV-7 Quantization Toolkit | [![Star](https://img.shields.io/github/stars/AUXStar/rwkv7-quantization.svg?style=social&label=Star)](https://github.com/AUXStar/rwkv7-quantization) |  | An RWKV-7 quantization and inference toolkit supporting FP8, INT8, INT4, and other schemes, with commands for inspecting model information, comparing models before and after quantization, and evaluation. |
| rwkv-rsv | [![Star](https://img.shields.io/github/stars/cgisky1980/rwkv-rsv.svg?style=social&label=Star)](https://github.com/cgisky1980/rwkv-rsv) |  | An RWKV-7 inference engine implemented in Rust with Vulkan/CUDA compute shaders, supporting FP16 and INT8 weight paths and a CPU FP32 reference implementation for accuracy comparisons. |
| rwkv_mobile_flutter | [![Star](https://img.shields.io/github/stars/RWKV-APP/rwkv_mobile_flutter.svg?style=social&label=Star)](https://github.com/RWKV-APP/rwkv_mobile_flutter) |  | A foreign function interface (FFI) plugin and runtime orchestration layer connecting Flutter/Dart apps to the native rwkv-mobile inference engine for on-device RWKV, speech, and multimodal integration. |
| VKWR | [![Star](https://img.shields.io/github/stars/szxysdt/VKWR.svg?style=social&label=Star)](https://github.com/szxysdt/VKWR) |  | An RWKV inference engine with optimized CUDA kernels and continuous batching, providing command-line launch and an OpenAI-compatible API service; still under development. |
| rosalia | [![Star](https://img.shields.io/github/stars/cryscan/rosalia.svg?style=social&label=Star)](https://github.com/cryscan/rosalia) |  | An RWKV inference engine implemented in Rust with Vulkan compute shaders, exploring the Rosa mechanism in a standalone runtime. |
| RWKV-7 × sglang | [![Star](https://img.shields.io/github/stars/Hakureirm/rwkv-sglang.svg?style=social&label=Star)](https://github.com/Hakureirm/rwkv-sglang) |  | An inference serving implementation integrating RWKV-7 with SGLang, with recurrent-state inference, INT8/INT4 quantization, OpenAI-compatible serving, and recorded benchmark comparisons against a reference implementation. |
| vllm-rwkv | [![Star](https://img.shields.io/github/stars/123123213weqw/vllm-rwkv.svg?style=social&label=Star)](https://github.com/123123213weqw/vllm-rwkv) |  | A vLLM distribution integrating native RWKV-7 recurrent-state scheduling and Albatross-derived CUDA kernels, with dynamic state management, batching, and OpenAI-compatible serving. |
| HTMLNLM | [![Star](https://img.shields.io/github/stars/ConsciousNode/HTMLNLM.svg?style=social&label=Star)](https://github.com/ConsciousNode/HTMLNLM) |  | A single-file, browser-based neural language model runtime built on RWKV-v7, supporting model training and inference in a web page without a separate server or Python environment. |

---

## Other RWKV Projects

| Title | Code | Paper | Description |
| :--- | :--- | :--- | :--- |
| SocialDeductionLLM | [![Star](https://img.shields.io/github/stars/SocialDeductionLLM/SocialDeductionLLM.svg?style=social&label=Star)](https://github.com/SocialDeductionLLM/SocialDeductionLLM) | [![arXiv:2502.06060](https://img.shields.io/badge/arXiv-2502.06060-b31b1b.svg)](https://arxiv.org/abs/2502.06060) | (AAMAS 2025) Multi-agent reinforcement learning. |
| JSONL to binidx | [![Star](https://img.shields.io/github/stars/Abel2076/json2binidx_tool.svg?style=social&label=Star)](https://github.com/Abel2076/json2binidx_tool) |  | A tool for converting `.jsonl` files into `.bin`/`.idx` (binidx) data for RWKV training. |
| RWKV-IF | [![Star](https://img.shields.io/github/stars/Lyttr/RWKVInverseFolding.svg?style=social&label=Star)](https://github.com/Lyttr/RWKVInverseFolding) | [![bioRxiv](https://img.shields.io/badge/bioRxiv-green)](https://www.biorxiv.org/content/10.1101/2025.06.13.659654v1.full.pdf) | An efficient, controllable RNA inverse-folding design framework based on RWKV. |
| PCF-RWKV |  | [![Paper](https://img.shields.io/badge/Paper-Preprint-yellow)](https://www.preprints.org/manuscript/202412.1705/v1) | A product carbon footprint estimation system based on RWKV. |
| ChemRB |  | [![Paper](https://img.shields.io/badge/Paper-SNNU-orange)](https://jsnu.magtech.com.cn/CN/10.15983/j.cnki.jsnu.2025005) | Molecule generation for medical applications. |
| DualComp |  | [![arXiv:2505.16256](https://img.shields.io/badge/arXiv-2505.16256-b31b1b.svg)](https://arxiv.org/abs/2505.16256) | Lossless data compression based on RWKV-7. |
| Ai00 Character Maker | [![Star](https://img.shields.io/github/stars/Ai00-X/Ai00-character-maker.svg?style=social&label=Star)](https://github.com/Ai00-X/Ai00-character-maker) |  | A synthetic data generation tool for RWKV role-playing. |
| RWKV-DPA |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Article-blue)](https://ieeexplore.ieee.org/document/10779439) | A linear-attention channel estimation method for vehicle-to-everything (V2X) communications. |
| RWKV_7_on_AMD_Radeon-Instinct | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV_7_on_AMD_Radeon-Instinct.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV_7_on_AMD_Radeon-Instinct) |  | A complete workflow for deploying RWKV-7 on AMD Radeon and Instinct GPUs. |
| RWKV-PEFT-GUI | [![Star](https://img.shields.io/github/stars/cttailearn/RWKV-PEFT-GUI.svg?style=social&label=Star)](https://github.com/cttailearn/RWKV-PEFT-GUI) |  | A graphical tool for processing datasets for RWKV models. |
| RWKV-nonogram | [![Star](https://img.shields.io/github/stars/LeC-Z/RWKV-nonogram.svg?style=social&label=Star)](https://github.com/LeC-Z/RWKV-nonogram) |  | An experimental project using an approximately 20M-parameter RWKV-6 model to solve nonogram puzzles, with a demo and a Colab entry point. |
| Sudoku-RWKV | [![Star](https://img.shields.io/github/stars/Jellyfish042/Sudoku-RWKV.svg?style=social&label=Star)](https://github.com/Jellyfish042/Sudoku-RWKV) |  | An RWKV-6 Sudoku-solving model with an interactive demo, a minimal inference example, and training data generation scripts. |
| RWKV-15Puzzle | [![Star](https://img.shields.io/github/stars/Jellyfish042/RWKV-15Puzzle.svg?style=social&label=Star)](https://github.com/Jellyfish042/RWKV-15Puzzle) |  | An RWKV-6 model specialized for the 15-puzzle, with a graphical demo, a minimal inference entry point, and training configuration instructions. |

