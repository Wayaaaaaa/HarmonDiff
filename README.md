

## Abstract

Medical image segmentation under limited annotation settings remains a significant challenge, as ambiguous boundaries, inter-patient anatomical variations, and imaging artifacts collectively degrade the reliability of pseudo-label supervision. Current semi-supervised methods rely primarily on spatial-domain feature learning and deterministic decoding. Consequently, they frequently suffer from blurred boundaries, structurally inconsistent predictions, and inadequate uncertainty estimation. To overcome these limitations, we introduce HarmonDiff, a dual-domain latent diffusion framework for semi-supervised medical image segmentation. HarmonDiff couples a primary segmentation network with a training-time latent refinement network. Specifically, it leverages a dual-domain fusion strategy to inject complementary spatial and spectral cues into multi-scale, image-conditioned features. Additionally, a frequency-domain enhancement module refines bottleneck representations in the Fourier domain, while a latent diffusion module denoises semantic features to generate structurally consistent pseudo-labels. Furthermore, a wavelet-guided decoder is employed to preserve high-frequency anatomical details during feature reconstruction while mitigating checkerboard artifacts. Extensive experiments across the ACDC, MSCMRSEG 2019, and Decathlon Prostate datasets demonstrate the effectiveness and strong generalization capability of the proposed framework. Specifically, on the ACDC dataset, HarmonDiff achieves Dice scores of 76.76%, 88.14%, and 90.42% using 1%, 5%, and 10% labeled data, respectively, consistently outperforming competing semi-supervised methods. Additionally, it attains a Dice score of 86.70% on MSCMRSEG 2019 with 20% labeled data, and 57.58% on Decathlon Prostate with 10% labeled data. Ultimately, these findings establish HarmonDiff as a highly robust, uncertainty-aware, and structure-preserving solution for semi-supervised medical image segmentation.

We will make our code publicly available once the paper is accepted. The GitHub repository link is: [HarmonDiff](https://github.com/Wayaaaaaa/HarmonDiff)

---

## Overview


![Network Architecture Diagram](1.png)

