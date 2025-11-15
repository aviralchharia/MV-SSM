<div align="center">

# MV-SSM: Multi-View State Space Modeling for 3D Human Pose Estimation

<div>
    <a href='https://aviralchharia.github.io/' target='_blank'>Aviral Chharia*</a>&emsp;
    <a href='https://www.linkedin.com/in/wenbogou' target='_blank'>Wenbo Gou*</a>&emsp;
    <a href='https://www.haoyed.com/' target='_blank'>Haoye Dong*</a>&emsp;
</div>
<div>
    Carnegie Mellon University&emsp;  National University of Singapore<br>
</div>
<div>
    <b>CVPR 2025</b>
</div>
<br>

  <a href="https://arxiv.org/abs/2509.00649"><img alt="arXiv" src="https://img.shields.io/badge/arXiv-2509.00649-00ff00.svg"></a>
  <a href="https://aviralchharia.github.io/MV-SSM/"><img alt="Webpage" src="https://img.shields.io/badge/Webpage-up-yellow"></a>
  [![GitHub Stars](https://img.shields.io/github/stars/aviralchharia/MV-SSM?style=social)](https://github.com/aviralchharia/MV-SSM)

---

<img src="assets/Motivation.jpeg" width="49%"/>

<strong> Comparison of different token scanning methods. (a) Cross Attention acts on all image tokens. (b) Projective Attention obtains anchors with perspective projection and selectively attends to sample tokens surrounding the anchor points. (c) The proposed Grid Token-guided Bidirectional Scanning (GTBS) encodes the local context and the joint spatial sequence at the visual feature and person-keypoint levels. </strong><br>
:open_book: For visual results, go checkout our <a href="https://aviralchharia.github.io/MV-SSM/" target="_blank">project page</a>
</div>

---

## :rocket: **Updates**
- 🔲 **Dec. 15, 2025**: MV-SSM Codes and Model Weights. Coming Soon!
- ✅ **Aug. 31, 2025**: We released MV-SSM on arXiv. Check the preprint!
- ✅ **Aug. 12, 2025**: MV-SSM is featured on TechXplore! Check out our [Blog](https://techxplore.com/news/2025-08-cameras-problems-deep-struggles-3d.html).
- ✅ **Feb. 26, 2025**: MV-SSM accepted at CVPR. Check out our Poster [here](https://cvpr.thecvf.com/virtual/2025/poster/33025). See everyone at Nashville!</i>

## :open_book: **Abstract**

While significant progress has been made in single-view 3D human pose estimation, multi-view 3D human pose estimation remains challenging, particularly in terms of generalizing to new camera configurations. Existing attention-based transformers often struggle to accurately model the spatial arrangement of keypoints, especially in occluded scenarios. Additionally, they tend to overfit specific camera arrangements and visual scenes from training data, resulting in substantial performance drops in new settings. In this study, we introduce a novel Multi-View State Space Modeling framework, named MV-SSM, for robustly estimating 3D human keypoints. We explicitly model the joint spatial sequence at two distinct levels: the feature level from multi-view images and the person keypoint level. We propose a Projective State Space (PSS) block to learn a generalized representation of joint spatial arrangements using state space modeling. Moreover, we modify Mamba's traditional scanning into an effective Grid Token-guided Bidirectional Scanning (GTBS), which is integral to the PSS block. Multiple experiments demonstrate that MV-SSM achieves strong generalization, outperforming state-of-the-art methods: +10.8 on AP25 (+24%) on the challenging three-camera setting in CMU Panoptic, +7.0 on AP25 (+13%) on varying camera arrangements, and +15.3 PCP (+38%) on Campus A1 in cross-dataset evaluations.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=aviralchharia/MV-SSM&type=Date)](https://www.star-history.com/#aviralchharia/MV-SSM&Date)

## License

Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc]. 
Permission is granted for non-commercial research. For commerical use, please reachout to us.

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg

## Acknowledgements

Parts of the codes have been taken and adapted from the below repos. Please acknowledge and adhere to the licenses of each repository that Hamba builds upon.
- [Mamba](https://github.com/state-spaces/mamba)
- [VMamba](https://github.com/MzeroMiko/VMamba)
- [MVGFormer](https://github.com/XunshanMan/MVGFormer)
- [MvP](https://github.com/sail-sg/mvp)
- [VoxelPose](https://github.com/microsoft/voxelpose-pytorch)

## :bookmark_tabs: Citation
If you find our work useful for your project, please consider adding a star to this repo and citing our paper:
```bibtex
    @inproceedings{chharia2025mv,
      title={MV-SSM: Multi-View State Space Modeling for 3D Human Pose Estimation},
      author={Chharia, Aviral and Gou, Wenbo and Dong, Haoye},
      booktitle={Proceedings of the Computer Vision and Pattern Recognition Conference},
      pages={11590--11599},
      year={2025}
    }
```
