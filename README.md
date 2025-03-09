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

In this work, a deep learning-based technique is used to study the image-to-joint inverse kinematics of a tendon-driven supportive continuum arm. An eye-off-hand configuration is considered by mounting a camera at a fixed pose with respect to the inertial frame attached at the arm base. This camera captures an image for each distinct joint variable at each sampling time to construct the training dataset. This repository contains the implementation of the conference paper  <a href="https://doi.org/10.21428/d82e957c.d8706a7c"> Image-to-Joint Inverse Kinematic of a Supportive Continuum Arm Using Deep Learning </a> published in <a href="https://www.computerrobotvision.org/2024/"> Canadian Conference on Robot and Vision (CRV2024) </a>.

## Real-world Setup
