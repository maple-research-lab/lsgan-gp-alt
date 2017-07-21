# LS-GAN-gp
This is the Tensorflow impementation of Ls-gan penalized with the gradient with respect to the input. 
Prerequsits:
-Python 2.7 or Python 3.3+
-Tensorflow 0.12.1
-SciPy
-pillow
Usage:
First download the data set using 
$ python download.py celebA
To train the network for CelebA dataset use the command :
$ python main.py --dataset celebA --input_height=108 --train --crop

This code has been written based on the Tensorflow impementation of DC-GAN coded by Taehoon Kim. 
