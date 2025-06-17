# RWKV 生态项目一览

一份精选的 RWKV 生态系统中的优秀项目、工具和资源的列表。

## 目录

- [RWKV 官方链接](#rwkv-官方链接)
- [RWKV 微调与训练](#rwkv-微调与训练)
  - [微调项目](#微调项目)
  - [训练项目](#训练项目)
- [图像与图形](#图像与图形)
  - [视觉语言](#视觉语言)
  - [视觉骨干网络](#视觉骨干网络)
  - [图像分割](#图像分割)
  - [图像生成](#图像生成)
  - [目标检测](#目标检测)
  - [其他图像任务](#其他图像任务)
- [音频相关](#音频相关)
- [时间序列](#时间序列)
- [机器人与具身智能](#机器人与具身智能)
- [RWKV 分词器](#rwkv-分词器)
- [RWKV 的 RAG 系统](#rwkv-rag)
- [聊天机器人与推理 API 服务器](#聊天机器人与推理-api-服务器)
- [RWKV 基准测试](#rwkv-基准测试)
- [RWKV 推理框架/算子库](#rwkv-推理框架算子库)
- [其他 RWKV 项目](#其他-rwkv-项目)

---

## RWKV 官方链接

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| RWKV-LM | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM) | | RWKV 的官方代码仓库，提供了 RWKV v1 至 v7 各版本的架构代码，以及配套的大语言模型训练实现。 |
| RWKV-4 架构论文 | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v4) | [![arXiv:2305.13048](https://img.shields.io/badge/arXiv-2305.13048-b31b1b.svg)](https://arxiv.org/abs/2305.13048) | RWKV-4 的架构论文。 |
| RWKV 5/6 架构论文 | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v5) | [![arXiv:2404.05892](https://img.shields.io/badge/arXiv-2404.05892-b31b1b.svg)](https://arxiv.org/abs/2404.05892) | RWKV-5/6 的架构论文。 |
| RWKV-7 架构论文 | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-LM.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-LM/tree/main/RWKV-v7)| [![arXiv:2503.14456](https://img.shields.io/badge/arXiv-2503.14456-b31b1b.svg)](https://arxiv.org/abs/2503.14456) | RWKV-7 的架构论文。 |
| RWKV pip 包 | [![PyPI - Downloads](https://img.shields.io/pypi/dm/rwkv.svg)](https://pypi.org/project/rwkv/) | | RWKV 的 pip 包，具体用法可以查看 [RWKV 官网](https://rwkv.cn/tutorials/intermediate/RWKVpip)。 |
| RWKV-CUDA | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV-CUDA.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV-CUDA) | | RWKV 的官方 CUDA 算子。 |
| Hugging Face 文档 | [![Hugging Face Docs](https://img.shields.io/badge/Hugging%20Face-Docs-blue)](https://huggingface.co/docs/transformers/model_doc/rwkv) | | Hugging Face 关于 RWKV 的介绍。 |
| rwkvcn-docs | [![Star](https://img.shields.io/github/stars/LeoLin4258/rwkvcn-docs.svg?style=social&label=Star)](https://github.com/LeoLin4258/rwkvcn-docs) | | RWKV 的中文文档项目链接 |
| RWKV.com | [![Star](https://img.shields.io/github/stars/BlinkDL/RWKV.com.svg?style=social&label=Star)](https://github.com/BlinkDL/RWKV.com) | | RWKV 的英文官网项目链接 |

---

## RWKV 微调与训练

### 微调项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| **⭐ (推荐)** RWKV-PEFT | [![Star](https://img.shields.io/github/stars/JL-er/RWKV-PEFT.svg?style=social&label=Star)](https://github.com/JL-er/RWKV-PEFT) | | RWKV 高效微调仓库，包含 LoRA、Pissa、Lisa、State 等多种微调方法。 |
| RWKV-PEFT-Simple | [![Star](https://img.shields.io/github/stars/Seikaijyu/RWKV-PEFT-Simple.svg?style=social&label=Star)](https://github.com/Seikaijyu/RWKV-PEFT-Simple) | | RWKV-PEFT 的简化版本，提供便捷脚本和微调说明。 |
| **🚧 (开发中)** RWKV-LM-RLHF | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-LM-RLHF.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-LM-RLHF) | | RWKV 强化学习（RLHF）工具包，含 SFT、对齐（DPO、ORPO）等。 |
| RWKV-LM-RLHF-DPO | [![Star](https://img.shields.io/github/stars/Triang-jyed-driung/RWKV-LM-RLHF-DPO.svg?style=social&label=Star)](https://github.com/Triang-jyed-driung/RWKV-LM-RLHF-DPO) | | RWKV 的 DPO 实现（直接偏好优化 - Direct Preference Optimization）。 |
| **⚠️ (可能过时)** RWKV-LoRA | [![Star](https://img.shields.io/github/stars/Blealtan/RWKV-LM-LoRA.svg?style=social&label=Star)](https://github.com/Blealtan/RWKV-LM-LoRA) | | RWKV LoRA 微调实现，不支持微调 RWKV-6 或更新的版本。 |

### 训练项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| wind_rwkv | [![Star](https://img.shields.io/github/stars/johanwind/wind_rwkv.svg?style=social&label=Star)](https://github.com/johanwind/wind_rwkv) | | 一个包含 RWKV 语言模型优化内核的存储库。目前专注于 RWKV-7。 |
| RWKV-LM-V7 | [![Star](https://img.shields.io/github/stars/RWKV-Vibe/RWKV-LM-V7.svg?style=social&label=Star)](https://github.com/RWKV-Vibe/RWKV-LM-V7) | | RWKV-LM-V7 是一个专注于易用性的 RWKV-7 多类模型训练项目，让开发者能够在15分钟内快速上手 RWKV-7 模型训练。 |
| RWKV-LM-V7-AMD-ROCm | [![Star](https://img.shields.io/github/stars/Alic-Li/RWKV-LM-V7-AMD-ROCm.svg?style=social&label=Star)](https://github.com/Alic-Li/RWKV-LM-V7-AMD-ROCm7) | | 适用于 AMD 的RWKV-LM-V7  |
| RWKV-infctx-trainer | [![Star](https://img.shields.io/github/stars/RWKV/RWKV-infctx-trainer.svg?style=social&label=Star)](https://github.com/RWKV/RWKV-infctx-trainer/) | | RWKV 无限上下文训练器，支持训练 10k 及以上长度的上下文。 |
| RWKV-Ouroboros | [![Star](https://img.shields.io/github/stars/neromous/RWKV-Ouroboros.svg?style=social&label=Star)](https://github.com/neromous/RWKV-Ouroboros) | | 基于 API 的 rwkv-trainer 项目，支持交替运行训练和推理。 |
| nanoRWKV | [![Star](https://img.shields.io/github/stars/Hannibal046/nanoRWKV.svg?style=social&label=Star)](https://github.com/Hannibal046/nanoRWKV) | | RWKV 模型的 nanoGPT 风格实现。 |
| RWKV_LM_EXT | [![Star](https://img.shields.io/github/stars/yynil/RWKV_LM_EXT.svg?style=social&label=Star)](https://github.com/yynil/RWKV_LM_EXT) | | 实现 RWKV 的功能扩展，包括序列分类/嵌入/peft/交叉编码器/双编码器/多模态等。 |
| chunkRWKV6 | [![Star](https://img.shields.io/github/stars/00ffcc/chunkRWKV6.svg?style=social&label=Star)](https://github.com/00ffcc/chunkRWKV6) | | 使用分块并行优化 RWKV 的 prefill 和训练速度。 |

---

## 图像与图形

### 视觉语言

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| VisualRWKV | [![Star](https://img.shields.io/github/stars/howard-hou/VisualRWKV.svg?style=social&label=Star)](https://github.com/howard-hou/VisualRWKV) | | 基于 RWKV 的视觉语言模型，可处理视觉任务。 |
| RWKV-CLIP | [![Star](https://img.shields.io/github/stars/deepglint/RWKV-CLIP.svg?style=social&label=Star)](https://github.com/deepglint/RWKV-CLIP) | [![arXiv:2406.06973](https://img.shields.io/badge/arXiv-2406.06973-b31b1b.svg)](https://arxiv.org/abs/2406.06973) | 🏅【EMNLP 2024】RWKV 驱动的 CLIP（视觉-语言表示学习）模型。 |

### 图像分类

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|Vision_QRWKV|[![Star](https://img.shields.io/github/stars/ChiShengChen/Vision_QRWKV.svg?style=social&label=Star)](https://github.com/ChiShengChen/Vision_QRWKV)|[![arXiv:2506.06633](https://img.shields.io/badge/arXiv-2506.06633-b31b1b.svg)](https://arxiv.org/abs/2506.06633)|用于图像分类的量子增强型 RWKV 模型|

### 视觉骨干网络

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Vision-RWKV (New Gen) | [![Star](https://img.shields.io/github/stars/xforcevesa/new-vrwkv.svg?style=social&label=Star)](https://github.com/xforcevesa/new-vrwkv) | | 全新一代 RWKV for Vision，基于 RWKV-7 实现。 |
| Vision-RWKV | [![Star](https://img.shields.io/github/stars/OpenGVLab/Vision-RWKV.svg?style=social&label=Star)](https://github.com/OpenGVLab/Vision-RWKV) | [![arXiv:2403.02308](https://img.shields.io/badge/arXiv-2403.02308-b31b1b.svg)](https://arxiv.org/abs/2403.02308)| 🏅🏅🏅【ICLR 2025 Spotlight】基于 RWKV 的视觉感知模型，能平滑处理高分辨率图像。 |
| PointRWKV | [![Star](https://img.shields.io/github/stars/hithqd/PointRWKV.svg?style=social&label=Star)](https://github.com/hithqd/PointRWKV) |[![arXiv:2405.15214](https://img.shields.io/badge/arXiv-2405.15214-b31b1b.svg)](https://arxiv.org/abs/2405.15214) | 🏅【AAAI 2025 】基于 RWKV 的 3D 点云学习框架。 |



### 图像分割

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| U-RWKV | [![Star](https://img.shields.io/github/stars/hbyecoding/U-RWKV.svg?style=social&label=Star)](https://github.com/hbyecoding/U-RWKV) | | 基于 RWKV 的图像分割模型。 |
| RWKV-SAM | [![Star](https://img.shields.io/github/stars/HarborYuan/ovsam.svg?style=social&label=Star)](https://github.com/HarborYuan/ovsam) | [![arXiv:2401.02955](https://img.shields.io/badge/arXiv-2401.02955-b31b1b.svg)](https://arxiv.org/abs/2401.02955)| 🏅【ECCV 2024】基于 RWKV 的开放词表图像分段切割方法“RWKV-SAM”。 |

### 图像生成

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Diffusion-RWKV | [![Star](https://img.shields.io/github/stars/feizc/Diffusion-RWKV.svg?style=social&label=Star)](https://github.com/feizc/Diffusion-RWKV) |[![arXiv:2404.04478](https://img.shields.io/badge/arXiv-2404.04478-b31b1b.svg)](https://arxiv.org/abs/2404.04478) | 基于 RWKV 的图像生成任务模型，擅长处理高分辨率图像。 |

### 目标检测

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| LION | [![Star](https://img.shields.io/github/stars/happinesslz/LION.svg?style=social&label=Star)](https://github.com/happinesslz/LION) | [![arXiv:2407.18232](https://img.shields.io/badge/arXiv-2407.18232-b31b1b.svg)](https://arxiv.org/abs/2407.18232)| 🏅【NeurIPS 2024】用于点云中 3D 对象检测的 Linear Group RNN（支持 RWKV）。 |

### 其他图像任务

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| FEAT | [![Star](https://img.shields.io/github/stars/Yaziwel/FEAT?style=social&label=Star)](https://github.com/Yaziwel/FEAT) |[![arXiv:2506.04956](https://img.shields.io/badge/arXiv-2506.04956-b31b1b.svg)](https://arxiv.org/abs/2506.04956) | 🏅🏅【MICCAI 2025 early accepted】基于 RWKV 的医学视频生成。 |
| Restore-RWKV | [![Star](https://img.shields.io/github/stars/Yaziwel/Restore-RWKV.svg?style=social&label=Star)](https://github.com/Yaziwel/Restore-RWKV) |[![arXiv:2407.11087](https://img.shields.io/badge/arXiv-2407.11087-b31b1b.svg)](https://arxiv.org/abs/2407.11087) | 使用 RWKV 进行高效且有效的医学图像恢复（PyTorch 实现）。 |
| LineRWKV | [![Star](https://img.shields.io/github/stars/diegovalsesia/linerwkv.svg?style=social&label=Star)](https://github.com/diegovalsesia/linerwkv) | [![arXiv:2403.17677](https://img.shields.io/badge/arXiv-2403.17677-b31b1b.svg)](https://arxiv.org/abs/2403.17677)| LineRWKV 是一种对高光谱图像进行无损和有损压缩的方法。 |

---

## 音频相关

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| RWKV-TTS | [![Star](https://img.shields.io/github/stars/yynil/RWKVTTS.svg?style=social&label=Star)](https://github.com/yynil/RWKVTTS) | [![arXiv:2504.03289](https://img.shields.io/badge/arXiv-2504.03289-b31b1b.svg)](https://arxiv.org/abs/2504.03289) | RWKV 语音合成模型，支持多种语言的文本转语音。 |
| RWKV-ASR | [![Star](https://img.shields.io/github/stars/AGENDD/RWKV-ASR.svg?style=social&label=Star)](https://github.com/AGENDD/RWKV-ASR) | | 使用预训练的 RWKV 语言模型进行**语音识别**。 |

---

## 时间序列

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| BlackGoose_Rimer | [![Star](https://img.shields.io/github/stars/Alic-Li/BlackGoose_Rimer.svg?style=social&label=Star)](https://github.com/Alic-Li/BlackGoose_Rimer) |[![arXiv:2503.06121](https://img.shields.io/badge/arXiv-2503.06121-b31b1b.svg)](https://arxiv.org/abs/2503.06121) | 基于 RWKV-7 的时间序列预测模型，支持多种时间序列任务。 |
| RWKV-TS | [![Star](https://img.shields.io/github/stars/howard-hou/RWKV-TS.svg?style=social&label=Star)](https://github.com/howard-hou/RWKV-TS) | | 基于 RWKV 的时间序列任务模型，低延迟和内存占用。 |

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

## RWKV-RAG

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| RWKV-RAG | [![Star](https://img.shields.io/github/stars/AIIRWKV/RWKV-RAG.svg?style=social&label=Star)](https://github.com/AIIRWKV/RWKV-RAG) | | 基于 RWKV 模型的一键 RAG 部署系统，可轻松搭建和管理本地知识库，同时提供了基于本地知识库的问答机器人和 RWKV 一键微调功能。 |

---

## 聊天机器人与推理 API 服务器

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| **⭐ (中文推荐)** RWKV Runner | [![Star](https://img.shields.io/github/stars/josStorer/RWKV-Runner.svg?style=social&label=Star)](https://github.com/josStorer/RWKV-Runner) | | RWKV Runner 是 RWKV 模型的管理和启动工具，带用户友好的 GUI 界面，支持训练和推理。 |
| **⭐ (中文推荐)** AI00 RWKV Server | [![Star](https://img.shields.io/github/stars/cgisky1980/ai00_rwkv_server.svg?style=social&label=Star)](https://github.com/cgisky1980/ai00_rwkv_server) | | Ai00 Server 是基于 web-rwkv 推理引擎的 RWKV 模型**推理 API 服务器**。 |
| **🇨🇳 (中文)** 闻达 Web UI | [![Star](https://img.shields.io/github/stars/wenda-LLM/wenda.svg?style=social&label=Star)](https://github.com/wenda-LLM/wenda) | | 针对特定环境进行内容生成的 LLM 调用平台，支持 RWKV 模型。 |
| **🇨🇳 (中文)** Role Play Chatbot | [![Star](https://img.shields.io/github/stars/shengxia/RWKV_Role_Playing.svg?style=social&label=Star)](https://github.com/shengxia/RWKV_Role_Playing) | | 基于 RWKV 的角色扮演 WebUI，使用 Gradio 制作。 |
| Easy_RWKV_webui | [![Star](https://img.shields.io/github/stars/No-22-Github/Easy_RWKV_webui.svg?style=social&label=Star)](https://github.com/No-22-Github/Easy_RWKV_webui) | | 基于 PyWebIO 的 RWKV 模型在线聊天室。 |
| Mini Model Daemon | [![Star](https://img.shields.io/github/stars/recursal/minmodmon.svg?style=social&label=Star)](https://github.com/recursal/minmodmon) | | 基于 web-rwkv 推理后端的 RWKV 模型推理工具。 |
| LocalAI | [![Star](https://img.shields.io/github/stars/go-skynet/LocalAI.svg?style=social&label=Star)](https://github.com/go-skynet/LocalAI) | | 开源 OpenAI 替代品，支持 RWKV。 |
| GPT Academic | [![Star](https://img.shields.io/github/stars/binary-husky/gpt_academic.svg?style=social&label=Star)](https://github.com/binary-husky/gpt_academic) | | 为 GPT/GLM 等 LLM 大语言模型提供实用化交互接口，支持 RWKV。 |
| LLMFarm | [![Star](https://img.shields.io/github/stars/guinmoon/LLMFarm.svg?style=social&label=Star)](https://github.com/guinmoon/LLMFarm) | | 使用 GGML 库在 iOS 和 MacOS 上离线使用大型语言模型，支持 RWKV。 |

---

## RWKV 基准测试

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| Uncheatable Eval | [![Star](https://img.shields.io/github/stars/Jellyfish042/uncheatable_eval.svg?style=social&label=Star)](https://github.com/Jellyfish042/uncheatable_eval) | | 使用最新的动态数据测试 LLM 性能，包含 RWKV。 |
| RULER_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/RULER_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/RULER_RWKV) | | RWKV 模型的 [RULER](https://arxiv.org/abs/2404.06654) 测试分数。 |
| LongBench_RWKV | [![Star](https://img.shields.io/github/stars/Ojiyumm/LongBench_RWKV.svg?style=social&label=Star)](https://github.com/Ojiyumm/LongBench_RWKV) | | RWKV 的 [LongBench](https://arxiv.org/abs/2308.14508) 测试分数。 |
| rwkv_mmlu | [![Star](https://img.shields.io/github/stars/Jellyfish042/rwkv_mmlu.svg?style=social&label=Star)](https://github.com/Jellyfish042/rwkv_mmlu) | | RWKV 模型的 MMLU 测试分数。 |

---

## RWKV 推理框架/算子库

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
|cann-ops-rwkv|[![Star](https://img.shields.io/github/stars/appleinsky/rwkv_Ascend.svg?style=social&label=Star)](https://github.com/appleinsky/rwkv_Ascend)||昇腾与rwkv共建的算子仓库|
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
| **🚧 (开发中)** rwkv-mobile | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-mobile.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-mobile) | | RWKV 移动端推理引擎。 |
| rwkv-qualcomm | [![Star](https://img.shields.io/github/stars/MollySophia/rwkv-qualcomm.svg?style=social&label=Star)](https://github.com/MollySophia/rwkv-qualcomm) | | 使用 Qualcomm AI Engine Direct SDK 推理 RWKV 模型。 |
| rwkv-by-hand-excel | [![Star](https://img.shields.io/github/stars/playaswd/rwkv-by-hand-excel.svg?style=social&label=Star)](https://github.com/playaswd/rwkv-by-hand-excel) | | 使用 Excel 实现 RWKV，帮助开发者探索 RWKV 原理。 |
| RWKV-Infer | [![Star](https://img.shields.io/github/stars/OpenMOSE/RWKV-Infer.svg?style=social&label=Star)](https://github.com/OpenMOSE/RWKV-Infer) | | 使用 FLA 进行 RWKV-V6/V7 推理，支持组合多个状态进行推理。 |
| MLC LLM | [![Star](https://img.shields.io/github/stars/mlc-ai/mlc-llm.svg?style=social&label=Star)](https://github.com/mlc-ai/mlc-llm) | | 机器学习编译器和高性能部署引擎，支持 RWKV 模型。 |

---

## 其他 RWKV 项目

| 标题 | 代码 | 论文 | 简介 |
| :--- | :--- | :--- | :--- |
| SpikeGPT | [![Star](https://img.shields.io/github/stars/ridgerchu/SpikeGPT.svg?style=social&label=Star)](https://github.com/ridgerchu/SpikeGPT) | | 一款受 RWKV 启发的新模型。 |
| JSONL to binidx | [![Star](https://img.shields.io/github/stars/Abel2076/json2binidx_tool.svg?style=social&label=Star)](https://github.com/Abel2076/json2binidx_tool) | | 这个工具用于将 `.jsonl` 文件转成适合 RWKV 训练的 `.bin /.idx`（binidx）数据。 |
| AI Town - RWKV Proxy | [![Star](https://img.shields.io/github/stars/recursal/ai-town-rwkv-proxy.svg?style=social&label=Star)](https://github.com/recursal/ai-town-rwkv-proxy?tab=readme-ov-file) | | 通过 RWKV 在本地运营一个大型 AI 城镇！ |
| Bot-Ani-RWKV | [![Star](https://img.shields.io/github/stars/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection.svg?style=social&label=Star)](https://github.com/Max-SF1/Bot-Ani-RWKV-twitter-bot-detection) | | 基于 RWKV 的推特水军机器人检测工具。|
| RWKVInverseFolding | [![Star](https://img.shields.io/github/stars/Lyttr/RWKVInverseFolding.svg?style=social&label=Star)](https://github.com/Lyttr/RWKVInverseFolding) | | 使用 RWKV 进行反向折叠。|
| poker-ai-rwkv | [![Star](https://img.shields.io/github/stars/meraline/poker-ai-rwkv.svg?style=social&label=Star)](https://github.com/meraline/poker-ai-rwkv) | | 带有 RWKV 的AI 扑克牌游戏系统。|
|Muon-RMS-Norm|[![Star](https://img.shields.io/github/stars/xTimeCrystal/Muon-RMS-Norm.svg?style=social&label=Star)](https://github.com/xTimeCrystal/Muon-RMS-Norm)|||