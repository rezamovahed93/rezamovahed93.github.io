---
layout: page
title: EEG-based Machine Learning for Depression Diagnosis
description: Machine learning and deep learning frameworks for diagnosing major depressive disorder from EEG signals.
img: assets/img/eeg_depression_diagram.png
importance: 1
category: research
---
{% include figure.liquid path="assets/img/eeg_depression_diagram.png" title="EEG-based MDD diagnosis pipeline" class="img-fluid rounded z-depth-1" %}

Major depressive disorder (MDD) is typically diagnosed through questionnaire-based clinical assessments, which can be subjective and may not always lead to an accurate diagnosis. This line of work explores how electroencephalogram (EEG) signals — an objective, non-invasive, and cost-effective measure of brain activity — can be combined with machine learning and deep learning to build more reliable, automated MDD diagnostic tools.

The work progressed across three studies:

**A classical machine learning framework** combined statistical, spectral, wavelet, functional connectivity, and nonlinear features extracted from EEG signals, with sequential backward feature selection used to identify the most informative feature subset before classification.

**A dictionary learning approach** built on this by using dictionary learning together with functional connectivity features to further improve diagnostic accuracy while keeping the pipeline interpretable.

**A deep learning approach** moved beyond hand-crafted features entirely: two images were constructed directly from EEG signals — one capturing spectral information, the other functional connectivity — and passed through a two-stream convolutional neural network. The combined output was then classified using a sequential LSTM, fully connected, and softmax architecture.

All three studies were validated on a public EEG dataset comprising recordings from 34 MDD patients and 30 healthy controls.

**Publications:**
- [A major depressive disorder classification framework based on EEG signals using statistical, spectral, wavelet, functional connectivity, and nonlinear analysis](https://doi.org/10.1016/j.jneumeth.2021.109209) — *Journal of Neuroscience Methods*, 2021
- [A major depressive disorder diagnosis approach based on EEG signals using dictionary learning and functional connectivity features](https://doi.org/10.1007/s13246-022-01135-1) — *Physical and Engineering Sciences in Medicine*, 2022
- [Automated major depressive disorder diagnosis using a dual-input deep learning model and image generation from EEG signals](https://doi.org/10.1080/17455030.2023.2187237) — *Waves in Random and Complex Media*, 2023
