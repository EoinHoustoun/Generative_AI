# Neural Style Transfer — Generative AI

Transforms celebrity photographs into comic book-style illustrations using deep neural artistic rendering with VGG19 and PyTorch — a full implementation of the Gatys et al. neural style transfer algorithm.

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org)
[![Generative AI](https://img.shields.io/badge/Generative%20AI-Computer%20Vision-7c3aed?style=for-the-badge)](https://github.com/EoinHoustoun/Generative_AI)
[![VGG19](https://img.shields.io/badge/Model-VGG19%20CNN-d97706?style=for-the-badge)](https://pytorch.org/vision/stable/models/vgg.html)

![Style Transfer Demo](https://github.com/EoinHoustoun/Eoin_Houstoun/blob/master/style_transfer6.gif?raw=true)

---

## Overview

- **Problem:** Neural artistic stylisation — transferring the visual style of one image (e.g. comic book art) onto the content of another (e.g. a photograph) while preserving recognisable structure.
- **Approach:** VGG19 CNN used as a fixed feature extractor. Content loss preserves high-level structure via deep layer activations; style loss captures texture and colour via Gram matrices across multiple layers. Iterative optimisation blends both.
- **Result:** Photorealistic stylisation of celebrity portraits into comic book illustrations, with animated GIFs documenting the full transformation process.

---

## Key Features

- VGG19 CNN feature extraction for separating content and style representations
- Gram matrix computation for multi-layer style loss
- Adjustable content/style loss weighting — controllable artistic effect intensity
- Intermediate checkpoint saving with animated GIF generation to visualise the optimisation process
- Swappable style images — apply any artistic reference to any content image
- Supports different optimisation algorithms for experimentation

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Framework | PyTorch |
| Model | VGG19 (pretrained, ImageNet) |
| Technique | Neural Style Transfer, Gram Matrix, Content/Style Loss |
| Libraries | torchvision, PIL, NumPy |
| Visualisation | matplotlib, GIF generation |

---

## Results

- Successfully transferred comic book illustration style onto celebrity portrait photographs
- Animated GIFs capture the iterative stylisation process from raw content to fully stylised output
- Adjustable alpha/beta weighting enables fine control over the photorealism vs. stylisation trade-off

---

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Swap in your own content and style images to generate custom stylisations.

---

## Project Structure

```
Generative_AI/
├── neural_style_transfer.ipynb   # Main implementation notebook
├── images/
│   ├── content/                  # Input photographs
│   └── style/                    # Style reference images
├── outputs/                      # Generated images and GIFs
├── requirements.txt
└── README.md
```

---

*Part of Eoin Houstoun's Data Science Portfolio — [github.com/EoinHoustoun](https://github.com/EoinHoustoun)*
