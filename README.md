# Neural Networks Project - Multi-ConDoS

#### Andrea Gervasio, matricola number: 1883259

Existing self-supervised medical image segmentation usually encounters the domain shift problem and/or the multimodality problem. To tackle these problems, the authors of the [paper](https://ieeexplore.ieee.org/document/10167829) *Multi-ConDoS: Multimodal Contrastive Domain Sharing Generative Adversarial Networks for Self-Supervised Medical Image Segmentation* propose multimodal contrastive domain sharing (Multi-ConDoS) generative adversarial networks. 

The main idea is to fuse CycleGAN and the classic paired image translation model, Pix2Pix, to achieve better domain translation capability. The domain sharing generative adversarial networks (DSGANs) also uses some shared layers to learn not only domain-specific but also domain-sharing information.

This notebook aims to reimplement this model using the PyTorch Lightning framework.

# Instructions

The notebook has been tested on Google Colab using a free subscription. Make sure that the runtime is set on T4 GPU before running. 

The user is not required to do anything, the code will handle the installation of the necessary libraries and the downloads of the data. If the user is interested in logging the training results on the Weights and Biases platform, they should look for the definition of the `log_wandb` parameter in Section 0.
