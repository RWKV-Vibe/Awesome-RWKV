---

[English Version](README_en.md)

---

# RWKV 生态项目一览

一份精选的 RWKV 生态系统中的优秀项目、工具和资源的列表。

## 目录

- [RWKV 官方链接](#rwkv-官方链接)
- [RWKV 微调与训练](#rwkv-微调与训练)
  - [微调项目](#微调项目)
  - [训练项目](#训练项目)
- [模型架构与优化](#模型架构与优化)
- [自然语言处理](#自然语言处理)
- [多模态融合](#多模态融合)
- [图像与图形](#图像与图形)
  - [视觉语言](#视觉语言)
  - [视觉骨干网络](#视觉骨干网络)
  - [图像分类](#图像分类)
  - [图像分割](#图像分割)
  - [图像生成](#图像生成)
  - [目标检测](#目标检测)
  - [超分辨率](#超分辨率)
  - [图像去噪/图像增强](#图像去噪图像增强)
  - [其他图像任务](#其他图像任务)
- [3D 与视频处理](#3d-与视频处理)
- [音频相关](#音频相关)
- [时间序列](#时间序列)
- [机器人与具身智能](#机器人与具身智能)
- [RWKV 分词器](#rwkv-分词器)
- [RWKV 的 RAG 系统](#rwkv-的-rag-系统)
- [聊天机器人与推理 API 服务器](#聊天机器人与推理-api-服务器)
- [RWKV 基准测试](#rwkv-基准测试)
- [RWKV 推理框架与算子库](#rwkv-推理框架与算子库)
- [其他 RWKV 项目](#其他-rwkv-项目)

---

## RWKV 官方链接

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| RWKV-LM | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM) | | RWKV 的官方代码仓库，提供了 RWKV v1 至 v7 各版本的架构代码，以及配套的大语言模型训练实现。 |
| RWKV-4 架构论文 | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v4) | [![arXiv:2305.13048](https://img.shields.io/badge/arXiv-2305.13048-b31b1b.svg)](https://arxiv.org/abs/2305.13048) | RWKV-4 的架构论文。 |
| RWKV 5/6 架构论文 | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v5) | [![arXiv:2404.05892](https://img.shields.io/badge/arXiv-2404.05892-b31b1b.svg)](https://arxiv.org/abs/2404.05892) | RWKV-5/6 的架构论文。 |
| RWKV-7 架构论文 | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v7)| [![arXiv:2503.14456](https://img.shields.io/badge/arXiv-2503.14456-b31b1b.svg)](https://arxiv.org/abs/2503.14456) | RWKV-7 的架构论文。 |
| RWKV pip 包 | [![PyPI](https://img.shields.io/pypi/v/rwkv.svg)](https://pypi.org/project/rwkv/)| | RWKV 的 pip 包，具体用法可以查看 [RWKV 官网](https://rwkv.cn/tutorials/intermediate/RWKVpip)。 |
| RWKV-CUDA | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-CUDA.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-CUDA) | | RWKV 的官方 CUDA 算子。 |
| Hugging Face 文档 | [![🤗 RWKV](https://img.shields.io/badge/🤗%20RWKV-blue)](https://huggingface.co/docs/transformers/model_doc/rwkv) | | Hugging Face 关于 RWKV 的介绍。 |
| rwkvcn-docs | [![Star](https://img.shields.io/github/stars/LeoLin4258/rwkvcn-docs.svg?style=social&label=Star)](https://github.com/LeoLin4258/rwkvcn-docs) | | RWKV 的中文文档项目链接 |
| RWKV.com | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV.com.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV.com) | | RWKV 的英文官网项目链接 |

---

## RWKV 微调与训练

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|RWKV-Development-Tools | [![Star](https://img.shields.io/github/stars/Ourboros-Alignment-Team/RWKV-Development-Tools.svg?style=social&label=Star)](https://github.com/Ourboros-Alignment-Team/RWKV-Development-Tools) | | 面向RWKV模型的研究平台，功能丰富的集成工具包 |

### 微调项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| **⭐ (推荐)** RWKV-PEFT | [![Star](https://img.shields.io/github/stars/JL-er/RWKV-PEFT.svg?style=social&label=Star)](https://github.com/JL-er/RWKV-PEFT) | | RWKV 高效微调仓库，包含 LoRA、Pissa、DiSHA、State 等多种微调方法。 |
| RWKV-PEFT-Simple | [![Star](https://img.shields.io/github/stars/Seikaijyu/RWKV-PEFT-Simple.svg?style=social&label=Star)](https://github.com/Seikaijyu/RWKV-PEFT-Simple) | | RWKV-PEFT 的简化版本，提供便捷脚本和微调说明。 |
| RWKV-LM-RLHF | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-LM-RLHF.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-LM-RLHF) | | RWKV 强化学习（RLHF）工具包，含 SFT、对齐（DPO、ORPO）等。 |

### 训练项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| wind_rwkv | [![Star](https://img.shields.io/github/stars/johanwind/wind_rwkv.svg?style=social&label=Star)](https://github.com/johanwind/wind_rwkv) | | 一个包含 RWKV 语言模型优化内核的存储库。目前专注于 RWKV-7。 |
| RWKV-LM-V7 | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/RWKV-LM-V7.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/RWKV-LM-V7) | | RWKV-LM-V7 是一个专注于易用性的 RWKV-7 多类模型训练项目，让开发者能够在15分钟内快速上手 RWKV-7 模型训练。 |
| RWKV-LM-V7-AMD-ROCm | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV-LM-V7-AMD-ROCm.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV-LM-V7-AMD-ROCm) | | 适用于 AMD 的RWKV-LM-V7  |
| RWKV-infctx-trainer | [![Star](https://img.shields.io/github/stars/RWKV/RWKV-infctx-trainer.svg?style=social&label=Star)](https://github.com/RWKV/RWKV-infctx-trainer/) | | RWKV 无限上下文训练器，支持训练 10k 及以上长度的上下文。 |
| RWKV-Ouroboros | [![Star](https://img.shields.io/github/stars/neromous/RWKV-Ouroboros.svg?style=social&label=Star)](https://github.com/neromous/RWKV-Ouroboros) | | 基于 API 的 rwkv-trainer 项目，支持交替运行训练和推理。 |
| nanoRWKV | [![Star](https://img.shields.io/github/stars/Hannibal046/nanoRWKV.svg?style=social&label=Star)](https://github.com/Hannibal046/nanoRWKV) | | RWKV 模型的 nanoGPT 风格实现。 |
| RWKV_LM_EXT | [![Star](https://img.shields.io/github/stars/yynil/RWKV_LM_EXT.svg?style=social&label=Star)](https://github.com/yynil/RWKV_LM_EXT) | | 实现 RWKV 的功能扩展，包括序列分类/嵌入/peft/交叉编码器/双编码器/多模态等。 |
| chunkRWKV6 | [![Star](https://img.shields.io/github/stars/00ffcc/chunkRWKV6.svg?style=social&label=Star)](https://github.com/00ffcc/chunkRWKV6) | | 使用分块并行优化 RWKV 的 prefill 和训练速度。 |
| Mini_RWKV_7 | [![Star](https://img.shields.io/github/stars/Alic-Li/Mini_RWKV_7.svg?style=social&label=Star)](https://github.com/Alic-Li/Mini_RWKV_7) | | 轻量化 RWKV-V7 语言模型训练全流程 |

---

## 模型架构与优化

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|RWKVQuant|[![Star](https://img.shields.io/github/stars/xuchen-dev/RWKVQuant.svg?style=social&label=Star)](https://github.com/xuchen-dev/RWKVQuant)| [![arXiv:2505.03803](https://img.shields.io/badge/arXiv-2505.03803-b31b1b.svg)](https://arxiv.org/abs/2505.03803)| RWKV 系列模型高效量化|
|RWKV-X|[![Star](https://img.shields.io/github/stars/howard-hou/RWKV-X.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-X)|[![arXiv:2504.21463](https://img.shields.io/badge/arXiv-2504.21463-b31b1b.svg)](https://arxiv.org/abs/2504.21463)|基于RWKV架构的线性复杂度混合语言模|
|ARWKV|[![Star](https://img.shields.io/github/stars/yynil/RWKVInside.svg?style=social&label=Star)](https://github.com/yynil/RWKVInside)|[![arXiv:2501.15570](https://img.shields.io/badge/arXiv-2501.15570-b31b1b.svg)](https://arxiv.org/abs/2501.15570)|RWKV 混合注意力的语言模型|
|TemporalRNNs|[![Star](https://img.shields.io/github/stars/RazvanDu/TemporalRNNs.svg?style=social&label=Star)](https://github.com/RazvanDu/TemporalRNNs)|[![arXiv:2402.02625](https://img.shields.io/badge/arXiv-2402.02625-b31b1b.svg)](https://arxiv.org/abs/2402.02625)|【ICML 2024 workshop】多时间视角优化架构的方法|
|GoldFinch||[![arXiv:2407.12077](https://img.shields.io/badge/arXiv-2407.12077-b31b1b.svg)](https://arxiv.org/abs/2407.12077)|RWKV/Transformer 混合模型|
|RWKV-Lite||[![arXiv](https://img.shields.io/badge/arXiv-2412.10856-b31b1b)](https://arxiv.org/abs/2412.10856)|高效的 RWKV 模型深度压缩方案|
|RADLADS|[![Star](https://img.shields.io/github/stars/recursal/RADLADS-paper.svg?style=social&label=Star)](https://github.com/recursal/RADLADS-paper)|[![arXiv](https://img.shields.io/badge/arXiv-2505.03005-b31b1b)](https://arxiv.org/abs/2505.03005)|将 Transformer 架构模型高效转换为 RWKV 架构模型|
| RWKV-Depth-recurrence | [![Star](https://img.shields.io/github/stars/EricZhang1412/RWKV-Depth-recurrence.svg?style=social&label=Star)](https://github.com/EricZhang1412/RWKV-Depth-recurrence) | | 具有深度递归（跨层参数共享）的 RWKV 模型实现 |

## 自然语言处理

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|L3TC|[![Star](https://img.shields.io/github/stars/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression.svg?style=social&label=Star)](https://github.com/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression)|[![arXiv:2412.16642](https://img.shields.io/badge/arXiv-2412.16642-b31b1b.svg)](https://arxiv.org/abs/2412.16642)|高效的无损文本压缩|
|CMGN||[![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0925231225004837)|基于 RWKV 的假新闻检测|
|RCME||[![Paper](https://img.shields.io/badge/Paper-PDF-blue)](https://www.engineeringletters.com/issues_v33/issue_6/EL_33_6_28.pdf)|混合架构的知识图谱补全|
| TongShunLM | [![Star](https://img.shields.io/github/stars/ovo-Tim/TongShunLM.svg?style=social&label=Star)](https://github.com/ovo-Tim/TongShunLM) | | 基于 RWKV-7 的轻量化用词通顺度打分模型 |

## 多模态融合

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|ModRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2505.14505-b31b1b)](https://arxiv.org/abs/2505.14505)|基于 RWKV-7 的多模态融合框架|

---

## 图像与图形

### 视觉语言

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| VisualRWKV | [![Star](https://img.shields.io/github/stars/howard-hou/VisualRWKV.svg?style=social&label=Star)](https://github.com/howard-hou/VisualRWKV) | [![arXiv:2406.13362](https://img.shields.io/badge/arXiv-2406.13362-b31b1b.svg)](https://arxiv.org/abs/2406.13362)| 【COLING 2025】基于 RWKV 的视觉语言模型，可处理视觉任务。 |
| RWKV-CLIP | [![Star](https://img.shields.io/github/stars/deepglint/RWKV-CLIP.svg?style=social&label=Star)](https://github.com/deepglint/RWKV-CLIP) | [![arXiv:2406.06973](https://img.shields.io/badge/arXiv-2406.06973-b31b1b.svg)](https://arxiv.org/abs/2406.06973) | 【EMNLP 2024】RWKV 驱动的 CLIP（视觉-语言表示学习）模型。 |
|RWKV-UI||[![arXiv](https://img.shields.io/badge/arXiv-2502.03971-b31b1b)](https://arxiv.org/abs/2502.03971)|基于 RWKV 的视觉语言模型，专注于 UI 理解和设计|

### 视觉骨干网络

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Vision-RWKV (New Gen) | [![Star](https://img.shields.io/github/stars/xforcevesa/new-vrwkv.svg?style=social&label=Star)](https://github.com/xforcevesa/new-vrwkv) | | 全新一代 RWKV for Vision，基于 RWKV-7 实现。 |
| Vision-RWKV | [![Star](https://img.shields.io/github/stars/OpenGVLab/Vision-RWKV.svg?style=social&label=Star)](https://github.com/OpenGVLab/Vision-RWKV) | [![arXiv:2403.02308](https://img.shields.io/badge/arXiv-2403.02308-b31b1b.svg)](https://arxiv.org/abs/2403.02308)| 【ICLR 2025 Spotlight】基于 RWKV 的视觉感知模型，能平滑处理高分辨率图像。 |
| PointRWKV | [![Star](https://img.shields.io/github/stars/hithqd/PointRWKV.svg?style=social&label=Star)](https://github.com/hithqd/PointRWKV) |[![arXiv:2405.15214](https://img.shields.io/badge/arXiv-2405.15214-b31b1b.svg)](https://arxiv.org/abs/2405.15214) | 【AAAI 2025 】基于 RWKV 的 3D 点云学习框架。 |
|RSRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2503.20382-b31b1b)](https://arxiv.org/abs/2503.20382)|高分辨率遥感分析，适用于分类、目标检测、分割等多种任务|

### 图像分类

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|Vision_QRWKV|[![Star](https://img.shields.io/github/stars/ChiShengChen/Vision_QRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/Vision_QRWKV)|[![arXiv:2506.06633](https://img.shields.io/badge/arXiv-2506.06633-b31b1b.svg)](https://arxiv.org/abs/2506.06633)|用于图像分类的量子增强型 RWKV 模型|
| Hi-RWKV | [![Star](https://img.shields.io/github/stars/HSI-Lab/Hi-RWKV.svg?style=social&label=Star)](https://github.com/HSI-Lab/Hi-RWKV) | [![IEEE TIP 2026](https://img.shields.io/badge/IEEE%20TIP-2026-blue)](https://doi.org/10.1109/TIP.2025.3648554) | 【IEEE TIP 2026】分层 RWKV 高光谱图像分类模型 |

### 图像分割

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| U-RWKV | [![Star](https://img.shields.io/github/stars/hbyecoding/U-RWKV.svg?style=social&label=Star)](https://github.com/hbyecoding/U-RWKV) | [![arXiv:2507.11415](https://img.shields.io/badge/arXiv-2507.11415-b31b1b.svg)](https://arxiv.org/abs/2507.11415) | 基于 RWKV 的图像分割模型。 |
| RWKV-SAM | [![Star](https://img.shields.io/github/stars/HarborYuan/ovsam.svg?style=social&label=Star)](https://github.com/HarborYuan/ovsam) | [![arXiv:2406.19369](https://img.shields.io/badge/arXiv-2406.19369-b31b1b.svg)](https://arxiv.org/abs/2406.19369)| 基于 RWKV 的开放词表图像分段切割方法“RWKV-SAM”。 |
|MMSegRWKV|[![Star](https://img.shields.io/github/stars/supercyt/MMSegRWKV.svg?style=social&label=Star)](https://github.com/supercyt/MMSegRWKV)||基于 RWKV 架构开发的多模态磁共振成像（MRI）分割模型|
|BSBP-RWKV|| [![PDF](https://img.shields.io/badge/PDF-OpenReview-red)](https://openreview.net/pdf?id=ULD5RCk0oo)|RWKV 医学图像分割|
|RWKV-UNet||[![arXiv](https://img.shields.io/badge/arXiv-2501.08458-b31b1b)](https://arxiv.org/abs/2501.08458)|RWKV 改进的 Unet 进行医学图像分割|
|HFE-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888300)|【ICASSP 2025】RWKV 强化高频成分的医学图像分割|
|Zig-RiR||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/10969076)|【IEEE TMI】嵌套 RWKV 的医学图像分割|
|Diet-Seg||[![bioRxiv](https://img.shields.io/badge/bioRxiv-2025.05.31.657149-b31b1b.svg)](https://www.biorxiv.org/content/10.1101/2025.05.31.657149v1)|医学图像分割|
|Med-URWKV||[![arXiv:2506.10858](https://img.shields.io/badge/arXiv-2506.10858-b31b1b.svg)](https://arxiv.org/abs/2506.10858)|基于 ImageNet 预训练,用于医学图像分割的纯 RWKV|

### 图像生成

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Diffusion-RWKV | [![Star](https://img.shields.io/github/stars/feizc/Diffusion-RWKV.svg?style=social&label=Star)](https://github.com/feizc/Diffusion-RWKV) |[![arXiv:2404.04478](https://img.shields.io/badge/arXiv-2404.04478-b31b1b.svg)](https://arxiv.org/abs/2404.04478) | 基于 RWKV 的图像生成任务模型，擅长处理高分辨率图像。 |
|SDiT||[![arXiv:2402.11588](https://img.shields.io/badge/arXiv-2402.11588-b31b1b.svg)](https://arxiv.org/abs/2402.11588)|脉冲神经网络结合 RWKV 的图像生成|

### 目标检测

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| LION | [![Star](https://img.shields.io/github/stars/happinesslz/LION.svg?style=social&label=Star)](https://github.com/happinesslz/LION) | [![arXiv:2407.18232](https://img.shields.io/badge/arXiv-2407.18232-b31b1b.svg)](https://arxiv.org/abs/2407.18232)| 【NeurIPS 2024】用于点云中 3D 对象检测的 Linear Group RNN（支持 RWKV）。 |
|RWKV-VG| [![Star](https://img.shields.io/github/stars/nianfd/RWKV-VG.svg?style=social&label=Star)](https://github.com/nianfd/RWKV-VG)|[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00530-025-01720-w)|基于 RWKV 架构的视觉定位框架|
|Substation equipment||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11760-025-03852-y)|变电站缺陷检测|

### 超分辨率

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|OmniRWKVSR||[![arXiv](https://img.shields.io/badge/arXiv-2502.00404-b31b1b)](https://arxiv.org/abs/2502.00404)|【IJCNN】基于 RWKV 的单图超分|
|Geometry-Aware RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10943155)|异构光场超分辨率|
|Delta-WKV||[![arXiv](https://img.shields.io/badge/arXiv-2502.20852-b31b1b)](https://arxiv.org/abs/2502.20852)|【MICCAI 2025】磁共振成像超分模型|
|MSB-RWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s13042-025-02644-7)|红外图像超分辨率|

### 图像去噪/图像增强

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|CRWKV|[![Star](https://img.shields.io/github/stars/Seeker98/CRWKV.svg?style=social&label=Star)](https://github.com/Seeker98/CRWKV)|[![arXiv:2505.02705](https://img.shields.io/badge/arXiv-2505.02705-b31b1b.svg)](https://arxiv.org/abs/2505.02705)|【IJCAI 2025】引入双向 WKV 机制的高效图像去噪|
|RWKV-IR||[![arXiv:2412.03814](https://img.shields.io/badge/arXiv-2412.03814-b31b1b.svg)](https://arxiv.org/abs/2412.03814)|基于 RWKV 的图像恢复|
| Restore-RWKV | [![Star](https://img.shields.io/github/stars/Yaziwel/Restore-RWKV.svg?style=social&label=Star)](https://github.com/Yaziwel/Restore-RWKV) |[![arXiv:2407.11087](https://img.shields.io/badge/arXiv-2407.11087-b31b1b.svg)](https://arxiv.org/abs/2407.11087) | 使用 RWKV 进行高效且有效的医学图像恢复（PyTorch 实现）。 |
|SRCNet||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888780)|【ICASSP 2025】基于 RWKV 的水下图像增强|
|ID-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10889384)|【ICASSP 2025】基于 RWKV 的高效图像去雨|
|Flare-Aware RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888487)|【ICASSP 2025】基于 RWKV 的高效图像去光晕|
|URWKV||[![arXiv:2505.23068](https://img.shields.io/badge/arXiv-2505.23068-b31b1b.svg)](https://arxiv.org/abs/2505.23068)|【CVPR 2025】低光照图像恢复|
|Pan-Sharpening||[![IEEE](https://img.shields.io/badge/IEEE-11023855-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11023855)|【IEEE TGRS】基于 RWKV 的全色锐化|
|DiffRWKVIR||[![arXiv:2506.14541](https://img.shields.io/badge/arXiv-2506.14541-b31b1b.svg)](https://arxiv.org/abs/2506.14541)|结合 RWKV 和扩散模型的图像修复|
| RetinexRWKV | [![Star](https://img.shields.io/github/stars/Alic-Li/RetinexRWKV.svg?style=social&label=Star)](https://github.com/Alic-Li/RetinexRWKV) | | 基于 RWKV 的低光照图像增强模型 |
| DRWKV | [![Star](https://img.shields.io/github/stars/JackBaixue/DRWKV.svg?style=social&label=Star)](https://github.com/JackBaixue/DRWKV) | [![arXiv:2507.18594](https://img.shields.io/badge/arXiv-2507.18594-b31b1b.svg)](https://arxiv.org/abs/2507.18594) | 专注于物体边缘的低光照图像增强 |

### 其他图像任务

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|LALIC|[![Star](https://img.shields.io/github/stars/sjtu-medialab/RwkvCompress.svg?style=social&label=Star)](https://github.com/sjtu-medialab/RwkvCompress)|[![arXiv:2502.05741](https://img.shields.io/badge/arXiv-2502.05741-b31b1b.svg)](https://arxiv.org/abs/2502.05741)| 【CVPR 2025】基于 RWKV 的图像压缩框架|
| LineRWKV | [![Star](https://img.shields.io/github/stars/diegovalsesia/linerwkv.svg?style=social&label=Star)](https://github.com/diegovalsesia/linerwkv) | [![arXiv:2403.17677](https://img.shields.io/badge/arXiv-2403.17677-b31b1b.svg)](https://arxiv.org/abs/2403.17677)| LineRWKV 是一种对高光谱图像进行无损和有损压缩的方法。 |
|OpenPAR|[![Star](https://img.shields.io/github/stars/Event-AHU/OpenPAR.svg?style=social&label=Star)](https://github.com/Event-AHU/OpenPAR)| [![arXiv:2504.10018](https://img.shields.io/badge/arXiv-2504.10018-b31b1b.svg)](https://arxiv.org/abs/2504.10018)|开源的行人属性识别框架，包含 RWKV|
|PathRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2503.03199-b31b1b)](https://arxiv.org/abs/2503.03199)|全玻图像分析|
|RWKVMatch||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888484)|【ICASSP 2025】基于 vision-RWKV 的全局和交叉融合机制的医学图像配准|
|EVA||[![arXiv:2505.11165](https://img.shields.io/badge/arXiv-2505.11165-b31b1b.svg)](https://arxiv.org/abs/2505.11165)|基于 RWKV-6 构建异步编码器的事件相机异步检测|
|RWKV-DPA||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/10779439)|基于 RWKV 的高效深度估计|
| ChangeRWKV | [![Star](https://img.shields.io/github/stars/ChangeRWKV/ChangeRWKV.svg?style=social&label=Star)](https://github.com/ChangeRWKV/ChangeRWKV) | | 基于 RWKV 的线性时间复杂度变化检测方法 |

---

## 3D 与视频处理

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| FEAT | [![Star](https://img.shields.io/github/stars/Yaziwel/FEAT.svg?style=social&label=Star)](https://github.com/Yaziwel/FEAT) |[![arXiv:2506.04956](https://img.shields.io/badge/arXiv-2506.04956-b31b1b.svg)](https://arxiv.org/abs/2506.04956) | 【MICCAI 2025 early accepted】基于 RWKV 的医学视频生成。 |
|TLS-RWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11063-024-11540-0)|基于 RWKV 的在线动作检测（OAD）|
|Video RWKV||[![arXiv:2411.05636](https://img.shields.io/badge/arXiv-2411.05636-b31b1b.svg)](https://arxiv.org/abs/2411.05636)|基于 RWKV 的视频动作识别|
|TCVADS||[![arXiv:2412.20201](https://img.shields.io/badge/arXiv-2412.20201-b31b1b.svg)](https://arxiv.org/abs/2412.20201)|基于 RWKV 的视频异常检测|
|StyleRWKV||[![arXiv:2412.19535](https://img.shields.io/badge/arXiv-2412.19535-b31b1b.svg)](https://arxiv.org/abs/2412.19535)|基于类 RWKV 架构的高效视频风格迁移|
|RainRWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00371-025-03965-y)|基于 RWKV 的高效视频去雨|

---

## 音频相关

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|MIDI-RWKV|[![Star](https://img.shields.io/github/stars/christianazinn/MIDI-RWKV.svg?style=social&label=Star)](https://github.com/christianazinn/MIDI-RWKV)|[![arXiv:2506.13001](https://img.shields.io/badge/arXiv-2506.13001-b31b1b.svg)](https://arxiv.org/abs/2506.13001)|基于 RWKV 的音乐生成|
| RWKV-TTS | [![Star](https://img.shields.io/github/stars/yynil/RWKVTTS.svg?style=social&label=Star)](https://github.com/yynil/RWKVTTS) | [![arXiv:2504.03289](https://img.shields.io/badge/arXiv-2504.03289-b31b1b.svg)](https://arxiv.org/abs/2504.03289) | RWKV 语音合成模型，支持多种语言的文本转语音。 |
| RWKV-ASR | [![Star](https://img.shields.io/github/stars/AGENDD/RWKV-ASR.svg?style=social&label=Star)](https://github.com/AGENDD/RWKV-ASR) | | 使用预训练的 RWKV 语言模型进行**语音识别**。 |
|Rate-Aware||[![arXiv](https://img.shields.io/badge/arXiv-2501.11999-b31b1b)](https://arxiv.org/abs/2501.11999)|基于 RWKV 的语音压缩方案|
| Con-RWKV | [![Star](https://img.shields.io/github/stars/NYCU-MLLab/Con-RWKV.svg?style=social&label=Star)](https://github.com/NYCU-MLLab/Con-RWKV) | | 基于 RWKV 的语音识别模型 |
| AudioRWKV | [![Star](https://img.shields.io/github/stars/Jiayu-Xiong/AudioRWKV.svg?style=social&label=Star)](https://github.com/Jiayu-Xiong/AudioRWKV) | | 基于 RWKV 的音频处理模型 |

---

## 时间序列

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| BlackGoose_Rimer | [![Star](https://img.shields.io/github/stars/Alic-Li/BlackGoose_Rimer.svg?style=social&label=Star)](https://github.com/Alic-Li/BlackGoose_Rimer) |[![arXiv:2503.06121](https://img.shields.io/badge/arXiv-2503.06121-b31b1b.svg)](https://arxiv.org/abs/2503.06121) | 基于 RWKV-7 的时间序列预测模型，支持多种时间序列任务。 |
| RWKV-TS | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-TS.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-TS) | | 基于 RWKV 的时间序列任务模型，低延迟和内存占用。 |
|MSRWKV-2DTCN ||[![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0360544224028433)|多尺度 RWKV 的短期光伏发电功率预测|
|AutoGMM-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10729884)|基于 RWKV 的无线传感器网络选择性转发攻击检测方案|
|DFT||[![arXiv:2411.06065](https://img.shields.io/badge/arXiv-2411.06065-b31b1b.svg)](https://arxiv.org/abs/2411.06065)|基于 RWKV 的股票价格预测|
|MATCC||[![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3627673.3679715)|基于 RWKV 的股票价格预测|
|ET_MGNN||[![Paper](https://img.shields.io/badge/Paper-SSRN-orange)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5114041)|通过 RWKV 进行时序建模的脑科学诊断模型|
|TabulaTime||[![arXiv](https://img.shields.io/badge/arXiv-2502.17049-b31b1b)](https://arxiv.org/abs/2502.17049)|用于 ACS 预测的时序模型|
|LASTGCN||[![Scientific Reports](https://img.shields.io/badge/Scientific%20Reports-2025-green)](https://www.nature.com/articles/s41598-025-93179-y)|基于 RWKV 的时空多图交通流预测|
|DREMnet||[![arXiv](https://img.shields.io/badge/arXiv-2503.22223-b31b1b)](https://arxiv.org/abs/2503.22223)|电磁信号去噪|
|RWKV-TDR7||[![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.22544)|逆运动学的运动轨迹规划|
|MolRWKV||[![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.70100)|生物学条件分子生成|
|QuantumRWKV||[![arXiv](https://img.shields.io/badge/arXiv-2505.13524-b31b1b)](https://arxiv.org/abs/2505.13524)|基于 RWKV 的量子增强时序预测|
|STWGRL||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-11002535-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11002535)|【IEEE IoT-J】使用 RWKV 作为核心模块的时序异常检测|
|MP-RWKV||[![MDPI](https://img.shields.io/badge/MDPI-Article-green)](https://www.mdpi.com/2673-4591/97/1/26)|基于 RWKV 的长期电力符合预测|

---

## 机器人与具身智能

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| DecisionRWKV | [![Star](https://img.shields.io/github/stars/ancorasir/DecisionRWKV.svg?style=social&label=Star)](https://github.com/ancorasir/DecisionRWKV) | [![arXiv:2407.16306](https://img.shields.io/badge/arXiv-2407.16306-b31b1b.svg)](https://arxiv.org/abs/2407.16306)| 【JCISE】经验回放（experience replay）+ Decision-RWKV 模型，适合机器人的终身学习算法。 |
| OccRWKV | [![Star](https://img.shields.io/github/stars/jmwang0117/OccRWKV.svg?style=social&label=Star)](https://github.com/jmwang0117/OccRWKV) | [![arXiv:2409.19987](https://img.shields.io/badge/arXiv-2409.19987-b31b1b.svg)](https://arxiv.org/abs/2409.19987)| 【ICRA 2025】线性复杂度的高效 3D 语义占用预测。 |

---

## RWKV 分词器

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| rwkv-tokenizer | [![Star](https://img.shields.io/github/stars/cahya-wirawan/rwkv-tokenizer.svg?style=social&label=Star)](https://github.com/cahya-wirawan/rwkv-tokenizer) | | 用 Rust 编写的快速 RWKV Tokenizer，支持 RWKV-V5/6 World 模型。 |
| rwkv_tokenizer.c | [![Star](https://img.shields.io/github/stars/mrsteyk/rwkv_tokenizer.c.svg?style=social&label=Star)](https://github.com/mrsteyk/rwkv_tokenizer.c) | | C 语言编写的 RWKV Trie 分词器。 |
| rwkv-tokenizer-go | [![Star](https://img.shields.io/github/stars/Ronsor/rwkv-tokenizer-go.svg?style=social&label=Star)](https://github.com/Ronsor/rwkv-tokenizer-go) | | Go 语言的 RWKV 分词器。 |
| RWKV-World-Tokenizer-CPP | [![Star](https://img.shields.io/github/stars/m8than/RWKV-World-Tokenizer-CPP.svg?style=social&label=Star)](https://github.com/m8than/RWKV-World-Tokenizer-CPP) | | 用 C++ 编写的高度优化的 RWKV World 模型 trie 分词器。 |

---

## RWKV 的 RAG 系统

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| RWKV-RAG | [![Star](https://img.shields.io/github/stars/AIIRWKV/RWKV-RAG.svg?style=social&label=Star)](https://github.com/AIIRWKV/RWKV-RAG) | | 基于 RWKV 模型的一键 RAG 部署系统，可轻松搭建和管理本地知识库，同时提供了基于本地知识库的问答机器人和 RWKV 一键微调功能。 |

---

## 聊天机器人与推理 API 服务器

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| **⭐ (中文推荐)** RWKV Runner | [![Star](https://img.shields.io/github/stars/josStorer/RWKV-Runner.svg?style=social&label=Star)](https://github.com/josStorer/RWKV-Runner) | | RWKV Runner 是 RWKV 模型的管理和启动工具，带用户友好的 GUI 界面，支持训练和推理。 |
| **⭐ (中文推荐)** AI00 RWKV Server | [![Star](https://img.shields.io/github/stars/cgisky1980/ai00_rwkv_server.svg?style=social&label=Star)](https://github.com/cgisky1980/ai00_rwkv_server) | | Ai00 Server 是基于 web-rwkv 推理引擎的 RWKV 模型**推理 API 服务器**。 |
|RWKV_APP|[![Star](https://img.shields.io/github/stars/RWKV-APP/RWKV_APP.svg?style=social&label=Star)](https://github.com/RWKV-APP/RWKV_APP)||使用 flutter 实现的 RWKV-LM 端侧推理 App|
| **🇨🇳 (中文)** Role Play Chatbot | [![Star](https://img.shields.io/github/stars/shengxia/RWKV_Role_Playing.svg?style=social&label=Star)](https://github.com/shengxia/RWKV_Role_Playing) | | 基于 RWKV 的角色扮演 WebUI，使用 Gradio 制作。 |
| Easy_RWKV_webui | [![Star](https://img.shields.io/github/stars/No-22-Github/Easy_RWKV_webui.svg?style=social&label=Star)](https://github.com/No-22-Github/Easy_RWKV_webui) | | 基于 PyWebIO 的 RWKV 模型在线聊天室。 |
| Mini Model Daemon | [![Star](https://img.shields.io/github/stars/recursal/minmodmon.svg?style=social&label=Star)](https://github.com/recursal/minmodmon) | | 基于 web-rwkv 推理后端的 RWKV 模型推理工具。 |
| frank_esp32 | [![Star](https://img.shields.io/github/stars/lsk-china/frank_esp32.svg?style=social&label=Star)](https://github.com/lsk-china/frank_esp32) | | 基于 RWKV 的 Firefly 聊天机器人硬件实现 |

---

## RWKV 基准测试

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Uncheatable Eval | [![Star](https://img.shields.io/github/stars/Jellyfish042/uncheatable_eval.svg?style=social&label=Star)](https://github.com/Jellyfish042/uncheatable_eval) | | 使用最新的动态数据测试 LLM 性能，包含 RWKV。 |
| RULER_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/RULER_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/RULER_RWKV) | | RWKV 模型的 [RULER](https://arxiv.org/abs/2404.06654) 测试分数。 |
| LongBench_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/LongBench_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/LongBench_RWKV) | | RWKV 的 [LongBench](https://arxiv.org/abs/2308.14508) 测试分数。 |
| rwkv_mmlu | [![Star](https://img.shields.io/github/stars/Jellyfish042/rwkv_mmlu.svg?style=social&label=Star)](https://github.com/Jellyfish042/rwkv_mmlu) | | RWKV 模型的 MMLU 测试分数。 |

---

## RWKV 推理框架与算子库

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|rwkv_Ascend|[![Star](https://img.shields.io/github/stars/appleinsky/rwkv_Ascend.svg?style=social&label=Star)](https://github.com/appleinsky/rwkv_Ascend)||昇腾与rwkv共建的算子仓库|
| rwkv7.c | [![Star](https://img.shields.io/github/stars/KevlarKanou/rwkv7.c.svg?style=social&label=Star)](https://github.com/KevlarKanou/rwkv7.c) | | RWKV-7 的 C 语言实现，支持 RWKV-7 模型的推理。 |
| rwkv.cpp | [![Star](https://img.shields.io/github/stars/RWKV/rwkv.cpp.svg?style=social&label=Star)](https://github.com/RWKV/rwkv.cpp) | | 在 CPU 上推理 RWKV 模型，支持 FP16、量化 INT4、INT5 和 INT8 推理。 |
| RWKVSharp | [![Star](https://img.shields.io/github/stars/imxcstar/RWKVSharp.svg?style=social&label=Star)](https://github.com/imxcstar/RWKVSharp) | | 使用 C# 封装的 RWKV 推理工具，基于 rwkv.cpp，支持运行 RWKV4/RWKV5/RWKV6/RWKV7 World 模型。 |
| RWKV_Pytorch | [![Star](https://img.shields.io/github/stars/yuunnn-w/RWKV_Pytorch.svg?style=social&label=Star)](https://github.com/yuunnn-w/RWKV_Pytorch) | | 用纯 Pytorch 原生实现的 RWKV 模型推理框架。 |
| rwkv-kit | [![Star](https://img.shields.io/github/stars/TorchRWKV/rwkv-kit.svg?style=social&label=Star)](https://github.com/TorchRWKV/rwkv-kit) | | RWKV 模型推理框架，支持批量推理、并行推理训练等各种功能。 |
| web-rwkv | [![Star](https://img.shields.io/github/stars/cryscan/web-rwkv.svg?style=social&label=Star)](https://github.com/cryscan/web-rwkv) | | 在纯 WebGPU/Rust 中实现 RWKV 模型推理。 |
| candle-rwkv | [![Star](https://img.shields.io/github/stars/nkypy/candle-rwkv.svg?style=social&label=Star)](https://github.com/nkypy/candle-rwkv) | | 在 Rust 的极简机器学习框架 candle 中实现 RWKV 模型推理（支持量化）。 |
| **🚧 (施工中)** RWKV7-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV7-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV7-Keras) | | RWKV 模型的 Keras 实现，支持训练和推理。 |
| RWKV6-Keras | [![Star](https://img.shields.io/github/stars/pass-lin/RWKV6-Keras.svg?style=social&label=Star)](https://github.com/pass-lin/RWKV6-Keras) | | RWKV 模型的 Keras 实现，支持训练和推理。 |
| rwkv-burn| [![Star](https://img.shields.io/github/stars/dymat/rwkv-burn.svg?style=social&label=Star)](https://github.com/dymat/rwkv-burn) | | RWKV 语言模型的 burn 实现。 |
| jaxrwkv | [![Star](https://img.shields.io/github/stars/bsarkar321/jaxrwkv.svg?style=social&label=Star)](https://github.com/bsarkar321/jaxrwkv) | | RWKV 语言模型的 JAX 实现 |
| rwkv-mobile | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-mobile.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-mobile) | | RWKV 移动端推理引擎。 |
| rwkv-qualcomm | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-qualcomm.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-qualcomm) | | 使用 Qualcomm AI Engine Direct SDK 推理 RWKV 模型。 |
| rwkv-by-hand-excel | [![Star](https://img.shields.io/github/stars/playaswd/rwkv-by-hand-excel.svg?style=social&label=Star)](https://github.com/playaswd/rwkv-by-hand-excel) | | 使用 Excel 实现 RWKV，帮助开发者探索 RWKV 原理。 |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) | | 使用 FLA 进行 RWKV-V6/V7 推理，支持组合多个状态进行推理。 |
| RWKV-DeepEmbed-mmap | [![Star](https://img.shields.io/github/stars/Beortext/RWKV-DeepEmbed-mmap.svg?style=social&label=Star)](https://github.com/Beortext/RWKV-DeepEmbed-mmap) | | RWKV DeepEmbed mmap 高效推理方案 |
| rwkv-burn(Rust-RWKV) | [![Star](https://img.shields.io/github/stars/w1c2j3/rwkv-burn.svg?style=social&label=Star)](https://github.com/w1c2j3/rwkv-burn) | | Rust 实现的 RWKV 模型 |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) | | 大规模 RWKV v7 推理框架，支持多状态组合和动态切换 |

---

## 其他 RWKV 项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|SocialDeductionLLM|[![Star](https://img.shields.io/github/stars/SocialDeductionLLM/SocialDeductionLLM.svg?style=social&label=Star)](https://github.com/SocialDeductionLLM/SocialDeductionLLM)|[![arXiv:2502.06060](https://img.shields.io/badge/arXiv-2502.06060-b31b1b.svg)](https://arxiv.org/abs/2502.06060)|【AAMAS 2025】多智能体强化学习|
| SpikeGPT | [![Star](https://img.shields.io/github/stars/ridgerchu/SpikeGPT.svg?style=social&label=Star)](https://github.com/ridgerchu/SpikeGPT) | | 一款受 RWKV 启发的新模型。 |
| JSONL to binidx | [![Star](https://img.shields.io/github/stars/Abel2076/json2binidx_tool.svg?style=social&label=Star)](https://github.com/Abel2076/json2binidx_tool) | | 这个工具用于将 `.jsonl` 文件转成适合 RWKV 训练的 `.bin /.idx`（binidx）数据。 |
| AI Town - RWKV Proxy | [![Star](https://img.shields.io/github/stars/recursal/ai-town-rwkv-proxy.svg?style=social&label=Star)](https://github.com/recursal/ai-town-rwkv-proxy?tab=readme-ov-file) | | 通过 RWKV 在本地运营一个大型 AI 城镇！ |
| Bot-Ani-RWKV | [![Star](https://img.shields.io/github/stars/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection.svg?style=social&label=Star)](https://github.com/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection) | | 基于 RWKV 的推特水军机器人检测工具。|
| RWKV-IF | [![Star](https://img.shields.io/github/stars/Lyttr/RWKVInverseFolding.svg?style=social&label=Star)](https://github.com/Lyttr/RWKVInverseFolding) | [![bioRxiv](https://img.shields.io/badge/bioRxiv-green)](https://www.biorxiv.org/content/10.1101/2025.06.13.659654v1.full.pdf)| 基于RWKV的高效可控RNA逆折叠设计框架。|
| poker-ai-rwkv | [![Star](https://img.shields.io/github/stars/meraline/poker-ai-rwkv.svg?style=social&label=Star)](https://github.com/meraline/poker-ai-rwkv) | | 带有 RWKV 的AI 扑克牌游戏系统。|
|Muon-RMS-Norm|[![Star](https://img.shields.io/github/stars/xTimeCrystal/Muon-RMS-Norm.svg?style=social&label=Star)](https://github.com/xTimeCrystal/Muon-RMS-Norm)||一种新型归一化方法|
|PCF-RWKV||[![Paper](https://img.shields.io/badge/Paper-Preprint-yellow)](https://www.preprints.org/manuscript/202412.1705/v1)|基于 RWKV 模型的产品碳足迹估算系统|
|ChemRB||[![Paper](https://img.shields.io/badge/Paper-SNNU-orange)](https://jsnu.magtech.com.cn/CN/10.15983/j.cnki.jsnu.2025005)|医学分子生成|
|DualComp||[![arXiv:2505.16256](https://img.shields.io/badge/arXiv-2505.16256-b31b1b.svg)](https://arxiv.org/abs/2505.16256)|基于 RWKV-7 的无损数据压缩|
| Ai00 Character Maker | [![Star](https://img.shields.io/github/stars/Ai00-X/Ai00-character-maker.svg?style=social&label=Star)](https://github.com/Ai00-X/Ai00-character-maker) | | RWKV 角色扮演数据合成工具 |
| RWKV_7_on_AMD_Radeon-Instinct | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV_7_on_AMD_Radeon-Instinct.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV_7_on_AMD_Radeon-Instinct) | | RWKV-7 在 AMD Radeon & Instinct 显卡上的部署全流程 |
| RWKV-PEFT-GUI | [![Star](https://img.shields.io/github/stars/cttailearn/RWKV-PEFT-GUI.svg?style=social&label=Star)](https://github.com/cttailearn/RWKV-PEFT-GUI) | | 用于 RWKV 模型数据集处理的图形化界面工具 |
