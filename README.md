# Densefuse: A Fusion Approach for Infrared and Visible Image Fusion
Infrared and visible image fusion using CNN layers and dense block architecture.

## Abstract
In this paper, we present a novel deep learning architecture for infrared and visible images fusion problem. 

In contrast to conventional convolutional networks, our encoding network is combined by convolutional neural network layer and dense block which the output of each layer is connected to every other layer. We attempt to use this architecture to get more useful features from source images in encoder process. Then appropriate fusion strategy is utilized to fuse these features. Finally, the fused image is reconstructed by decoder. 

Compare with existing fusion methods, the proposed fusion method achieves state-of-the-art performance in objective and subjective assessment.

### The framework of fusion method
![](https://github.com/exceptionLi/imagefusion_densefuse/blob/master/figures/framework.png)

### Training process
![](https://github.com/exceptionLi/imagefusion_densefuse/blob/master/figures/train.png)

### Fusion strategy - addition
![](https://github.com/exceptionLi/imagefusion_densefuse/blob/master/figures/fuse_addition.png)

### Fusion strategy - l1-norm
![](https://github.com/exceptionLi/imagefusion_densefuse/blob/master/figures/fuse_l1norm.png)


## Experimental Setting

We train our network using MS-COCO as input images which contains 80000 images and all resize to 256×256 and RGB to gray. Learning rate is 1×10^(-4).The batch size and epochs are 2 and 4, respectively. Our method is implemented with GTX 1080Ti and 64GB RAM.

If you have any question about this code, feel free to reach me(hui_li_jnu@163.com)
