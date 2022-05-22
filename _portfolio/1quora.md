---
title: "Insincere question classification witih BiLSTM and Attention"
excerpt: "2018"
collection: portfolio
---

For my `Classification and Clustering` subject in my Master's Degree, I developed an algorithm to detect insincere questions in Quora. I did an [EDA](https://www.kaggle.com/anebzt/quora-eda) first to explore the data, and then another [notebook](https://www.kaggle.com/anebzt/quora-preprocessing-model) with the preprocessing with pretrained embeddings and the BiLSTM model with one Attention layer:

```
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
input_1 (InputLayer)         (None, 40)                0         
_________________________________________________________________
embedding_1 (Embedding)      (None, 40, 300)           30000000  
_________________________________________________________________
bidirectional_1 (Bidirection (None, 40, 128)           187392    
_________________________________________________________________
bidirectional_2 (Bidirection (None, 40, 64)            41472     
_________________________________________________________________
attention_1 (Attention)      (None, 64)                104       
_________________________________________________________________
dense_1 (Dense)              (None, 32)                2080      
_________________________________________________________________
dropout_1 (Dropout)          (None, 32)                0         
_________________________________________________________________
dense_2 (Dense)              (None, 1)                 33        
=================================================================
Total params: 30,231,081
Trainable params: 231,081
Non-trainable params: 30,000,000
_________________________________________________________________
```

Given a trainset of 1.3M questions and a testset of 50k questions, with just 6% of insincere questions, this pipeline achieved a F1-score of 0.66. The highest in the competition achieved a F1-score of 0.71, and employed model stacking or even BERT. 