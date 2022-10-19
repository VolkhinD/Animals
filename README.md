# Animals

This work is made for [Kaggle Dataset](https://www.kaggle.com/datasets/anshulmehtakaggl/wildlife-animals-images) 'Wild Animals' using PyTorch. So there are 2 ways of getting data and creating Torch Dataset in **Kaggle Notebook** and **Google Colab Notebook** \
I use --300-resized images and pretrained Resnet-18 model. \
In this work I'm playing with learning rate schedular and train model with 5 different ones:

* Train the whole model with constant learning rate
* Train the model with ***Step_lr shcedular***, so every N steps learning rate multiplied by gamma
* Train the model using ***Layer-Wise Learning Rate***. The key idea is to gradually reduce the learning rate when going deeper into the network.  
* Train the model with custom function using ***Lambda Shcedular***
* Train the model with ***ReduceLRonPlateau***. Reduce learning rate when a metric has stopped improving.

All methods work well, exept first one.
