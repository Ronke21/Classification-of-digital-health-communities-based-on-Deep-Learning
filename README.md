# Classification-of-digital-health-communities-based-on-Deep-Learning

## Introduction:

As part of the graduation project of the Deep Learning course,
We will carry out a research project in the field of health communities.
A database containing various Hebrew texts of health forums will be selected, and we will try to classify the medical community to which the texts belong.

**The classification will by by users and by texts - for 1 from 41 health communities!**

The classification  will be done using different models and we will compare the results:

1.   Random forest based on eigen vectors of the laplacian.
2.   Node2Vec based on random walks inside a LR model.
3.   GCN based on adjacency and feature matrix multiply - inside a LR model.
4.   RNN with pretraind embeddings by word2 vec.

## Final Results:

**The accuracy for classification of communities from a social network in healts topics:**

1.   Random forest based on eigen vectors of the laplacian:   **0.4585**
2.   Node2Vec based on random walks inside a LR model:    **0.1307**
3.   GCN based on adjacency and feature matrix multiply - inside a LR model:    **0.4887**
4.   RNN with Learning embeddings by word2 vec:  **0.5279**

![image](https://user-images.githubusercontent.com/73187207/198519190-6947c74d-5356-4416-9b53-295680db4dd6.png)


#### RNN with Learning embeddings is the BEST!


*   bigger dataset for better training and full picture (not only 2021)
*   doc2vec models - use uniqe hebrew features, parsing with morphological analysis
*   Laplacian eigen vectors - fine tune the results to ~48%
*   GCN - train a multy output logistic regression classifier
*   For the RNN&LSTM - try more epochs, different layers structure and sizes
*   try different models - CNN, Transformer
