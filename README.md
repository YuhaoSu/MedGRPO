# MedGRPO: Multi-Task Reinforcement Learning for Heterogeneous Medical Video Understanding

[![Project Page](https://img.shields.io/badge/Project-Page-blue)](https://yuhaosu.github.io/MedGRPO/)
[![Code](https://img.shields.io/badge/GitHub-Code-black?logo=github)](https://github.com/UII-AI/MedGRPO-Code)
[![Model](https://img.shields.io/badge/🤗-Model-yellow)](https://huggingface.co/UII-AI/uAI-NEXUS-MedVLM-1.0a-7B-RL)
[![Demo](https://img.shields.io/badge/🤗-Demo-yellow)](https://huggingface.co/spaces/UII-AI/MedGRPO-Demo)
[![Benchmark](https://img.shields.io/badge/🤗-MedVidBench-yellow)](https://huggingface.co/datasets/UII-AI/MedVidBench)
[![Leaderboard](https://img.shields.io/badge/🤗-Leaderboard-yellow)](https://huggingface.co/spaces/UII-AI/MedVidBench-Leaderboard)

## Abstract

Large vision-language models struggle with medical video understanding, where spatial precision, temporal reasoning, and clinical semantics are critical. To address this, we first introduce **MedVidBench**, a large-scale benchmark of 531,850 video-instruction pairs across 8 medical sources spanning video, segment, and frame-level tasks, curated through a rigorous quality assurance pipeline with expert-guided prompting and dual-model validation.

While supervised fine-tuning on MedVidBench yields noticeable gains, standard Reinforcement Learning (RL) fails due to imbalanced reward scales across datasets, which destabilizes optimization and leads to training collapse. To overcome this, we introduce **MedGRPO**, a novel RL framework for balanced multi-dataset training with two key innovations: (1) *cross-dataset reward normalization* that maps each dataset's median performance to a common reward value, ensuring fair optimization regardless of difficulty, and (2) a *medical LLM judge* that evaluates caption quality on five clinical dimensions through comparative similarity scoring.

Supervised fine-tuning Qwen2.5-VL-7B on MedVidBench substantially outperforms GPT-4.1 and Gemini-2.5-Flash across all tasks, demonstrating MedVidBench's efficacy, while our MedGRPO framework further improves upon the SFT baseline across grounding and captioning tasks. Our work establishes a foundational benchmark and robust training methodology for advancing vision-language models in medical domains.

## Citation

```bibtex
@article{su2025medgrpo,
  title={MedGRPO: Multi-Task Reinforcement Learning for Heterogeneous Medical Video Understanding},
  author={Su, Yuhao and Choudhuri, Anwesa and Gao, Zhongpai and Planche, Benjamin and Nguyen, Van Nguyen and Zheng, Meng and Shen, Yuhan and Innanje, Arun and Chen, Terrence and Elhamifar, Ehsan and Wu, Ziyan},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
}
```
