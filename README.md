# Image_Reconstruction

## Model Architecture

Tried implementing recurrent neural network (RNN) as BiLSTM, conditional GAN as Pix2Pix, & Context Encoder. Also, done inferencing of the pre-trained text-to-image diffusion model Stable Diffusion, for this image inpainting task.

## Dataset Description

The training dataset used in this project consists of images of four classes of animals, namely Cat, Dog, Elephant, and Tiger. For each class, there are two types of images - Masked and Unmasked. Every masked image in the dataset is a 256 x 256 image with precisely two masks which are squares of size 75 x 75. And for each category, there is a csv file named masked info.csv that contains information about the location of the masks (holes) in each image. Each unmasked image in the dataset is a complete image of size 256 x 256. In the test dataset, we have only 200 masked images of the same size as 256 x 256 with exactly two masks of the same size as 75 x 75. And there is exactly one csv file that contains the information about the location of the masks (holes) in all the 200 test-masked images.
