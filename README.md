# MedGRPO: Multi-Task Reinforcement Learning for Heterogeneous Medical Video Understanding

This repository contains the project website for MedGRPO.

## Project Page

Visit the project page at: [https://yuhaosu.github.io/MedGRPO/](https://yuhaosu.github.io/MedGRPO/)

## Overview

**MedGRPO** introduces a comprehensive framework for medical video understanding, combining a large-scale dataset with a novel multi-task reinforcement learning approach.

### MedVidBench Dataset

- **531K video-instruction pairs**: Large-scale dataset for medical video understanding
- **8 diverse tasks**: Covers video-level, segment-level, and frame-level understanding

### MedGRPO Framework

- **Multi-Task Reinforcement Learning**: Novel RL framework for heterogeneous medical video tasks
- **Cross-Dataset Reward Normalization**: Balanced training across different tasks
- **Medical LLM Judge**: Specialized evaluation for medical video captions

### Results

Compared to SFT baseline:
- **+0.074 mIoU@0.3** on temporal action grounding
- **+0.588 LLM score** on video summary generation
- Consistent improvements across all 8 tasks

## Website Template

This website is based on the [Nerfies](https://nerfies.github.io) template.

## Citation

```bibtex
@article{su2025medgrpo,
  title={MedGRPO: Multi-Task Reinforcement Learning for Heterogeneous Medical Video Understanding},
  author={Su, Yuhao and Choudhuri, Anwesa and Gao, Zhongpai and Planche, Benjamin and Nguyen, Van Nguyen and Zheng, Meng and Shen, Yuhan and Innanje, Arun and Chen, Terrence and Elhamifar, Ehsan and Wu, Ziyan},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
}
```

## Deploying to GitHub Pages

1. Create a new repository named `MedGRPO` on GitHub
2. Push this folder to the repository
3. Go to Settings → Pages → Source: Deploy from a branch → Select `main` branch
4. The site will be live at `https://yuhaosu.github.io/MedGRPO/`
