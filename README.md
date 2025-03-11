

[![DOI](https://zenodo.org/badge/331695371.svg)](https://zenodo.org/doi/10.5281/zenodo.10392182)
# Berkeley Single Cell Computational Microscopy Dataset

See the [project website](https://waller-lab.github.io/BSCCM/) and [paper](https://arxiv.org/abs/2402.06191) for more information.

For using the `bsccm` python package for using the dataset, see the [Getting Started Jupyter notebook](https://github.com/Waller-Lab/BSCCM/blob/main/Getting_started.ipynb).

Raw data is hosted [here](https://doi.org/10.5061/dryad.sxksn038s), but it is easiest to download using the python package as shown in the notebook

Clone the dataset given above and do the initial setup by using the Get Starter Jupyter notebook.




This project explores the application of generative AI in the field of fluorescence microscopy by generating synthetic images to enhance the quality and quantity of microscopic image datasets. The study leverages the Pix2Pix model, a conditional Generative Adversarial Network (GAN) architecture, to evaluate the efficiency of an existing input type and investigate the potential of a novel input type.

### Key Objectives

1. Generate synthetic fluorescence microscopy images using two distinct types of input images.

2. Evaluate the effectiveness of the Pix2Pix model in generating high-quality synthetic images.

3. Address data availability challenges in the medical domain by expanding datasets through generative AI.

4. Validate a newly published dataset of white blood cell microscopic images using a supervised model with two different input types.

### Methodology

- Data
  - We experiement this approach of generating synthetic images using two types of input data.
  - Approach 1: Input Brightfield Images to generate fluorescence images
  - Approach 2: Input Masked Fluorescence images where all channels except 1 will be masked in the input images. Here the channels are masked randomly, which means different input images will have a random combination of 5 out of 6 channels masked. The output fluorescence image generated will have all 6 channels that were input to the model.
 
    
Images of Brightfield images given as input
   <img width="990" alt="brightfield_images_input" src="https://github.com/user-attachments/assets/8d6f63e2-96a3-442e-b879-ac4053d82f0b" />
Images of fluorescence images given as reference to the model to generate output
  <img width="1010" alt="fluorescence_images from dataset" src="https://github.com/user-attachments/assets/69532f13-9592-4c5b-9503-5341985affc1" />



- Model Architecture: Utilized the Pix2Pix model, a conditional GAN designed for image-to-image translation tasks.
- Training & Validation: Conducted rigorous training and validation processes to assess the model’s performance with both input types.
- Dataset Augmentation: Focused on generating synthetic images from real fluorescence microscopy images to overcome data scarcity issues in medical imaging.

  
### Model pipeline

![image](https://github.com/user-attachments/assets/34ec58e9-b4aa-4622-8e85-cb96ee1a6b98)
![image](https://github.com/user-attachments/assets/2438eb32-f55f-4f08-a0ae-86792f065bce)

### Challenges Addressed

- Limited availability of medical imaging datasets due to confidentiality concerns and high costs associated with dataset creation.

- The need for reliable synthetic data to support advancements in medical imaging applications.

### Results

- Successfully generated high-quality synthetic fluorescence microscopy images using generative AI techniques.
- Demonstrated the potential of generative models like Pix2Pix in improving image quality and expanding medical imaging datasets.
- Validated the reliability of a newly published white blood cell microscopic image dataset, confirming its utility for supervised learning tasks.

### Impact

This project highlights how generative AI can play a transformative role in addressing data limitations in medical imaging by:

1. Enhancing dataset diversity and size without compromising confidentiality.

2. Supporting advancements in medical research and diagnostics through improved image quality.

### Technologies & Tools

1. Generative Adversarial Networks (GANs)

2. Pix2Pix Model

3. Python (Deep Learning Frameworks)

4. Fluorescence Microscopy Datasets

5. Supervised Learning Models

This study underscores the growing potential of generative AI in revolutionizing medical imaging applications while addressing critical challenges related to data availability and quality.




