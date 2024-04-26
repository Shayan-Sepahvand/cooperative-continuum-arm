# Image-to-shape supportive continuum arm dataset

The goal of this project is to solve the inverse kinematics of the supportive continuum arm presented in https://www.computerrobotvision.org/, in Guelph, Ontario, Canada in May 28th.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset Details](#dataset-details)
3. [Usage](#usage)
4. [Contributing](#contributing)
5. [License](#license)

## Introduction

This dataset contains 999 RGB images and 999 joint variable stored in a txt file. The images are names from 1 to 999, and the lables in the text file are ordered the same. For example, lable #1 corresponds to image 1.jpg.

## Dataset Details

Dataset Specifications
- **Size**: 43.2 MB
- **Format**: images are stored as jpeg and the labels are stored in a text file.
- **Source**: https://drive.google.com/file/d/1cS0kaeGU7AD2bTIyMSXwhqMtkYZi-ATi/view?usp=drive_link
- **Preprocessing**: No preprocessing required. 

## Usage

[Explain how to use your dataset. Provide examples of how to load and analyze it using popular data processing libraries or tools.]

### Example:

```python
import pandas as pd

# Load the dataset
data = pd.read_csv('dataset.csv')

# Display the first few rows
print(data.head())

