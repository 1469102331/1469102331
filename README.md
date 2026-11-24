# Hi, I'm Shuo Guo 👋

**M.Sc. student in Computer Technology @ Hunan Normal University (HUNNU)**

I work on **hyperspectral imaging** — fusing a low-resolution hyperspectral image with a high-resolution multispectral image to recover a high-resolution hyperspectral image (HR-HSI), with an emphasis on **spectral fidelity** and **spatial detail refinement**.

![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-2.1-EE4C2C?logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-11.8-76B900?logo=nvidia&logoColor=white)
![Research](https://img.shields.io/badge/Research-Hyperspectral%20Imaging-8A2BE2)

---

## 🔬 Research Interests

- **Hyperspectral and multispectral image fusion (HMIF)** — spectral consistency constrained reconstruction, latent coefficient estimation, nonlinear spectral mapping
- **Spectral super-resolution / reconstruction** — spectral prior learning, response-matrix calibration
- **Detail refinement with transform-domain priors** — discrete wavelet transform, high-frequency subband enhancement
- **Efficient attention & state-space models** — dual-guided multi-head hybrid attention, Mamba-convolution hybrids
- **Remote sensing image processing** — pansharpening, benchmark evaluation on CAVE / Harvard / KAIST / Pavia

---

## 📄 Papers & Code

| Work | Venue | Code | Paper |
|---|---|---|---|
| **SINet** — Spatial Invertible Network with Mamba-Convolution for Hyperspectral Image Fusion | Preprint | [![Repo](https://img.shields.io/badge/GitHub-SINet-181717?logo=github)](https://github.com/Guoshuo-cv/SINet) | [PDF](https://github.com/Guoshuo-cv/SINet/blob/main/SINet.pdf) |
| **SCDRNet** — Learning Spectral Consistency and Detail Refinement for Hyperspectral Image Fusion | Under review | [![Repo](https://img.shields.io/badge/GitHub-SCDRNet-181717?logo=github)](https://github.com/Guoshuo-cv/SCDRNet) | [PDF](https://github.com/Guoshuo-cv/SCDRNet/blob/main/SCDRNet.pdf) |

**SCDRNet in one paragraph.** HMIF is reformulated as a *spectrally constrained detail reconstruction* problem and solved by a two-stage network: (1) an MSI-aligned latent coefficient estimator plus a shared nonlinear spectral reconstruction network, which produces a spectrally consistent initialization; (2) a wavelet-based detail refinement stage where a Dual-Guided Multi-Head Hybrid Attention (DGMHA) module enhances high-frequency subbands while the low-frequency component is replaced by HS-derived spectral features. Fixed Haar filters keep the transform parameter-free and exactly invertible.

---

## 💻 Highlighted Repositories

**[SCDRNet](https://github.com/Guoshuo-cv/SCDRNet)** · `PyTorch` `hyperspectral-image-fusion` `wavelet` `attention`
Two-stage spectral-consistency + detail-refinement network, with full training / testing / evaluation scripts and the paper PDF.

**[SINet](https://github.com/Guoshuo-cv/SINet)** · `PyTorch` `Mamba` `invertible-network` `image-fusion`
Spatial invertible network with Mamba-convolution for HR-HSI reconstruction; framework figure, requirements and metric code included.

Both repositories share the same evaluation protocol: CAVE / Harvard / KAIST with 8× spatial downsampling, Gaussian PSF ($\sigma=3$, $8\times8$), and the Nikon D700 spectral response matrix to simulate the HR-MSI.

---

## 🎓 Education

- **M.Sc. in Computer Technology** — Hunan Normal University, Changsha, China *(current)*
- **B.Sc.** — Nanjing Agricultural University; thesis on *Chinese herbal medicine image recognition*

---

## 🔗 Links

[![ORCID](https://img.shields.io/badge/ORCID-0009--0003--2915--5436-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0003-2915-5436)
[![GitHub](https://img.shields.io/badge/GitHub-Guoshuo-cv-181717?logo=github)](https://github.com/Guoshuo-cv)

📫 Best way to reach me: open an issue in the relevant repository, or contact me via ORCID.

---

## 🌸 Acknowledgement

My code and evaluation pipeline benefit from open-source efforts including
[DSPNet](https://github.com/syc11-25/DSPNet),
[LRTN](https://github.com/YuanyeLiu/Low-Rank-Transformer-For-High-Resolution-Hyperspectral-Computational-Imaging),
[Hyper-DSNet](https://github.com/liangjiandeng/Hyper-DSNet) and
[HyperPanCollection](https://github.com/liangjiandeng/HyperPanCollection).
Thanks to all the contributors.

<br/>

<details>
<summary>中文简介</summary>

Shuo Guo，湖南师范大学计算机技术硕士研究生，研究方向为高光谱与多光谱图像融合、光谱重建与空间细节增强。关注谱一致性约束下的重建建模、隐系数估计、非线性光谱映射、小波域细节增强以及 Mamba/Transformer 混合结构在高光谱融合中的应用。代表性工作 SINet 与 SCDRNet，代码与论文均已开源。

</details>
