# SRGAN + Flow Loss
## W4731 Computer Vision Final Project: Video Superresolution

In this project, a loss function to improve upon the baseline approach which simply applies image supperresolution to each frame will be proposed. Based on the [SRGAN](https://github.com/tensorlayer/srgan) proposed by [Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network](https://arxiv.org/abs/1609.04802), we propose a novel specific loss function which does not take only one single frame but a bundle of temporally neighbouring frames into the GAN. The model takes a sliding window of several consecutive frames as the input for generator network and outputs a bundle of consecutive SR frames. A perceptual loss function regarding both the single frame superresolution quality and the temporal continuity is proposed and the experimental results will evaluate the quality of superresolved videos using this loss function.