As this is an assignment on GAN, hyperparameters like no. of epochs and architectural choices matter, choose them wisely, this will impact your results - refer to slide no.17 in this link on architectural guidelines. 
Questions:- 
1. [Noise to Image Generation] 
Train a DCGAN to generate images from noise. Use the MNIST database to learn the GAN network. 
[Discriminator in DCGAN:- 
i. if roll no. % 2 == 0: use VGG16 as a discriminator. 
ii. if roll no. % 2 == 1: use Resnet 18 as a discriminator.] 
Perform the following tasks: [35 marks for training GAN] 
b. Uniformly generate ten noise vectors that act as latent representation vectors, and generate the images for these noise vectors, and visualize them at [5 + 5 + 5 marks] 
i. After the first epoch. 
ii. After n/2th epoch.
iii. After your last epoch. (say n epochs in total) 
and comment on the image interpretation at (i), (ii) and (iii), can you identify the images? Pass these images generated at each epoch to the model you’ve trained in Assignment - 2 (Q1) and report their predictions with confidence scores. Comment on them. [5 + 15 marks] 
c. Plot generator and discriminator losses for all the iterations. [One iteration = forward pass of a mini-batch] [10 marks] 
d. [Bonus] Do we have control of what class image the generator will generate, given a noise vector? Suppose, we are interested in generating only “4” images, will the GAN you trained in (a) can do that? Explain why. If not, modify the GAN trained above to do this. [10 + 40 marks] 
2. [Image to Image Translation] 
Your task is to train a GAN that generates maps given satellite images. [Dataset Link]. [40 marks for training GAN] 
a. Report visualized image translations [satellite image -ground truth map - map generated]. [at least 10 examples] [10 marks] 
b. Plot generator and discriminator losses for all the iterations. [One iteration = forward pass of a mini-batch]. [10 marks] 
c. Use the pre-trained sat2map generator model from here [Pytorch - Link, TensorFlow - Link] and generate images for the same ten examples in (a). Compare and comment on the images generated with a pre-trained generator with your trained generator in (a). Support your claim with SSIM. [15 + 5 marks] 
3. Choose any GAN paper from top venues (with h5-index > 50, for example, CVPR, ECCV, ICCV, ICML, etc.) in the last two years [2019-20] [Reference:- https://github.com/hindupuravinash/the-gan-zoo], reproduce the results in the paper. You can use the authors’ code (mostly provided via GitHub) or any other reimplementation available on the internet. [Please cite the source]. You should be able to understand and explain the code that you are using. [80 marks]
