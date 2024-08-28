<h1 align="center"> GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion </h1>

<h3 align="center"> Jiaxin Wei and Stefan Leutenegger </h3>

<h3 align="center">
  <a href="https://arxiv.org/abs/2408.12677">Paper</a> | <a href="https://youtu.be/rW8o_cRPZBg">Video</a> | <a href="https://gs-fusion.github.io/">Project Page</a>
</h3>

<p align="center">
  <a href="">
    <img src="./media/teaser.gif" alt="teaser" width="100%">
  </a>
</p>

<p align="center"> All the reported results are obtained from a single Nvidia RTX 3060 GPU. </p>

Abstract: *Traditional volumetric fusion algorithms preserve the spatial structure of 3D scenes, which is beneficial for many tasks in computer vision and robotics. However, they often lack realism in terms of visualization. Emerging 3D Gaussian splatting bridges this gap, but existing Gaussian-based reconstruction methods often suffer from artifacts and inconsistencies with the underlying 3D structure, and struggle with real-time optimization, unable to provide users with immediate feedback in high quality. One of the bottlenecks arises from the massive amount of Gaussian parameters that need to be updated during optimization. Instead of using 3D Gaussian as a standalone map representation, we incorporate it into a volumetric mapping system to take advantage of geometric information and propose to use a quadtree data structure on images to drastically reduce the number of splats initialized. In this way, we simultaneously generate a compact 3D Gaussian map with fewer artifacts and a volumetric map on the fly. Our method, GSFusion, significantly enhances computational efficiency without sacrificing rendering quality, as demonstrated on both synthetic and real datasets.*

## Note

This repository contains the code used in the paper "GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion". The code will be released upon acceptance of the paper.


## Evaluation

We develop an automatic evaluation system for GSFusion and provide several pre-trained models for assessment. You can download the necessary data [here](https://cloud.cvai.cit.tum.de/s/dQZgJPE2ydzq32E), and follow the instructions in [GSFusion_eval](https://github.com/goldoak/GSFusion_eval) to get started.


## Citation

If you find our paper and code useful, please cite us:
```bibtex
@misc{wei2024gsfusiononlinergbdmapping,
      title={GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion}, 
      author={Jiaxin Wei and Stefan Leutenegger},
      year={2024},
      eprint={2408.12677},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2408.12677}, 
}
```
