# Image-to-joint inverse kinematics estimation of a cooperative continuum arm

<p align = 'left'>
    <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-3.8-ff69b4.svg" />
    <a href= "https://www.tensorflow.org">
    <img src="https://img.shields.io/badge/Tensorflow-2.13.1-2BAF2B.svg" /></a>
    <a href="https://developer.nvidia.com/cuda-toolkit">
    <img src="https://img.shields.io/badge/CUDA-11.8-76B900.svg" /></a>
</p>





<!-- ## Table of Contents
The goal of this project is to solve the inverse kinematics of the supportive continuum arm presented in https://www.computerrobotvision.org/, in Guelph, Ontario, Canada in May 28th.
1. [Introduction](#introduction)
2. [Dataset Details](#dataset-details)
3. [Usage](#usage)
4. [Contributing](#contributing)
5. [License](#license) -->

## Introduction

In this work, a deep learning-based technique is used to study the image-to-joint inverse kinematics of a tendon-driven supportive continuum arm. An eye-off-hand configuration is considered by mounting a camera at a fixed pose with respect to the inertial frame attached at the arm base. This camera captures an image for each distinct joint variable at each sampling time to construct the training dataset. This repository contains the implementation of the conference paper  <a href="https://doi.org/10.21428/d82e957c.d8706a7c"> **Image-to-Joint Inverse Kinematic of a Supportive Continuum Arm Using Deep Learning** </a> published in <a href="https://www.computerrobotvision.org/2024/"> Canadian Conference on Robot and Vision (CRV2024) </a>.

## Project Layout 

The project layout can be described as follows:

```
    ├── Scripts              # All Jupyter Notebook Files
    |
    ├── Dataset                 # Contains the images collected and the lables
    |   ├── imgs                # 999 RGB images collected
    |   ├── lables              # The joint variable
    |
    ├── Results                 # Result Directory
    
```

## Setup to create the dataset

As illustrated below, the SCCR comprises the operative (the arm on the left) and supportive arms (the arm on the right). Each arm consists of several elements: additional spacer disks for transmitting motor tensions to the tip flexible spring steel backbone, spacer disks made with PLA filament to guide the tendons, and four braided Kevlar lines serving as tendons. These tendons align along a circle with a radius of $18.55$ (mm), running parallel to the backbone. The manipulation of the tendons is done using Dynamixel servomotors AX-12A (Robotis, Lakeforest CA). 

<p align="center">
<img src="./results/CCR_Demo_Short.gif", width = "400" >
</p>

The block diagram of the entire data collecting setup is as follows:

<p align="center">
<img src="./results/setup.png", width = "1000" >
</p>

## Citation

I will be grateful if you cite my work in case you use this repository. 

```python


@article{Sepahvand2024Image,
	author = {Sepahvand, Shayan and Wang, Guanghui and Janabi-Sharifi, Farrokh},
	journal = {Proceedings of the Conference on Robots and Vision},
	year = {2024},
	month = {may 28},
	note = {https://crv.pubpub.org/pub/60urxy9p},
	publisher = {},
	title = {Image-to-{Joint} {Inverse} {Kinematic} of a {Supportive} {Continuum} {Arm} {Using} {Deep} {Learning}},
}
