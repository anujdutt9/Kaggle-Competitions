# Flower Classification TPU

This folder contains the experiments for training a deep learning model for classifying 104 types of flowers using a TPU. Various models and approaches have been tried in these notebooks.

# Kaggle Competition

https://www.kaggle.com/c/flower-classification-with-tpus/overview

# Approaches

|       Notebook        |                       Description                       |
| --------------------- | ------------------------------------------------------- |
|[vgg-flower-classification-tpu.ipynb](https://github.com/anujdutt9/Kaggle-Competitions/blob/master/Flower-Classification-TPU/vgg-flower-classification-tpu.ipynb)| Baseline kernel using random left, right flip for image augmentation and pre-trained VGG-16 model. |
|[vgg-cutout-flower-classification-tpu.ipynb](https://github.com/anujdutt9/Kaggle-Competitions/blob/master/Flower-Classification-TPU/vgg-cutout-flower-classification-tpu.ipynb)| Baseline kernel with random left, right, up, down flip, random brightness and CutOut augmentations, with pre-trained VGG-16 model. |
|[efficientnetb7-densenet-ensemble.ipynb](https://github.com/anujdutt9/Kaggle-Competitions/blob/master/Flower-Classification-TPU/efficientnetb7-densenet-ensemble.ipynb)| Added CutOut, rotation, shear x and y to augmentations, with an ensemble of pre-trained EfficientNet-B7 and DenseNet-121 models.|

# Final Score

![Output](Flower-Classification-TPU/EfficientNet-DenseNet-Ensemble.png "Output")
![Output](EfficientNet-DenseNet-Ensemble.png "Output")

# References

1. Baseline Kernel: https://www.kaggle.com/mgornergoogle/getting-started-with-100-flowers-on-tpu
2. CutOut from TensorFlow Addons: https://colab.research.google.com/drive/1m-3EKvK9Th9rRTDPytlv59TUgPYipxlr?usp=sharing#scrollTo=KeIF8mYH0joq
3. Flower Classification with CutMix and Mixup: https://www.kaggle.com/cdeotte/cutmix-and-mixup-on-gpu-tpu
4. Rotation Augmentation: https://www.kaggle.com/cdeotte/rotation-augmentation-gpu-tpu-0-96
5. Model Ensemble: https://www.kaggle.com/zenerdiode818/flower-8-3-20/notebook
