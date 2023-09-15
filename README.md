# Image_Reconstruction

## Model Architecture

Photo reconstruction is a challenging task in computer vision that aims to reconstruct high-quality images from incomplete or degraded inputs. It has various applications in fields such as satellite imagery, medical imaging, and artistic rendering. In recent years, deep learning models have been widely used for photo reconstruction tasks due to their ability to learn representations from large datasets and capture high-level features. 

Explored different deep neural networks such as BiLSTM, Pix2Pix, Context Encoder, and Stable Diffusion for reconstructing high-quality images from degraded inputs. The degraded inputs have missing pixels i.e. the inputs contain masks. Performed some experiments including fine-tuning to evaluate the performance of our models, and have analyzed the results.
Tried implementing recurrent neural network (RNN) as BiLSTM, conditional GAN as Pix2Pix, & Context Encoder. Also, done inferencing of the pre-trained text-to-image diffusion model Stable Diffusion, for this image inpainting task.

## Dataset Description

The training dataset used in this project consists of images of four classes of animals, namely Cat, Dog, Elephant, and Tiger. For each class, there are two types of images - Masked and Unmasked. Every masked image in the dataset is a 256 x 256 image with precisely two masks which are squares of size 75 x 75. And for each category, there is a csv file named masked info.csv that contains information about the location of the masks (holes) in each image. Each unmasked image in the dataset is a complete image of size 256 x 256. In the test dataset, we have only 200 masked images of the same size as 256 x 256 with exactly two masks of the same size as 75 x 75. And there is exactly one csv file that contains the information about the location of the masks (holes) in all the 200 test-masked images.
