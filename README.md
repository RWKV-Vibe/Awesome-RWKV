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
| stateswap | [![Star](https://img.shields.io/github/stars/Nice0o0/stateswap.svg?style=social&label=Star)](https://github.com/Nice0o0/stateswap) |  | 冻结 RWKV-7 模型权重，仅训练初始循环状态以保存人格或任务模式；提供状态热切换、混合、压缩和聊天界面。 |
| Preen | [![Star](https://img.shields.io/github/stars/No-22-Github/Preen.svg?style=social&label=Star)](https://github.com/No-22-Github/Preen) |  | 面向 Apple Silicon Mac 的 RWKV-7 状态微调工具，提供 SwiftUI 图形界面和命令行入口，可导入 JSONL 数据并导出可加载的初始状态文件。 |
| rwkvtune | [![Star](https://img.shields.io/github/stars/aierwiki/rwkvtune.svg?style=social&label=Star)](https://github.com/aierwiki/rwkvtune) |  | 面向 RWKV 的训练工具包，提供类似 Hugging Face TRL 的 Config、Trainer 与 Dataset 工作流，覆盖监督微调及偏好优化。 |

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
| RWKV-Megatron | [![Star](https://img.shields.io/github/stars/TimeMobius/RWKV-Megatron.svg?style=social&label=Star)](https://github.com/TimeMobius/RWKV-Megatron) |  | 基于 NVIDIA Megatron-Core 的 RWKV-6/RWKV-7 分布式训练框架，集成张量、流水线、序列和数据并行，提供混合精度训练与检查点转换。 |
| rwkv-metal | [![Star](https://img.shields.io/github/stars/RafaelUI/rwkv-metal.svg?style=social&label=Star)](https://github.com/RafaelUI/rwkv-metal) |  | 基于 MLX 与自定义 Metal WKV-7 算子的 Apple Silicon 训练框架，支持 RWKV-7 预训练、LoRA/QLoRA 微调、状态微调及推理。 |
| transformers-rwkv7 | [![Star](https://img.shields.io/github/stars/dfytensor/transformers-rwkv7.svg?style=social&label=Star)](https://github.com/dfytensor/transformers-rwkv7) |  | 自包含的 Hugging Face 兼容 RWKV-7 Goose 实现，以纯 PyTorch 接入 Trainer、PEFT 等训练工具，并提供循环状态推理路径。 |
---

## 模型架构与优化

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|RWKVQuant|[![Star](https://img.shields.io/github/stars/xuchen-dev/RWKVQuant.svg?style=social&label=Star)](https://github.com/xuchen-dev/RWKVQuant)| [![arXiv:2505.03803](https://img.shields.io/badge/arXiv-2505.03803-b31b1b.svg)](https://arxiv.org/abs/2505.03803)| RWKV 系列模型高效量化|
|RWKV-X|[![Star](https://img.shields.io/github/stars/howard-hou/RWKV-X.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-X)|[![arXiv:2504.21463](https://img.shields.io/badge/arXiv-2504.21463-b31b1b.svg)](https://arxiv.org/abs/2504.21463)|基于RWKV架构的线性复杂度混合语言模|
|ARWKV|[![Star](https://img.shields.io/github/stars/yynil/RWKVInside.svg?style=social&label=Star)](https://github.com/yynil/RWKVInside)|[![arXiv:2501.15570](https://img.shields.io/badge/arXiv-2501.15570-b31b1b.svg)](https://arxiv.org/abs/2501.15570)|RWKV 混合注意力的语言模型|
|TemporalRNNs|[![Star](https://img.shields.io/github/stars/RazvanDu/TemporalRNNs.svg?style=social&label=Star)](https://github.com/RazvanDu/TemporalRNNs)|[![arXiv:2402.02625](https://img.shields.io/badge/arXiv-2402.02625-b31b1b.svg)](https://arxiv.org/abs/2402.02625)|【ICML 2024 workshop】多时间视角优化架构的方法|
| GoldFinch | [![Star](https://img.shields.io/github/stars/recursal/GoldFinch-paper.svg?style=social&label=Star)](https://github.com/recursal/GoldFinch-paper) | [![arXiv:2407.12077](https://img.shields.io/badge/arXiv-2407.12077-b31b1b.svg)](https://arxiv.org/abs/2407.12077) | RWKV/Transformer 混合模型。 |
|RWKV-edge||[![arXiv](https://img.shields.io/badge/arXiv-2412.10856-b31b1b)](https://arxiv.org/abs/2412.10856)|高效的 RWKV 模型深度压缩方案|
|RADLADS|[![Star](https://img.shields.io/github/stars/recursal/RADLADS-paper.svg?style=social&label=Star)](https://github.com/recursal/RADLADS-paper)|[![arXiv](https://img.shields.io/badge/arXiv-2505.03005-b31b1b)](https://arxiv.org/abs/2505.03005)|将 Transformer 架构模型高效转换为 RWKV 架构模型|
| RWKV-Depth-recurrence | [![Star](https://img.shields.io/github/stars/EricZhang1412/RWKV-Depth-recurrence.svg?style=social&label=Star)](https://github.com/EricZhang1412/RWKV-Depth-recurrence) | | 具有深度递归（跨层参数共享）的 RWKV 模型实现 |
| ROSA-Soft | [![Star](https://img.shields.io/github/stars/wjie98/rosa_soft.svg?style=social&label=Star)](https://github.com/wjie98/rosa_soft) |  | ROSA 后缀检索算子的 PyTorch 扩展，提供 CUDA 精确匹配、用于训练的替代梯度，以及基于 C++ 后缀自动机的有状态 CPU 推理。 |
| ROSA-Tuning | [![Star](https://img.shields.io/github/stars/zyaaa-ux/ROSA-Tuning.svg?style=social&label=Star)](https://github.com/zyaaa-ux/ROSA-Tuning) | [![arXiv:2602.02499](https://img.shields.io/badge/arXiv-2602.02499-b31b1b.svg)](https://arxiv.org/abs/2602.02499) | 将 ROSA 后缀匹配记忆机制与窗口注意力语言模型结合，用于长上下文建模；提供训练实现和基于 Qwen3 的实验配置。 |
| B3D-RWKV | [![Star](https://img.shields.io/github/stars/leonardodalinky/B3D-RWKV.svg?style=social&label=Star)](https://github.com/leonardodalinky/B3D-RWKV) | [![arXiv:2605.25969](https://img.shields.io/badge/arXiv-2605.25969-b31b1b.svg)](https://arxiv.org/abs/2605.25969) | 基于 RWKV-7 的三元块离散扩散语言模型，通过掩码块与干净块组合训练实现文本填充，提供训练、推理和评估代码。 |

## 自然语言处理

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|L3TC|[![Star](https://img.shields.io/github/stars/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression.svg?style=social&label=Star)](https://github.com/alipay/L3TC-leveraging-rwkv-for-learned-lossless-low-complexity-text-compression)|[![arXiv:2412.16642](https://img.shields.io/badge/arXiv-2412.16642-b31b1b.svg)](https://arxiv.org/abs/2412.16642)|高效的无损文本压缩|
|CMGN||[![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0925231225004837)|基于 RWKV 的假新闻检测|
|RCME||[![Paper](https://img.shields.io/badge/Paper-PDF-blue)](https://www.engineeringletters.com/issues_v33/issue_6/EL_33_6_28.pdf)|混合架构的知识图谱补全|
| TongShunLM | [![Star](https://img.shields.io/github/stars/ovo-Tim/TongShunLM.svg?style=social&label=Star)](https://github.com/ovo-Tim/TongShunLM) | | 基于 RWKV-7 的轻量化用词通顺度打分模型 |
| rwkv-jev | [![Star](https://img.shields.io/github/stars/XingQiPan/rwkv-jev.svg?style=social&label=Star)](https://github.com/XingQiPan/rwkv-jev) |  | 基于 RWKV-7 的结构化决策服务，在固定候选标签集合上输出概率分布，兼容 TypeSafe 的 /v1/systemone 接口，适用于分类与受限决策。 |
| RWKV_document-term-translator | [![Star](https://img.shields.io/github/stars/LuckySongXiao/RWKV_document-term-translator.svg?style=social&label=Star)](https://github.com/LuckySongXiao/RWKV_document-term-translator) |  | 基于 C# WPF 的 Windows 文档术语翻译助手，支持 Word、Excel 文档和术语库管理，可接入 rwkv_lightning 或 llama.cpp 推理后端。 |
| rwkv-code-completion | [![Star](https://img.shields.io/github/stars/xun082/rwkv-code-completion.svg?style=social&label=Star)](https://github.com/xun082/rwkv-code-completion) |  | 基于 RWKV 的 VS Code 代码补全扩展，支持实时补全、多候选展示和中间填充（FIM），需连接自建 RWKV 推理后端。 |

## 多模态融合

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| ModRWKV | [![Star](https://img.shields.io/github/stars/Joluck/mod-rwkv.svg?style=social&label=Star)](https://github.com/Joluck/mod-rwkv) | [![arXiv:2505.14505](https://img.shields.io/badge/arXiv-2505.14505-b31b1b.svg)](https://arxiv.org/abs/2505.14505) | 基于 RWKV-7 的多模态融合框架。 |

---

## 图像与图形

### 视觉语言

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| VisualRWKV | [![Star](https://img.shields.io/github/stars/howard-hou/VisualRWKV.svg?style=social&label=Star)](https://github.com/howard-hou/VisualRWKV) | [![arXiv:2406.13362](https://img.shields.io/badge/arXiv-2406.13362-b31b1b.svg)](https://arxiv.org/abs/2406.13362)| 【COLING 2025】基于 RWKV 的视觉语言模型，可处理视觉任务。 |
| RWKV-CLIP | [![Star](https://img.shields.io/github/stars/deepglint/RWKV-CLIP.svg?style=social&label=Star)](https://github.com/deepglint/RWKV-CLIP) | [![arXiv:2406.06973](https://img.shields.io/badge/arXiv-2406.06973-b31b1b.svg)](https://arxiv.org/abs/2406.06973) | 【EMNLP 2024】RWKV 驱动的 CLIP（视觉-语言表示学习）模型。 |
|RWKV-UI||[![arXiv](https://img.shields.io/badge/arXiv-2502.03971-b31b1b)](https://arxiv.org/abs/2502.03971)|基于 RWKV 的视觉语言模型，专注于 UI 理解和设计|
| PestVL-Net |  | [![CVPR 2026 Findings](https://img.shields.io/badge/CVPR-2026%20Findings-blue)](https://openaccess.thecvf.com/content/CVPR2026F/html/Li_PestVL-Net_Enabling_Multimodal_Pest_Learning_Via_Fine-grained_Vision-Language_Interaction_CVPRF_2026_paper.html) | 【CVPR 2026 Findings】面向害虫细粒度识别的视觉语言框架，视觉分支以 RWKV 结合显著性引导的自适应窗口划分，语言端用 MLLM 融合农业专家知识与多模态思维链生成描述。 |
| MCUVLM-RWKV |  | [![Paper](https://img.shields.io/badge/Paper-NSTL-orange)](https://opaj.napstic.cn/periodicalArticle/0120260300988014) | 面向 STM32 微控制器的轻量化视觉语言模型，由轻量视觉编码器、特征映射器与 RWKV 解码器组成，在单片机资源约束下完成图像描述。 |

### 视觉骨干网络

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Vision-RWKV (New Gen) | [![Star](https://img.shields.io/github/stars/xforcevesa/new-vrwkv.svg?style=social&label=Star)](https://github.com/xforcevesa/new-vrwkv) | | 全新一代 RWKV for Vision，基于 RWKV-7 实现。 |
| Vision-RWKV | [![Star](https://img.shields.io/github/stars/OpenGVLab/Vision-RWKV.svg?style=social&label=Star)](https://github.com/OpenGVLab/Vision-RWKV) | [![arXiv:2403.02308](https://img.shields.io/badge/arXiv-2403.02308-b31b1b.svg)](https://arxiv.org/abs/2403.02308)| 【ICLR 2025 Spotlight】基于 RWKV 的视觉感知模型，能平滑处理高分辨率图像。 |
| PointRWKV | [![Star](https://img.shields.io/github/stars/hithqd/PointRWKV.svg?style=social&label=Star)](https://github.com/hithqd/PointRWKV) |[![arXiv:2405.15214](https://img.shields.io/badge/arXiv-2405.15214-b31b1b.svg)](https://arxiv.org/abs/2405.15214) | 【AAAI 2025 】基于 RWKV 的 3D 点云学习框架。 |
| RSRWKV | [![Star](https://img.shields.io/github/stars/Ling-yunchi/RSRWKV.svg?style=social&label=Star)](https://github.com/Ling-yunchi/RSRWKV) | [![arXiv:2503.20382](https://img.shields.io/badge/arXiv-2503.20382-b31b1b.svg)](https://arxiv.org/abs/2503.20382) | 高分辨率遥感分析框架，适用于分类、目标检测、分割等任务。 |
### 图像分类

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|Vision_QRWKV|[![Star](https://img.shields.io/github/stars/ChiShengChen/Vision_QRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/Vision_QRWKV)|[![arXiv:2506.06633](https://img.shields.io/badge/arXiv-2506.06633-b31b1b.svg)](https://arxiv.org/abs/2506.06633)|用于图像分类的量子增强型 RWKV 模型|
| Hi-RWKV（将在论文被接收后开源） | [![Star](https://img.shields.io/github/stars/HSI-Lab/Hi-RWKV.svg?style=social&label=Star)](https://github.com/HSI-Lab/Hi-RWKV) | | 分层 RWKV 高光谱图像分类模型 |

### 图像分割

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| U-RWKV | [![Star](https://img.shields.io/github/stars/hbyecoding/U-RWKV.svg?style=social&label=Star)](https://github.com/hbyecoding/U-RWKV) | [![arXiv:2507.11415](https://img.shields.io/badge/arXiv-2507.11415-b31b1b.svg)](https://arxiv.org/abs/2507.11415) | 基于 RWKV 的图像分割模型。 |
| RWKV-SAM | [![Star](https://img.shields.io/github/stars/HarborYuan/ovsam.svg?style=social&label=Star)](https://github.com/HarborYuan/ovsam) | [![arXiv:2406.19369](https://img.shields.io/badge/arXiv-2406.19369-b31b1b.svg)](https://arxiv.org/abs/2406.19369)| 基于 RWKV 的开放词表图像分段切割方法“RWKV-SAM”。 |
|MMSegRWKV|[![Star](https://img.shields.io/github/stars/supercyt/MMSegRWKV.svg?style=social&label=Star)](https://github.com/supercyt/MMSegRWKV)||基于 RWKV 架构开发的多模态磁共振成像（MRI）分割模型|
|BSBP-RWKV|| [![PDF](https://img.shields.io/badge/PDF-OpenReview-red)](https://openreview.net/pdf?id=ULD5RCk0oo)|RWKV 医学图像分割|
| RWKV-UNet | [![Star](https://img.shields.io/github/stars/juntaoJianggavin/RWKV-UNet.svg?style=social&label=Star)](https://github.com/juntaoJianggavin/RWKV-UNet) | [![arXiv:2501.08458](https://img.shields.io/badge/arXiv-2501.08458-b31b1b.svg)](https://arxiv.org/abs/2501.08458) | 融合 RWKV 长程依赖建模的 U-Net 医学图像分割模型。 |
| HFE-RWKV | [![Star](https://img.shields.io/github/stars/yezizi1022/HFE-RWKV.svg?style=social&label=Star)](https://github.com/yezizi1022/HFE-RWKV) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://doi.org/10.1109/ICASSP49660.2025.10888300) | 【ICASSP 2025】基于 RWKV 的层次特征增强医学图像分割模型 |
| Zig-RiR | [![Star](https://img.shields.io/github/stars/txchen-USTC/Zig-RiR.svg?style=social&label=Star)](https://github.com/txchen-USTC/Zig-RiR) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://doi.org/10.1109/TMI.2025.3561797) | 基于 RWKV 的 Zigzag 扫描与反向残差医学图像分割模型 |
|Diet-Seg||[![bioRxiv](https://img.shields.io/badge/bioRxiv-2025.05.31.657149-b31b1b.svg)](https://www.biorxiv.org/content/10.1101/2025.05.31.657149v1)|医学图像分割|
|Med-URWKV||[![arXiv:2506.10858](https://img.shields.io/badge/arXiv-2506.10858-b31b1b.svg)](https://arxiv.org/abs/2506.10858)|基于 ImageNet 预训练,用于医学图像分割的纯 RWKV|
| SCRWKV | [![Star](https://img.shields.io/github/stars/zhxhzy/SCRWKV.svg?style=social&label=Star)](https://github.com/zhxhzy/SCRWKV) | [![arXiv:2605.14926](https://img.shields.io/badge/arXiv-2605.14926-b31b1b.svg)](https://arxiv.org/abs/2605.14926) | 用于裂缝分割的结构校准 Vision-RWKV 网络，结合多尺度纹理建模与轻量解码器，提供训练、测试和评估代码。 |
| SRWKV | [![Star](https://img.shields.io/github/stars/ukeLin/SRWKV.svg?style=social&label=Star)](https://github.com/ukeLin/SRWKV) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/11676832) | 【IEEE TNNLS】形状引导的 RWKV 医学图像分割网络，用形状先验引导序列遍历并以自适应位移调整感受野；官方实现含训练、测试脚本与权重下载说明。 |
| RWKVFUSE | [![Star](https://img.shields.io/github/stars/alqurri/rwkv.svg?style=social&label=Star)](https://github.com/alqurri/rwkv) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/11515577) | 【ISBI 2026】VRWKV 与 CNN 的并行双编码器医学图像分割网络，融合局部空间特征与长程依赖；仓库提供 Synapse/ACDC 的训练与测试脚本。 |
| FreRWKV-Net | [![Star](https://img.shields.io/github/stars/Stu-Ziyang-Zhang/FreRWKV-Net.svg?style=social&label=Star)](https://github.com/Stu-Ziyang-Zhang/FreRWKV-Net) | [![Springer](https://img.shields.io/badge/Springer-Article-red)](https://doi.org/10.1007/978-981-92-3495-0_14) | 视网膜血管分割的频域引导网络，由血管差分注意力 VDAM、频域方向预测驱动的 FGD-RWKV 与多尺度频空交叉注意力 MS-FSCA 组成；仓库提供模型与训练/测试代码，未附权重。 |
| MD-RWKV-UNET | [作者仓库](https://github.com/fzy-eng/MD-RWKV-UNET)（无 README） | [![arXiv:2603.27261](https://img.shields.io/badge/arXiv-2603.27261-b31b1b.svg)](https://arxiv.org/abs/2603.27261) | 面向多器官分割的 RWKV-UNet 变体，引入尺度感知解剖编码与跨阶段融合；作者仓库仅有一次文件上传，无复现说明。 |
| SegRWKV | [![Star](https://img.shields.io/github/stars/luminescentfrr/SegRWKV.svg?style=social&label=Star)](https://github.com/luminescentfrr/SegRWKV) | [![JCDE 2026](https://img.shields.io/badge/Oxford-JCDE%202026-blue)](https://doi.org/10.1093/jcde/qwag065) | 【JCDE】以 URWKV 为骨干、沿用 nnU-Net 流程的生物医学分割框架，覆盖腹部 MR、内窥镜与显微三类任务；仓库含预处理、训练与评估脚本。 |
| RWKVSegDiT | [![Star](https://img.shields.io/github/stars/alqurri/RWKVSegDiT.svg?style=social&label=Star)](https://github.com/alqurri/RWKVSegDiT) |  | 以层级 RWKV 为骨干、将分割建模为图像条件掩码扩散的医学分割实现，仓库含 ISIC 数据准备、训练、采样与评估脚本。 |
| CropRWKV | [![Star](https://img.shields.io/github/stars/Shutong-Hou/CropRWKV.svg?style=social&label=Star)](https://github.com/Shutong-Hou/CropRWKV) |  | 面向作物叶片病斑表型分析的线性复杂度 RWKV 分割研究，含统一训练协议、多种子基准、混合精度训练失败诊断与全部源数据表；稿件已投 *Plants*。 |


### 图像生成

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Diffusion-RWKV | [![Star](https://img.shields.io/github/stars/feizc/Diffusion-RWKV.svg?style=social&label=Star)](https://github.com/feizc/Diffusion-RWKV) |[![arXiv:2404.04478](https://img.shields.io/badge/arXiv-2404.04478-b31b1b.svg)](https://arxiv.org/abs/2404.04478) | 基于 RWKV 的图像生成任务模型，擅长处理高分辨率图像。 |

### 目标检测

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| LION | [![Star](https://img.shields.io/github/stars/happinesslz/LION.svg?style=social&label=Star)](https://github.com/happinesslz/LION) | [![arXiv:2407.18232](https://img.shields.io/badge/arXiv-2407.18232-b31b1b.svg)](https://arxiv.org/abs/2407.18232)| 【NeurIPS 2024】用于点云中 3D 对象检测的 Linear Group RNN（支持 RWKV）。 |
|RWKV-VG| [![Star](https://img.shields.io/github/stars/nianfd/RWKV-VG.svg?style=social&label=Star)](https://github.com/nianfd/RWKV-VG)|[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00530-025-01720-w)|基于 RWKV 架构的视觉定位框架|
|Substation equipment||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11760-025-03852-y)|变电站缺陷检测|
| Titanium-Strip-Defect |  | [![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0952197626003799) | 面向钛带表面缺陷检测的 RWKV 启发上下文建模与层级差分融合方法，以线性复杂度上下文模块替代自注意力完成工业质检识别。 |

### 超分辨率

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| OmniRWKVSR | [![Star](https://img.shields.io/github/stars/question110/omnirwkvsr.svg?style=social&label=Star)](https://github.com/question110/omnirwkvsr) | [![arXiv:2502.00404](https://img.shields.io/badge/arXiv-2502.00404-b31b1b.svg)](https://arxiv.org/abs/2502.00404) | 基于 RWKV 的单图像超分辨率模型|
| Geometry-Aware RWKV | [![Star](https://img.shields.io/github/stars/chenzean/LF-RWKVNet.svg?style=social&label=Star)](https://github.com/chenzean/LF-RWKVNet) | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://doi.org/10.1109/LSP.2025.3555445) | 基于 RWKV 的几何感知光场图像超分辨率模型 |
|Delta-WKV||[![arXiv](https://img.shields.io/badge/arXiv-2502.20852-b31b1b)](https://arxiv.org/abs/2502.20852)|【MICCAI 2025】磁共振成像超分模型|
|MSB-RWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s13042-025-02644-7)|红外图像超分辨率|

### 图像去噪/图像增强

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|CRWKV|[![Star](https://img.shields.io/github/stars/Seeker98/CRWKV.svg?style=social&label=Star)](https://github.com/Seeker98/CRWKV)|[![arXiv:2505.02705](https://img.shields.io/badge/arXiv-2505.02705-b31b1b.svg)](https://arxiv.org/abs/2505.02705)|【IJCAI 2025】引入双向 WKV 机制的高效图像去噪|
| RWKV-IR | [![Star](https://img.shields.io/github/stars/YuzhenD/Resyn.svg?style=social&label=Star)](https://github.com/YuzhenD/Resyn) | [![arXiv:2412.03814](https://img.shields.io/badge/arXiv-2412.03814-b31b1b.svg)](https://arxiv.org/abs/2412.03814) | 基于 RWKV 的图像恢复方法 |
| Restore-RWKV | [![Star](https://img.shields.io/github/stars/Yaziwel/Restore-RWKV.svg?style=social&label=Star)](https://github.com/Yaziwel/Restore-RWKV) |[![arXiv:2407.11087](https://img.shields.io/badge/arXiv-2407.11087-b31b1b.svg)](https://arxiv.org/abs/2407.11087) | 使用 RWKV 进行高效且有效的医学图像恢复（PyTorch 实现）。 |
|SRCNet||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888780)|【ICASSP 2025】基于 RWKV 的水下图像增强|
|ID-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10889384)|【ICASSP 2025】基于 RWKV 的高效图像去雨|
|Flare-Aware RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888487)|【ICASSP 2025】基于 RWKV 的高效图像去光晕|
| URWKV | [![Star](https://img.shields.io/github/stars/FZU-N/URWKV.svg?style=social&label=Star)](https://github.com/FZU-N/URWKV) | [![arXiv:2505.23068](https://img.shields.io/badge/arXiv-2505.23068-b31b1b.svg)](https://arxiv.org/abs/2505.23068) | 【CVPR 2025】基于多状态建模的统一 RWKV 低光照图像恢复模型。 |
|Pan-Sharpening||[![IEEE](https://img.shields.io/badge/IEEE-11023855-blue.svg)](https://ieeexplore.ieee.org/abstract/document/11023855)|【IEEE TGRS】基于 RWKV 的全色锐化|
| RetinexRWKV | [![Star](https://img.shields.io/github/stars/Alic-Li/RetinexRWKV.svg?style=social&label=Star)](https://github.com/Alic-Li/RetinexRWKV) | | 基于 RWKV 的低光照图像增强模型 |
| DRWKV | [![Star](https://img.shields.io/github/stars/JackBaixue/DRWKV.svg?style=social&label=Star)](https://github.com/JackBaixue/DRWKV) | [![arXiv:2507.18594](https://img.shields.io/badge/arXiv-2507.18594-b31b1b.svg)](https://arxiv.org/abs/2507.18594) | 专注于物体边缘的低光照图像增强 |
| Fourier-RWKV | [![Star](https://img.shields.io/github/stars/Dilizlr/Fourier-RWKV.svg?style=social&label=Star)](https://github.com/Dilizlr/Fourier-RWKV) | [![arXiv:2512.08161](https://img.shields.io/badge/arXiv-2512.08161-b31b1b.svg)](https://arxiv.org/abs/2512.08161) | 面向图像去雾的多状态感知网络，将 WKV 建模扩展到频域，并结合可变形四向位移与语义桥接模块；提供训练/测试代码与权重下载。 |
| CLUIE | [![Star](https://img.shields.io/github/stars/geekpool/CLUIE.svg?style=social&label=Star)](https://github.com/geekpool/CLUIE) | [![arXiv:2607.21467](https://img.shields.io/badge/arXiv-2607.21467-b31b1b.svg)](https://arxiv.org/abs/2607.21467) | 【IEEE TIP】面向水下图像增强的聚类感知 RWKV 框架，通过语义动态重排构造内容自适应递归轨迹，并以暗响应调制补偿局部结构；提供 PyTorch 实现。 |
| EvRWKV | [![Star](https://img.shields.io/github/stars/Echo0517/EvRWKV.svg?style=social&label=Star)](https://github.com/Echo0517/EvRWKV) | [![arXiv:2507.03184](https://img.shields.io/badge/arXiv-2507.03184-b31b1b.svg)](https://arxiv.org/abs/2507.03184) | 事件引导的低光图像增强框架，通过 Cross-RWKV 与频谱融合模块持续交互事件流与图像特征；官方实现已开源。 |

### 其他图像任务

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|LALIC|[![Star](https://img.shields.io/github/stars/sjtu-medialab/RwkvCompress.svg?style=social&label=Star)](https://github.com/sjtu-medialab/RwkvCompress)|[![arXiv:2502.05741](https://img.shields.io/badge/arXiv-2502.05741-b31b1b.svg)](https://arxiv.org/abs/2502.05741)| 【CVPR 2025】基于 RWKV 的图像压缩框架|
| LineRWKV | [![Star](https://img.shields.io/github/stars/diegovalsesia/linerwkv.svg?style=social&label=Star)](https://github.com/diegovalsesia/linerwkv) | [![arXiv:2403.17677](https://img.shields.io/badge/arXiv-2403.17677-b31b1b.svg)](https://arxiv.org/abs/2403.17677)| LineRWKV 是一种对高光谱图像进行无损和有损压缩的方法。 |
|OpenPAR|[![Star](https://img.shields.io/github/stars/Event-AHU/OpenPAR.svg?style=social&label=Star)](https://github.com/Event-AHU/OpenPAR)| [![arXiv:2504.10018](https://img.shields.io/badge/arXiv-2504.10018-b31b1b.svg)](https://arxiv.org/abs/2504.10018)|开源的行人属性识别框架，包含 RWKV|
| PathRWKV | [![Star](https://img.shields.io/github/stars/Puzzle-Logic/PathRWKV.svg?style=social&label=Star)](https://github.com/Puzzle-Logic/PathRWKV) | [![arXiv:2503.03199](https://img.shields.io/badge/arXiv-2503.03199-b31b1b.svg)](https://arxiv.org/abs/2503.03199) | 基于 RWKV 的病理全切片图像分析模型。 |
|RWKVMatch||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10888484)|【ICASSP 2025】基于 vision-RWKV 的全局和交叉融合机制的医学图像配准|
| EVA | [![Star](https://img.shields.io/github/stars/haohq19/eva.svg?style=social&label=Star)](https://github.com/haohq19/eva) | [![arXiv:2505.11165](https://img.shields.io/badge/arXiv-2505.11165-b31b1b.svg)](https://arxiv.org/abs/2505.11165) | 基于 RWKV-6 异步编码器的事件视觉框架，支持事件相机数据的识别与检测。 |
| ChangeRWKV | [![Star](https://img.shields.io/github/stars/ChangeRWKV/ChangeRWKV.svg?style=social&label=Star)](https://github.com/ChangeRWKV/ChangeRWKV) | [![AAAI 2026](https://img.shields.io/badge/AAAI-2026-blue)](https://ojs.aaai.org/index.php/AAAI/article/view/38167) | 【AAAI 2026】基于 RWKV 的线性时间复杂度变化检测方法。 |
| RWKV-CD |  | [![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/document/11456675) | 面向遥感建筑物变化检测的 Vision-RWKV 框架，通过双分支编码、特征融合与噪声抑制处理双时相影像。 |
| MRT | [![Star](https://img.shields.io/github/stars/luke1453lh/MRT.svg?style=social&label=Star)](https://github.com/luke1453lh/MRT) | [![AAAI 2026](https://img.shields.io/badge/AAAI-2026-blue)](https://doi.org/10.1609/aaai.v40i9.37650) | 【AAAI 2026】极低码率图像压缩模型，窗口内用 Transformer 局部注意力、跨窗口用双向 RWKV 建模，配合 RWKV 压缩模型与生成式解码器；提供完整训练、编解码与评测脚本。 |
---

## 3D 与视频处理

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| FEAT | [![Star](https://img.shields.io/github/stars/Yaziwel/FEAT.svg?style=social&label=Star)](https://github.com/Yaziwel/FEAT) |[![arXiv:2506.04956](https://img.shields.io/badge/arXiv-2506.04956-b31b1b.svg)](https://arxiv.org/abs/2506.04956) | 【MICCAI 2025 early accepted】基于 RWKV 的医学视频生成。 |
|TLS-RWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s11063-024-11540-0)|基于 RWKV 的在线动作检测（OAD）|
|Video RWKV||[![arXiv:2411.05636](https://img.shields.io/badge/arXiv-2411.05636-b31b1b.svg)](https://arxiv.org/abs/2411.05636)|基于 RWKV 的视频动作识别|
|StyleRWKV||[![arXiv:2412.19535](https://img.shields.io/badge/arXiv-2412.19535-b31b1b.svg)](https://arxiv.org/abs/2412.19535)|基于类 RWKV 架构的高效视频风格迁移|
|RainRWKV||[![Springer](https://img.shields.io/badge/Springer-Article-red)](https://link.springer.com/article/10.1007/s00371-025-03965-y)|基于 RWKV 的高效视频去雨|
| RWKV3D |  | [![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3746027.3755658) | 【ACM MM 2025】面向点云分析的 RWKV 模型，结合局部特征混合与双向多头位移，支持从零训练及单模态、跨模态预训练。 |
| RWKV-PCSSC | [![Star](https://img.shields.io/github/stars/shuaiqianende/RWKVPCSSC.svg?style=social&label=Star)](https://github.com/shuaiqianende/RWKVPCSSC) | [![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3746027.3754908) | 【ACM MM 2025】点云语义场景补全网络，用 RWKV 种子生成器与逐级点反卷积恢复场景，参数量较 PointSSC 降低约 4.18 倍；官方仓库已开源。 |
| PointDGRWKV |  | [![arXiv:2508.20835](https://img.shields.io/badge/arXiv-2508.20835-b31b1b.svg)](https://arxiv.org/abs/2508.20835) | 面向未见域点云分类的 RWKV 框架，结合几何感知位移与跨域特征对齐；作者仓库已建但代码尚未发布。 |
| P-RWKV / PointER |  | [![arXiv:2606.10395](https://img.shields.io/badge/arXiv-2606.10395-b31b1b.svg)](https://arxiv.org/abs/2606.10395) | 面向点云的 P-RWKV 模块及自监督表征学习框架 PointER，通过局部感知扩展与空间上下文增强建模非规则三维几何；论文声明接收后开源。 |
| Otter |  | [![AAAI 2026](https://img.shields.io/badge/AAAI-2026-blue)](https://ojs.aaai.org/index.php/AAAI/article/view/37428) | 【AAAI 2026 Oral】面向广角少样本动作识别的增强 RWKV 模型，通过主体强调与时序重建抑制背景干扰。 |
| MG-RWKV |  | [![arXiv:2607.00902](https://img.shields.io/badge/arXiv-2607.00902-b31b1b.svg)](https://arxiv.org/abs/2607.00902) | 【ECCV 2026】音视频时序伪造定位的多粒度 RWKV 框架，结合双向 RWKV、多粒度专家路由与跨粒度一致性约束，在 O(T) 复杂度下定位篡改片段。 |
| VRWKV-Editor | [![Star](https://img.shields.io/github/stars/abdo-RG/VRWKV-Editor.svg?style=social&label=Star)](https://github.com/abdo-RG/VRWKV-Editor) | [![Springer](https://img.shields.io/badge/Springer-Multimedia%20Systems-red)](https://doi.org/10.1007/s00530-026-02649-4) | 【Multimedia Systems 2026】把扩散视频编辑中的二次时空注意力替换为线性 3D-VRWKV（双向 Bi-WKV）聚合，在 Tune-A-Video 流程上完成对象替换、背景修改与风格变换；提供训练与编辑代码。 |
---

## 音频相关

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|MIDI-RWKV|[![Star](https://img.shields.io/github/stars/christianazinn/MIDI-RWKV.svg?style=social&label=Star)](https://github.com/christianazinn/MIDI-RWKV)|[![arXiv:2506.13001](https://img.shields.io/badge/arXiv-2506.13001-b31b1b.svg)](https://arxiv.org/abs/2506.13001)|基于 RWKV 的音乐生成|
| RWKV-TTS | [![Star](https://img.shields.io/github/stars/yynil/RWKVTTS.svg?style=social&label=Star)](https://github.com/yynil/RWKVTTS) | [![arXiv:2504.03289](https://img.shields.io/badge/arXiv-2504.03289-b31b1b.svg)](https://arxiv.org/abs/2504.03289) | RWKV 语音合成模型，支持多种语言的文本转语音。 |
| RWKV-ASR | [![Star](https://img.shields.io/github/stars/AGENDD/RWKV-ASR.svg?style=social&label=Star)](https://github.com/AGENDD/RWKV-ASR) | | 使用预训练的 RWKV 语言模型进行**语音识别**。 |
|Rate-Aware||[![arXiv](https://img.shields.io/badge/arXiv-2501.11999-b31b1b)](https://arxiv.org/abs/2501.11999)|基于 RWKV 的语音压缩方案|
| Con-RWKV | [![Star](https://img.shields.io/github/stars/NYCU-MLLab/Con-RWKV.svg?style=social&label=Star)](https://github.com/NYCU-MLLab/Con-RWKV) | | 基于 RWKV 的语音识别模型 |
| AudioRWKV | [![Star](https://img.shields.io/github/stars/Jiayu-Xiong/AudioRWKV.svg?style=social&label=Star)](https://github.com/Jiayu-Xiong/AudioRWKV) | [![arXiv:2509.02167](https://img.shields.io/badge/arXiv-2509.02167-b31b1b.svg)](https://arxiv.org/abs/2509.02167) | 基于 RWKV-7 的双向音频模式识别模型。 |

---

## 时间序列

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| BlackGoose_Rimer | [![Star](https://img.shields.io/github/stars/Alic-Li/BlackGoose_Rimer.svg?style=social&label=Star)](https://github.com/Alic-Li/BlackGoose_Rimer) |[![arXiv:2503.06121](https://img.shields.io/badge/arXiv-2503.06121-b31b1b.svg)](https://arxiv.org/abs/2503.06121) | 基于 RWKV-7 的时间序列预测模型，支持多种时间序列任务。 |
| RWKV-TS | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-TS.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-TS) | [![arXiv:2401.09093](https://img.shields.io/badge/arXiv-2401.09093-b31b1b.svg)](https://arxiv.org/abs/2401.09093) | 基于 RWKV 的时间序列模型，支持预测、分类、异常检测及缺失值填补等任务。 |
|MSRWKV-2DTCN ||[![ScienceDirect](https://img.shields.io/badge/ScienceDirect-Article-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0360544224028433)|多尺度 RWKV 的短期光伏发电功率预测|
|AutoGMM-RWKV||[![IEEE Xplore](https://img.shields.io/badge/IEEE%20Xplore-Abstract-orange)](https://ieeexplore.ieee.org/abstract/document/10729884)|基于 RWKV 的无线传感器网络选择性转发攻击检测方案|
| DFT | [![Star](https://img.shields.io/github/stars/cq-dong/DFT_25.svg?style=social&label=Star)](https://github.com/cq-dong/DFT_25) | [![arXiv:2411.06065](https://img.shields.io/badge/arXiv-2411.06065-b31b1b.svg)](https://arxiv.org/abs/2411.06065) | 基于 RWKV 的股票价格预测方法|
| MATCC | [![Star](https://img.shields.io/github/stars/dyccolin/MATCC.svg?style=social&label=Star)](https://github.com/dyccolin/MATCC) | [![ACM DL](https://img.shields.io/badge/ACM-Paper-red)](https://dl.acm.org/doi/abs/10.1145/3627673.3679715) | 融合市场趋势与跨时间相关性、使用 RWKV 建模的股票价格预测框架。 |
| ET_MGNN | [![Star](https://img.shields.io/github/stars/BrainFC/ET_MGNN.svg?style=social&label=Star)](https://github.com/BrainFC/ET_MGNN) | [![Paper](https://img.shields.io/badge/Paper-SSRN-orange)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5114041) | 使用 RWKV 进行时序建模的多模态动态脑图表示学习模型，用于脑疾病诊断。 |
|TabulaTime||[![arXiv](https://img.shields.io/badge/arXiv-2502.17049-b31b1b)](https://arxiv.org/abs/2502.17049)|用于 ACS 预测的时序模型|
|LASTGCN||[![Scientific Reports](https://img.shields.io/badge/Scientific%20Reports-2025-green)](https://www.nature.com/articles/s41598-025-93179-y)|基于 RWKV 的时空多图交通流预测|
|DREMnet||[![arXiv](https://img.shields.io/badge/arXiv-2503.22223-b31b1b)](https://arxiv.org/abs/2503.22223)|电磁信号去噪|
|RWKV-TDR7||[![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.22544)|逆运动学的运动轨迹规划|
| MolRWKV | [![Star](https://img.shields.io/github/stars/bigwestHan/MolRWKV.svg?style=social&label=Star)](https://github.com/bigwestHan/MolRWKV) | [![Wiley](https://img.shields.io/badge/Wiley-Online%20Library-red)](https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.70100) | 结合局部增强与图增强的 RWKV 条件分子生成模型。 |
| QuantumRWKV | [![Star](https://img.shields.io/github/stars/ChiShengChen/QuantumRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/QuantumRWKV) | [![arXiv:2505.13524](https://img.shields.io/badge/arXiv-2505.13524-b31b1b.svg)](https://arxiv.org/abs/2505.13524) | 通过量子增强通道混合实现时间序列预测的 RWKV 模型。 |
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
| RWKV_APP |[![Star](https://img.shields.io/github/stars/RWKV-APP/RWKV_APP.svg?style=social&label=Star)](https://github.com/RWKV-APP/RWKV_APP)||使用 flutter 实现的 RWKV-LM 端侧推理 App|
| **🇨🇳 (中文)** Role Play Chatbot | [![Star](https://img.shields.io/github/stars/shengxia/RWKV_Role_Playing.svg?style=social&label=Star)](https://github.com/shengxia/RWKV_Role_Playing) | | 基于 RWKV 的角色扮演 WebUI，使用 Gradio 制作。 |
| Easy_RWKV_webui | [![Star](https://img.shields.io/github/stars/No-22-Github/Easy_RWKV_webui.svg?style=social&label=Star)](https://github.com/No-22-Github/Easy_RWKV_webui) | | 基于 PyWebIO 的 RWKV 模型在线聊天室。 |
| Mini Model Daemon | [![Star](https://img.shields.io/github/stars/recursal/minmodmon.svg?style=social&label=Star)](https://github.com/recursal/minmodmon) | | 基于 web-rwkv 推理后端的 RWKV 模型推理工具。 |
| frank_esp32 | [![Star](https://img.shields.io/github/stars/lsk-china/frank_esp32.svg?style=social&label=Star)](https://github.com/lsk-china/frank_esp32) | | 基于 RWKV 的 Firefly 聊天机器人硬件实现 |
| RWKV State Agent | [![Star](https://img.shields.io/github/stars/123123213weqw/rwkv-agent.svg?style=social&label=Star)](https://github.com/123123213weqw/rwkv-agent) |  | 以 RWKV 循环状态为核心的本地 Agent 运行时，支持跨轮状态复用、结构化工具调用和多任务状态隔离，提供联网检索、命令与文件工具。 |
| rwkv_lightning | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/rwkv_lightning.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/rwkv_lightning) |  | 基于 Albatross 与 FastAPI 的 RWKV 批量推理后端，提供 NVIDIA CUDA 和 AMD ROCm 路径，并支持量化推理与服务接口。 |
| RWKV-Server | [![Star](https://img.shields.io/github/stars/AUXStar/RWKV-Server.svg?style=social&label=Star)](https://github.com/AUXStar/RWKV-Server) |  | 面向并发请求的 RWKV 批量推理服务器，提供 OpenAI 兼容 API、SSE 流式输出、循环状态复用与动态批处理调度。 |
| RWKV-Router | [![Star](https://img.shields.io/github/stars/cgisky1980/rwkv-router.svg?style=social&label=Star)](https://github.com/cgisky1980/rwkv-router) |  | 基于规则与小型 RWKV 分类器的请求路由网关，将请求分级并分配给本地模型或云端 API，提供 OpenAI、Anthropic 兼容接口与多语言绑定。 |
| RWKV-Scout | [![Star](https://img.shields.io/github/stars/rwkv-rs/RWKV-Scout.svg?style=social&label=Star)](https://github.com/rwkv-rs/RWKV-Scout) |  | 以 RWKV 为决策核心的联网检索 Agent，涵盖任务拆解、查询与工具选择、证据审核及回答生成，并记录证据与执行轨迹。 |
| rwkv_lightning_cuda | [![Star](https://img.shields.io/github/stars/Alic-Li/rwkv_lightning_cuda.svg?style=social&label=Star)](https://github.com/Alic-Li/rwkv_lightning_cuda) |  | 面向 NVIDIA CUDA、附带 AMD HIP 路径的 RWKV-7 推理服务，提供 OpenAI 兼容与原生批量 API、流式输出、状态缓存、状态微调和量化功能。 |
| RWKV-LH | [![Star](https://img.shields.io/github/stars/rwkv-rs/RWKV-LH.svg?style=social&label=Star)](https://github.com/rwkv-rs/RWKV-LH) |  | 面向 RWKV 状态续写模型的实验性编码 Agent，结合决策模型、执行模型和按需调用的规划模型，提供工具执行、完成条件校验与中断恢复。 |
| RWKV_Role_Playing_with_GPT-SoVITS | [![Star](https://img.shields.io/github/stars/v3ucn/RWKV_Role_Playing_with_GPT-SoVITS.svg?style=social&label=Star)](https://github.com/v3ucn/RWKV_Role_Playing_with_GPT-SoVITS) |  | 在 RWKV 角色扮演 WebUI 基础上接入 GPT-SoVITS 语音对话，支持角色配置与本地运行；适合单用户体验。 |
| RWKV-Agent | [![Star](https://img.shields.io/github/stars/No-22-Github/RWKV-Agent.svg?style=social&label=Star)](https://github.com/No-22-Github/RWKV-Agent) |  | 面向 Apple Silicon 的本地优先 RWKV 工作区 Agent，使用 Go 与 MLX 推理，提供命令行、终端界面、桌面与浏览器入口；当前工具能力以只读操作为主。 |
---

## RWKV 基准测试

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Uncheatable Eval | [![Star](https://img.shields.io/github/stars/Jellyfish042/uncheatable_eval.svg?style=social&label=Star)](https://github.com/Jellyfish042/uncheatable_eval) | [![arXiv:2609.27510](https://img.shields.io/badge/arXiv-2609.27510-b31b1b.svg)](https://arxiv.org/abs/2609.27510) | 使用持续更新的新文本和无损压缩率评估语言模型能力，覆盖 RWKV 等模型。 |
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
| jaxrwkv | [![Star](https://img.shields.io/github/stars/bsarkar321/jaxrwkv.svg?style=social&label=Star)](https://github.com/bsarkar321/jaxrwkv) | | RWKV 语言模型的 JAX 实现 |
| rwkv-mobile | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-mobile.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-mobile) | | RWKV 移动端推理引擎。 |
| rwkv-qualcomm | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-qualcomm.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-qualcomm) | | 使用 Qualcomm AI Engine Direct SDK 推理 RWKV 模型。 |
| rwkv-by-hand-excel | [![Star](https://img.shields.io/github/stars/playaswd/rwkv-by-hand-excel.svg?style=social&label=Star)](https://github.com/playaswd/rwkv-by-hand-excel) | | 使用 Excel 实现 RWKV，帮助开发者探索 RWKV 原理。 |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) | | 使用 FLA 进行 RWKV-V6/V7 推理，支持组合多个状态进行推理。 |
| RWKV-DeepEmbed-mmap | [![Star](https://img.shields.io/github/stars/Beortext/RWKV-DeepEmbed-mmap.svg?style=social&label=Star)](https://github.com/Beortext/RWKV-DeepEmbed-mmap) | | RWKV DeepEmbed mmap 高效推理方案 |
| rwkv-burn(Rust-RWKV) | [![Star](https://img.shields.io/github/stars/w1c2j3/rwkv-burn.svg?style=social&label=Star)](https://github.com/w1c2j3/rwkv-burn) | | Rust 实现的 RWKV 模型 |
| wkvm | [![Star](https://img.shields.io/github/stars/xiaol/wkvm.svg?style=social&label=Star)](https://github.com/xiaol/wkvm) |  | 面向 RWKV-7、GDN、Mamba2 等线性及混合模型的状态推理框架，以固定大小的状态槽管理请求，并提供状态快照、分叉、休眠与恢复能力。 |
| RWKV-7 Hugging Face Reference | [![Star](https://img.shields.io/github/stars/rwkv-rs/hf-adapter.svg?style=social&label=Star)](https://github.com/rwkv-rs/hf-adapter) |  | 面向 Hugging Face Transformers 的纯 PyTorch RWKV-7 参考实现，分离模型配置、循环缓存与算子，提供权重转换工具及可选的 NVIDIA 加速算子接口。 |
| FlashRWKV2 | [![Star](https://img.shields.io/github/stars/rwkv-rs/FlashRWKV2.svg?style=social&label=Star)](https://github.com/rwkv-rs/FlashRWKV2) |  | 基于 TileLang 的 RWKV-7 GPU 算子库，提供训练与推理共用的 BF16 前向路径、FP32 累加与循环状态，以及面向推理的融合算子接口。 |
| RWKV-MUSA | [![Star](https://img.shields.io/github/stars/KakaruHayate/RWKV-MUSA.svg?style=social&label=Star)](https://github.com/KakaruHayate/RWKV-MUSA) |  | 面向摩尔线程 GPU 的 RWKV-7 循环算子与模型集成，提供可选 torch_musa 后端、Hugging Face 适配和 PyTorch 参考计算路径。 |
| rwkv-hf-kernels | [![Star](https://img.shields.io/github/stars/Hakureirm/rwkv-hf-kernels.svg?style=social&label=Star)](https://github.com/Hakureirm/rwkv-hf-kernels) |  | 为 Hugging Face Transformers 的 RWKV-7 模型提供可选融合 CUDA 算子，以可移植的 PyTorch 实现作为参考路径。 |
| rwkv-quant | [![Star](https://img.shields.io/github/stars/RafaelUI/rwkv-quant.svg?style=social&label=Star)](https://github.com/RafaelUI/rwkv-quant) |  | 面向 Apple Silicon 的 RWKV-7 量化工具包与 Metal 推理后端，提供可移植的 .rwkvq 检查点格式、校准和直接读取量化权重的 GPU 算子。 |
| RWKV-7 Quantization Toolkit | [![Star](https://img.shields.io/github/stars/AUXStar/rwkv7-quantization.svg?style=social&label=Star)](https://github.com/AUXStar/rwkv7-quantization) |  | RWKV-7 量化与推理工具包，支持 FP8、INT8、INT4 等方案，并提供模型信息查看、量化前后比较及评估命令。 |
| rwkv-rsv | [![Star](https://img.shields.io/github/stars/cgisky1980/rwkv-rsv.svg?style=social&label=Star)](https://github.com/cgisky1980/rwkv-rsv) |  | 使用 Rust 与 Vulkan/CUDA 计算着色器实现的 RWKV-7 推理引擎，支持 FP16、INT8 权重路径，并提供 CPU FP32 参考实现用于精度对照。 |
| dspark-rwkv | [![Star](https://img.shields.io/github/stars/cgisky1980/dspark-rwkv.svg?style=social&label=Star)](https://github.com/cgisky1980/dspark-rwkv) |  | 将 DSpark 半自回归推测解码适配到 RWKV-7 的实验项目，提供训练、解码及评测实现；仓库已撤回早期加速与接受率结果，使用时需参照其勘误。 |
| rwkv_mobile_flutter | [![Star](https://img.shields.io/github/stars/RWKV-APP/rwkv_mobile_flutter.svg?style=social&label=Star)](https://github.com/RWKV-APP/rwkv_mobile_flutter) |  | 连接 Flutter/Dart 应用与原生 rwkv-mobile 推理引擎的 FFI 插件和运行时编排层，用于设备端 RWKV、语音及多模态功能集成。 |
| VKWR | [![Star](https://img.shields.io/github/stars/szxysdt/VKWR.svg?style=social&label=Star)](https://github.com/szxysdt/VKWR) |  | 带优化 CUDA 算子与连续批处理的 RWKV 推理引擎，提供命令行启动方式和 OpenAI 兼容 API 服务；项目仍在开发中。 |
| rosalia | [![Star](https://img.shields.io/github/stars/cryscan/rosalia.svg?style=social&label=Star)](https://github.com/cryscan/rosalia) |  | 使用 Rust 与 Vulkan 计算着色器实现的 RWKV 推理引擎，探索在独立运行时中实现 Rosa 机制。 |
| RWKV-7 × sglang | [![Star](https://img.shields.io/github/stars/Hakureirm/rwkv-sglang.svg?style=social&label=Star)](https://github.com/Hakureirm/rwkv-sglang) |  | 将 RWKV-7 接入 SGLang 的推理服务实现，支持循环状态推理、INT8/INT4 量化及 OpenAI 兼容服务，并提供基准与参考实现对照记录。 |
| vllm-rwkv | [![Star](https://img.shields.io/github/stars/123123213weqw/vllm-rwkv.svg?style=social&label=Star)](https://github.com/123123213weqw/vllm-rwkv) |  | 集成原生 RWKV-7 循环状态调度与 Albatross 派生 CUDA 算子的 vLLM 发行版，提供动态状态管理、批处理和 OpenAI 兼容服务。 |
| HTMLNLM | [![Star](https://img.shields.io/github/stars/ConsciousNode/HTMLNLM.svg?style=social&label=Star)](https://github.com/ConsciousNode/HTMLNLM) |  | 单文件浏览器端神经语言模型运行时，基于 RWKV-v7 架构，在网页中提供模型训练与推理，无需独立服务器或 Python 环境。 |

---

## 其他 RWKV 项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|SocialDeductionLLM|[![Star](https://img.shields.io/github/stars/SocialDeductionLLM/SocialDeductionLLM.svg?style=social&label=Star)](https://github.com/SocialDeductionLLM/SocialDeductionLLM)|[![arXiv:2502.06060](https://img.shields.io/badge/arXiv-2502.06060-b31b1b.svg)](https://arxiv.org/abs/2502.06060)|【AAMAS 2025】多智能体强化学习|
| SpikeGPT | [![Star](https://img.shields.io/github/stars/ridgerchu/SpikeGPT.svg?style=social&label=Star)](https://github.com/ridgerchu/SpikeGPT) | [![arXiv:2302.13939](https://img.shields.io/badge/arXiv-2302.13939-b31b1b.svg)](https://arxiv.org/abs/2302.13939) | 【TMLR】受 RWKV 启发的脉冲神经网络生成式语言模型。 |
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
| RWKV-DPA | | [论文](https://ieeexplore.ieee.org/document/10779439) | 面向车联网（V2X）通信的线性注意力信道估计方法。 |
| RWKV_7_on_AMD_Radeon-Instinct | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV_7_on_AMD_Radeon-Instinct.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV_7_on_AMD_Radeon-Instinct) | | RWKV-7 在 AMD Radeon & Instinct 显卡上的部署全流程 |
| RWKV-PEFT-GUI | [![Star](https://img.shields.io/github/stars/cttailearn/RWKV-PEFT-GUI.svg?style=social&label=Star)](https://github.com/cttailearn/RWKV-PEFT-GUI) | | 用于 RWKV 模型数据集处理的图形化界面工具 |
| RWKV-nonogram | [![Star](https://img.shields.io/github/stars/LeC-Z/RWKV-nonogram.svg?style=social&label=Star)](https://github.com/LeC-Z/RWKV-nonogram) |  | 使用约 20M 参数的 RWKV-6 模型求解数织谜题的实验项目，提供演示与 Colab 体验入口。 |
| Sudoku-RWKV | [![Star](https://img.shields.io/github/stars/Jellyfish042/Sudoku-RWKV.svg?style=social&label=Star)](https://github.com/Jellyfish042/Sudoku-RWKV) |  | 基于 RWKV-6 的数独求解模型，提供交互演示、最小推理示例与训练数据生成脚本。 |
| RWKV-15Puzzle | [![Star](https://img.shields.io/github/stars/Jellyfish042/RWKV-15Puzzle.svg?style=social&label=Star)](https://github.com/Jellyfish042/RWKV-15Puzzle) |  | 面向 15 拼图问题的 RWKV-6 专用模型，提供图形演示、最小推理入口和训练配置说明。 |
