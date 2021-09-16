# Binary Classifier
A melanoma classifier model built on the EffecientNet B3 model using transfer learning. 

This file consists of the original binary classifier that was trained to determine a baseline for performance on predicting classes of lesions. The EffecientNet_CNN_full_dataset uses the entire dataset from the ISIC 2020 challenge. Alternatively, the EffecientNet_CNN_Single_code contains the code to train a model on only a single clinic from the data. Both of these models use the pre-exisiting EfficientNet B3 Model trained on ImageNet and then use tranfer learning. The CNN_ROC file produces ROC curves to compare the results of a model's predictions and the ground truth. 


#### Code Starters Used/Adapted: 

ImageGenerator that works with Albumentations:
https://github.com/mjkvaak/ImageDataAugmentor/blob/master/ImageDataAugmentor/image_data_augmentor.py

Custom efficientNet:
https://github.com/qubvel/efficientnet

Kaggle Melanoma Starter Code:
https://www.kaggle.com/hyunkic/melanoma-cnn-approach-imgen

Albumentations Augmentation Library:
https://pypi.org/project/albumentations/#spatial-level-transforms

SIIM ISIC Melanoma Classification 1st place solution- augmentations used 
https://github.com/haqishen/SIIM-ISIC-Melanoma-Classification-1st-Place-Solution/blob/master/dataset.py![image](https://user-images.githubusercontent.com/43506570/133662420-56e6a166-a21c-47df-82a8-c6e04d6523d5.png)
