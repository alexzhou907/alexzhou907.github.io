---
permalink: /pvd
layout: project
title: '3D Shape Generation and Completion through Point-Voxel Diffusion'
site_name: ''
author_profile: false
redirect_from: 
  - /linqizhou/pvd
---

{% include data_path %}

<center><h1>3D Shape Generation and Completion through Point-Voxel Diffusion</h1></center>
<center><h3><a href="https://alexzhou907.github.io/">Linqi Zhou<sup>1</sup></a>&nbsp;&nbsp;&nbsp;
  <a href="https://yilundu.github.io/">Yilun Du<sup>2</sup></a>&nbsp;&nbsp;&nbsp;
  <a href="https://jiajunwu.com/">Jiajun Wu<sup>1</sup></a>
</h3></center>
<center><h3>
  <sup>1</sup> Stanford University;
  <sup>2</sup> MIT;
</h3></center>

<center><h3>
  ICCV 2021
</h3></center>

<!-- paper icons -->
<center>
<table style="margin-top: 20px">
    <tr>
        <td><center><a href="https://arxiv.org/abs/2104.03670" class="nav-link"><img class="filter-blue" src="{{ "/images/paper_icon.svg" | prepend: data_path }}" width="48" height="48"/><br>Paper</a></center>
        </td>
        <td><center><a href="https://github.com/alexzhou907/PVD" class="nav-link"><img class="filter-blue" src="{{ "/images/github.svg" | prepend: data_path }}" width="48" height="48"/><br>Code<br></a></center>
        </td>
    </tr>
</table>
</center>

<center>
<img src="{{ "/images/project_pages/pvd/pvd_teaser.gif" | prepend: data_path }}" width="900"/> 
</center>

<h2 class="title">Overview</h2>
<p>
We propose a novel approach for probabilistic generative modeling of 3D shapes. Unlike most existing models that learn to deterministically translate a latent vector to a shape, our model, Point-Voxel Diffusion (PVD), is a unified, probabilistic formulation for unconditional shape generation and conditional, multi-modal shape completion. PVD combines denoising diffusion models with the hybrid, point-voxel representation of 3D shapes. It can be viewed as a series of denoising steps, reversing the diffusion process from observed point cloud data to Gaussian noise, and is trained by optimizing a variational lower bound to the (conditional) likelihood function. Experiments demonstrate that PVD is capable of synthesizing high-fidelity shapes, completing partial point clouds, and generating multiple completion results from single-view depth scans of real objects. 
</p>
<center>

<div class="videoWrapper">
<iframe  src="https://www.youtube.com/embed/64jl79i6HNY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>


</center>

<h2 class="title">Generation and Completion</h2>
<p>
Our model can perform fully unconditional generation and conditional generation, a.k.a. shape completion. For the following
figure: (left) our generation result, (right) depth maps, sampled partial shapes, and our completion.
<center>
<div style="width: 700">
    <img src="{{ "/images/project_pages/pvd/gen_comp.gif" | prepend: data_path }}" /> 
    <table width="100%">
    <tr>
        <td style="width: 40%; text-align: center">Generation</td><td style="width: 5%;"></td>
        <td style="text-align: center">Completion</td>
    </tr>
</table>
</div>
</center>
</p>

<h2 class="title">Multimodal Completion</h2>
<p>
On ShapeNet, our model gives considerably diverse completion. For the following figure: (top) completion from input view,
(bottom) our completion. The depth image of the bottom of a chair is shown on the left.
<center>
<div style="width: 900">
    <img src="{{ "/images/project_pages/pvd/mm_shapenet.gif" | prepend: data_path }}"/> 
    <table width="100%">
    <tr>
        <td style="width: 20%; text-align: center;">Input Depth</td>
        <td style="text-align: center">Possible Completion</td>
    </tr>
</table>
</div>
</center>
On Partnet, our model produces completion with both higher fidelity and higher diversity. For the follwing figure, we present 
partial shape on the left and 5 different completion for each model on the right.
<br><br>
<center>
<div style="width: 900">
    <img src="{{ "/images/project_pages/pvd/mm_partnet.gif" | prepend: data_path }}"/> 
    <table width="100%">
    <tr>
        <td style="width: 8%;"></td>
        <td style="width: 28%; text-align: center">cGAN</td>
        <td style="width: 37%; text-align: center">KNN-latent</td><td style="width: 3%;"></td>
        <td style="text-align: center">PVD (Ours)</td>
    </tr>
</table>
</div>
</center>
</p>

<p>
Our pretrained model on ShapeNet can also perform well on real dataset, Redwood 3DScan. Here, the left two examples show more complete views of 
a chair and a table, whose completion are stable. The right two examples show more uncertain views of a chair and a table,
and their completion show variability. Within each example, (top) 3 completion from input view, (bottom) 3 full completion.
<center>
<div style="width: 900">
    <img src="{{ "/images/project_pages/pvd/mm_redwood.gif" | prepend: data_path }}"/> 
    <table width="100%">
    <tr>
        <td style="width: 15%; text-align: center">RGB-D</td>
        <td style="width: 33%; text-align: center">Possible Completion</td><td style="width: 3.5%;"></td>
        <td style="width: 15%; text-align: center">RGB-D</td>
        <td style="text-align: center">Possible Completion</td>
    </tr>
</table>
</div>
</center>
</p>
<h2 class="title">Citation</h2>
<pre>
@inproceedings{Zhou_2021_ICCV,
    author    = {Zhou, Linqi and Du, Yilun and Wu, Jiajun},
    title     = {3D Shape Generation and Completion Through Point-Voxel Diffusion},
    booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
    month     = {October},
    year      = {2021},
    pages     = {5826-5835}
}
</pre>

<p>Please send any questions to <a href="https://alexzhou907.github.io/">Linqi Zhou</a> and <a href="https://yilundu.github.io/">Yilun Du</a>.</p>



