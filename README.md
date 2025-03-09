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

## Real-world Setup
<p align="center">
<img src="./results/CCR_Demo_Short.gif", width = "200" >
</p>

<!-- ## Project Layout 

To ease the implementation of different learning models and kinematic models, the project is structured in the following manner - 

```
    .
    ├── Scripts              # All Jupyter Notebook Files
    │   ├── INN                 # Inverible Neural Networks
    │   |── RBF                 # Radial Basis Functions
    │   ├── MLP                 # Multi-Layer Perceptron
    │   ├── ELM                 # Extreme Learning Machine
    │   └── Cascade_Correlatin  # Cascade Correlation
    |
    ├── Dataset                 # Contain the workspace generated using different models as a pkl file
    |
    ├── Models                  # Kinematic Robot Models
    │   ├── PCC                 # Piecewise Constant Curvature Model
    │   └── Static              # Static Model based on cosserat rod theory and string theory
    |
    ├── Results                 # Result Directory
    │   ├── Training            # All the learning models are stored as sav file
    │   ├── Trajectory          # Stores the trajectory output from learning models
    │   └── Workspace           # Snipet of workspace generated using Kinematic Models
    |
    ├── main.py.                # Main program to train different learning models
    └── trajectory.py           # Test the trained model on different trajectories
    
``` -->

## Citation

I will be grateful if you cite my work if you use this repository. 

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