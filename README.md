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

| Work | Venue | Status | Code | Links |
|---|---|---|---|---|
| **SINet** — Spatial Invertible Network With Mamba-Convolution for Hyperspectral Image Fusion | IEEE JSTSP, vol. 19, no. 8, Dec. 2025 | Published | [![Repo](https://img.shields.io/badge/GitHub-SINet-181717?logo=github)](https://github.com/Guoshuo-cv/SINet) | [PDF](https://github.com/Guoshuo-cv/SINet/blob/main/SINet.pdf) · [DOI](https://doi.org/10.1109/JSTSP.2025.3596518) |
| **SSDAN** — S²-Differential Feature Awareness Network for Hyperspectral Image Fusion | IEEE TGRS, vol. 64, Art. no. 5507410, 2026 | Published | [![Repo](https://img.shields.io/badge/GitHub-SSDAN-181717?logo=github)](https://github.com/MSFLabX/SSDAN) | [DOI](https://doi.org/10.1109/TGRS.2026.3671284) |
| **SCDRNet** — Learning Spectral Consistency and Detail Refinement for Hyperspectral Image Fusion | IEEE TIP, accepted (to appear) | Accepted | [![Repo](https://img.shields.io/badge/GitHub-SCDRNet-181717?logo=github)](https://github.com/Guoshuo-cv/SCDRNet) | Online version pending |

*One further paper is accepted and awaiting its online version; it will be listed here as soon as the final version appears.*

**SCDRNet in one paragraph.** HMIF is reformulated as a *spectrally constrained detail reconstruction* problem and solved by a two-stage network: (1) an MSI-aligned latent coefficient estimator plus a shared nonlinear spectral reconstruction network, which produces a spectrally consistent initialization; (2) a wavelet-based detail refinement stage where a Dual-Guided Multi-Head Hybrid Attention (DGMHA) module enhances high-frequency subbands while the low-frequency component is replaced by HS-derived spectral features. Fixed Haar filters keep the transform parameter-free and exactly invertible.

## 💻 Highlighted Repositories

**[SCDRNet](https://github.com/Guoshuo-cv/SCDRNet)** · `PyTorch` `hyperspectral-image-fusion` `wavelet` `attention`
Two-stage spectral-consistency + detail-refinement network, with full training / testing / evaluation scripts. (Paper accepted by IEEE TIP; full text will be linked after the online version appears.)

**[SSDAN](https://github.com/MSFLabX/SSDAN)** · `PyTorch` `differential-feature` `frequency-domain` `image-fusion`
S²-differential feature awareness network: spatial–frequency fusion network with a dual-branch design plus a differential S² complementarity module.

**[SINet](https://github.com/Guoshuo-cv/SINet)** · `PyTorch` `Mamba` `invertible-network` `image-fusion`
Spatial invertible network with Mamba-convolution for HR-HSI reconstruction; framework figure, requirements and metric code included.

Both repositories share the same evaluation protocol: CAVE / Harvard / KAIST with 8× spatial downsampling, Gaussian PSF ($\sigma=3$, $8\times8$), and the Nikon D700 spectral response matrix to simulate the HR-MSI.

---

## 🎓 Education

- **Master's (professional degree) in Electronic Information — Computer Technology (085404)** — Hunan Normal University, Changsha, China *(in progress)*
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

Shuo Guo，湖南师范大学电子信息（计算机技术，085404）专业学位硕士研究生，研究方向为高光谱与多光谱图像融合、光谱重建与空间细节增强。关注谱一致性约束下的重建建模、隐系数估计、非线性光谱映射、小波域细节增强以及 Mamba/Transformer 混合结构在高光谱融合中的应用。已发表 IEEE JSTSP（SINet）与 IEEE TGRS（SSDAN）各一篇，另有 2 篇已录用待在线出版；代表性代码均已开源（GitHub: Guoshuo-cv）。

</details>
