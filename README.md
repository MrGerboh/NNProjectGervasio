# Neural Networks Project - Multi-ConDoS

### Andrea Gervasio, matricola number: 1883259

Existing self-supervised medical image segmentation usually encounters the domain shift problem and/or the multimodality problem. To tackle these problems, the authors of the [paper](https://ieeexplore.ieee.org/document/10167829) *Multi-ConDoS: Multimodal Contrastive Domain Sharing Generative Adversarial Networks for Self-Supervised Medical Image Segmentation* propose multimodal contrastive domain sharing (Multi-ConDoS) generative adversarial networks. 

The main idea is to fuse CycleGAN and the classic paired image translation model, Pix2Pix, to achieve better domain translation capability. The domain sharing generative adversarial networks (DSGANs) also uses some shared layers to learn not only domain-specific but also domain-sharing information.

This notebook aims to reimplement this model using the PyTorch Lightning framework.

# Instructions

The notebook has been tested on Google Colab using a free subscription. Make sure that the runtime is set on T4 GPU before running. 

Since it appears that the *.ipynb* file does not display correctly the images inside, I will leave the link to the Google Colab notebook [here](https://colab.research.google.com/drive/1PgNSfQHqeAwFhQo1M4Pdr4G5RvQ9Kxa0?usp=sharing).

The user is not required to do anything, the code will handle the installation of the necessary libraries and the downloads of the data. If the user is interested in logging the training results on the Weights and Biases platform, they should look for the definition of the `log_wandb` parameter in Section 0.

# Results

The notebook will save the weights of the trained and the finetuned model, as well as the masks generated after the finetuning process. For easy access, they can also be found in [this](https://drive.google.com/drive/folders/1IkqiZmgY8VJyWm1ZDaK6d5-7kIijSxFa?usp=sharing) Google Drive folder.

Below are reported the losses logged during training and finetuning:

### Training Losses:

![](https://drive.google.com/uc?export=view&id=1Wwi8cAlQSyI0mNg9t1LbDHrVfdze9qAC)

![](https://drive.google.com/uc?export=view&id=12g1zjyqBFOSP7uJrYrBdqcjRTZsVWMPV)

![](https://drive.google.com/uc?export=view&id=1luA-iOYR1DwQ48rmXQh1kv4kQu-PVStv)

### Finetuning Losses:
![](https://drive.google.com/uc?export=view&id=10-gS-bLNJjm76DNJjpz5IOyHn2bP_xq5)

![](https://drive.google.com/uc?export=view&id=19OLTxxCKzi6dJmF2N6KAJVRMqh228HJq)

![](https://drive.google.com/uc?export=view&id=1LpMyYycKcox5POFiMiFh13hGQHpeWKhw)

![](https://drive.google.com/uc?export=view&id=1EnvsapIX44GS6B2CZwpfONGldOfPS1wc)

### Generated masks:

Example of generated masks can be found here

![mask_24](https://github.com/user-attachments/assets/985f545b-0867-4fc5-b678-6187942c5302) ![mask_268](https://github.com/user-attachments/assets/7f98b3ed-a48e-4066-b6bc-900371877007) ![mask_575](https://github.com/user-attachments/assets/c73a01da-661e-49db-a026-49823d9d595f)

