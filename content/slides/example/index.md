---
title: Slides
summary: An introduction to using Hugo Blox Builder's Slides feature.
authors: []
tags: []
categories: []
date: '2019-02-05T00:00:00Z'
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

# Diffusion Probability Model
### Li Junbiao & Xie Junhong
#### Supervisors: Yang Sikun, Zheng Xubin, Li Xiaoming

---

## Table of Contents
1. Research Question and Motivation
2. Research Approach and Methodology
3. Interim Results
4. Summary and Reflections
5. Work Plan and Outlook

---

## Research Question and Motivation
- **Gaussian Distribution**: Used to represent measurement errors, for example, the volume of a 220mL filled beer bottle follows a Gaussian distribution with a mean of 220mL and a specific variance.
- **Denoising**: Introduces methods for denoising data using Diffusion Bridge and Score Matching through neural networks.
- **Score Matching**: Compares with DDPM which requires forward and backward processes, while this research only needs to construct a forward Bridge.

---

## Research Approach and Methodology
- **Diffusion Processes**: Discusses Drift Function and Diffusion Function.
- **Diffusion Bridge**: Introduces Diffusion Bridge as a process with conditional constraints at time T to be K.
- **Brownian Bridge**: Explains Brownian Bridge as a process for solving the backward Kolmogorov equation.
- **Training Method**: Demonstrates how to calculate Brownian Bridge by sampling points from source and target distributions, making every time point and point on the Brownian bridge into training data.

---

## Interim Results
- Shows the prediction process of fitting the Score function using MLP, including tasks in 1D and 2D.
- Introduces methods of fitting the Score function with neural networks, including generating “digit” images from the MNIST dataset.

---

## Summary and Reflections
- Discusses how simple models gradually reach a bottleneck in complex tasks.
- Suggests methods for improving models, such as using a UNet-based Model and time encoding.


---

## 5. Work Plan and Outlook
- Explores time reversal and complex image generation (such as animals, portraits, etc.).
- Plans to refine and tune the model, for instance, incorporating EfficientNet and ViT as encoders, and a Transformer decoder as the decoder.