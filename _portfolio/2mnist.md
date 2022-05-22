---
title: "CNN implementation on MNIST dataset in Keras"
excerpt: "2018"
collection: portfolio
---

In my summer job on 2018 I researched CNNs for image classification extensively and I decided to create a detailed explanatory notebook on my [Kaggle account](https://www.kaggle.com/anebzt/mnist-with-cnn-in-keras-detailed-explanation) with what I had learnt in the process, advice on hyperparameter tuning, failures and successes, what works best in each case based on my experience... and hoping to make the steep curve smoother to beginners. I referenced insightful code snippets from other kernels and included detailed explanations aimed at people implementing a classification model for the first time. At the time of writing, it has been forked 72 times.

I used a quite small CNN model for this task:

```
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_1 (Conv2D)            (None, 28, 28, 32)        832       
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 28, 28, 32)        25632     
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 14, 14, 32)        0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 14, 14, 32)        0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 14, 14, 64)        51264     
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 14, 14, 64)        102464    
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 7, 7, 64)          0         
_________________________________________________________________
dropout_2 (Dropout)          (None, 7, 7, 64)          0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 3136)              0         
_________________________________________________________________
dense_1 (Dense)              (None, 120)               376440    
_________________________________________________________________
dense_2 (Dense)              (None, 84)                10164     
_________________________________________________________________
dense_3 (Dense)              (None, 10)                850       
=================================================================
Total params: 567,646
Trainable params: 567,646
Non-trainable params: 0
_________________________________________________________________
```