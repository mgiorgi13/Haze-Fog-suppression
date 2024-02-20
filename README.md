# Haze-Fog-Suppression

## Overview

This project focuses on image dehazing using Generative Adversarial Networks (GANs). Leveraging the Atmospheric Scattering Model (ATSM), synthetic datasets, and the Pix2PixHD framework, we explore two models: a Single GAN model and a more complex Classifier + GAN model.

## Atmospheric Scattering Model (ATSM)

The ATSM provides a theoretical framework for understanding hazy image generation. It models the observed hazy image as the result of haze-free scene radiance attenuated by a transmission matrix and added with global atmospheric light.

## Dataset

Two datasets, M3FD and RESIDE SOTS, were used for training and evaluation. M3FD was utilized to create a synthetic dataset for training, while RESIDE SOTS served as a benchmark for evaluation.

## Pix2PixHD

Pix2PixHD, an advanced GAN framework, was employed for image-to-image translation tasks. It features a coarse-to-fine generator with global and local enhancers and multi-scale discriminators for high-resolution image synthesis.

## Models

Two models were developed: a Single GAN model and a Classifier + GAN model. The Classifier + GAN model incorporates VGG16 and InceptionV3 classifiers for fog level classification before applying the GAN.

## Results

Qualitative evaluation demonstrated significant improvement in image quality. Classifier comparisons using VGG16 and InceptionV3 showed excellent results on the M3FD dataset. However, poor results on RESIDE SOTS suggest parameter adjustments are needed.

## Usage
1. Clone the repository:
   ```
   git clone https://github.com/mattiadido95/Haze-Fog-Suppression.git
   ```
## Dependencies
- Python 3.x
- TensorFlow
- Keras
- Other required libraries (specified in code files)

## License
This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
We acknowledge the support and resources provided by Colab Pro during the training phase. Special thanks to the contributors to Pix2PixHD and the datasets used in this project.

Feel free to explore, contribute, or reach out for further collaboration!
