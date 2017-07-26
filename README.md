# Loss-Sensitve GAN With Gradient Penalty

This is the Tensorflow impementation of LS-GAN penalized with the gradient with respect to the input. IT has been implemented based on the DC-GAN implementation by Taehoon Kim.

Please cite the following paper when referring to the following algorithms:

**Guo-Jn Qi. Loss-Sensitive Generative Adversarial Networks on Lipschitz Densities. arXiv:1701.06264 [[pdf](https://arxiv.org/abs/1701.06264)]**

## Reference

### LS-GAN

Code: https://github.com/guojunq/lsgan

Paper: https://arxiv.org/pdf/1701.06264

The implementation follows the idea of gradient penalty proposed originally in the first version of LS-GAN, Chapter 5 [[pdf](https://arxiv.org/pdf/1701.06264v1.pdf)], quoted here
"Alternatively, one may consider to directly minimize
the gradient norm ||∇xLθ(x)|| as a regularizer for
the LS-GAN. In this paper, we adopt weight decay for its
simplicity and find it works well with the LS-GAN model
in experiments."


## Usage
The code has been written in Tensorflow. Following is the list of prerequisites

### Prerequisites

-Python 2.7 or Python 3.3+ 

-Tensorflow 0.12.1 

-SciPy 

-pillow Usage
### Data-Set
Change the directory to LS-GAN-GP directory.
You can download the CelebA data-set using command:  
```
$ python download.py celebA
```

### Training Model
To train the network for CelebA dataset use the command  
```
$ python main.py --dataset celebA --input_height=108 --train --crop
```

During the training process the snapshot of the models are saved in folder called **checkpoint** and generated samples in folder called **samples** 
### Results

### 1 epoch
![alt text](https://github.com/MarziEd/LS-GAN-gp/blob/master/results/train_00_3099.png)

### 3 epoch
![alt text](https://github.com/MarziEd/LS-GAN-gp/blob/master/results/train_03_3103.png)

### 4 epoch
![alt text](https://github.com/MarziEd/LS-GAN-gp/blob/master/results/train_04_3138.png)

### 10 epoch
![alt text](https://github.com/MarziEd/LS-GAN-gp/blob/master/results/train_10_3148.png)

### 24 epoch
![alt text](https://github.com/MarziEd/LS-GAN-gp/blob/master/results/train_24_3138.png)

