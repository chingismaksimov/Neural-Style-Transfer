# Neural-Style-Transfer
This is an implementation of Neural Style Transfer Algorithm first proposed by Gatys et al. (2016). Given two input images, the algorithms applies the style of one of the images to the contents of the other. The two input images are known as style image and content image, respectively. As the content image for this project, we chose a random picture of a city. As the style image, we choose *Starry Night* by Vincent van Gogh. This is not a particularly original choice of the style image but it works quite well. The two input images are saved in img/input folder. 

The successful application of the algorithm requires a neural network that can provide good feature representation of the input images. Given time and computational constraints, we made use of the pretrained VGG-19 network available from torchvision package. We used Adam optimizer with a learning rate of 0.005 and MSE as the loss function. 

The training was done over 3,000 epochs. The training progress along with the generated images are saved in img/output folder. 

# References
 L. A. Gatys, A. S. Ecker, and M. Bethge, “Image style transfer using convolutional neural networks,” in *Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition*, 2016, pp. 2414–2423.
