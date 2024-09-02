# Neural Networks Project - Multi-ConDoS

#### Andrea Gervasio, matricola number: 1883259

Existing self-supervised medical image segmentation usually encounters the domain shift problem and/or the multimodality problem. To tackle these problems, the authors of the [paper](https://ieeexplore.ieee.org/document/10167829) *Multi-ConDoS: Multimodal Contrastive Domain Sharing Generative Adversarial Networks for Self-Supervised Medical Image Segmentation* propose multimodal contrastive domain sharing (Multi-ConDoS) generative adversarial networks. \\
The main idea is to fuse CycleGAN and the classic paired image translation model, Pix2Pix, to achieve better domain translation capability. The domain
sharing generative adversarial networks (DSGANs) also uses some shared layers to learn not only domain-specific but also domain-sharing information.

This notebook aims to reimplement this model using the PyTorch Lightning framework.
