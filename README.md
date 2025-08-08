---
license: cc-by-nc-4.0
tags:
  - geometric deep learning
  - SE(3)
  - spatial reasoning
  - AI geometry
---

<div align="center">

# 🎯 GASM Weights
## Geometric Attention for Spatial & Mathematical Understanding

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Hugging Face Space](https://img.shields.io/badge/🤗%20Hugging%20Face-Space-yellow)](https://huggingface.co/spaces/scheitelpunk/GASM)

*Neural architecture for SE(3)-invariant spatial reasoning from natural language*

</div>

---

## 🧠 About GASM

**GASM** stands for **Geometric Attention for Spatial & Mathematical Understanding**

This repository contains the pretrained model weights used in the live [Hugging Face Space](https://huggingface.co/spaces/scheitelpunk/GASM) to map input text into structured 3D spatial representations.

### 🔬 Technical Components

- 🗣️ **NLP**: spaCy-based entity & relation parsing
- 📐 **Geometry**: Lie group operations in **SE(3)** space  
- 🌀 **Optimization**: Riemannian curvature optimization

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `gasm_weights.pth` | PyTorch weights file used by the core GASM engine |

---

## 🚀 Quick Start

Load the weights into your own pipeline using `huggingface_hub`:

```python
from huggingface_hub import hf_hub_download
import torch

# Download and load weights
weights_path = hf_hub_download("scheitelpunk/gasm-weights", "gasm_weights.pth")
model.load_state_dict(torch.load(weights_path))
```

---

## 📄 License

Released under **CC-BY-NC 4.0** - For research and non-commercial use only. All rights reserved, Versino PsiOmega GmbH

### 📚 Citation

If you use GASM or its weights, please cite:

```bibtex
@misc{gasm2025,
  title={GASM: Geometric Attention for Spatial Understanding},
  author={Michael Neuberger, Versino PsiOmega GmbH},
  year={2025},
  url={https://huggingface.co/spaces/scheitelpunk/GASM}
}
```

---

## 🔗 Related Repositories

- 🔬 **[GASM Space](https://huggingface.co/spaces/scheitelpunk/GASM)** - Live demo
- 💻 **[Source Code](https://github.com/scheitelpunk/GASM-Huggingface)** - Implementation

---

<div align="center">

**Made with ❤️ for geometric deep learning**

Versino PsiOmega GmbH, http://psiomega.versino.de
</div>

