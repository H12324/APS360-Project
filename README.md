# APS360-Project
Machine Learning for APS360

This project looks to create an CNN based autoencoder model using several techniques such as residual connections and instance awareness. 

A landscape dataset from kaggle is used for the same. We pre-process images to 128 x 128 with padding or crop, and use the LAB color space. The pre-processed image is saved as a numpy array which is used to train the model using a custom DataLoader. 

We use a UNET style architecture for the autoencoder with a CSPDarknet52 object detection backbone (pretrained) embedding fused to the model at the bottleneck. 

PSNR Loss is predominantly used for training.

Several helper functions such as quick_qualitative, to_rgb and various others can be found in the notebook too.
