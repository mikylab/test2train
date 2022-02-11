# Melanoma CNN Binary Classifer
A melanoma CNN classifer model built on the EffecientNet B3 model pretrained on imagenet and then retrained on images of benign and malignant lesions. This code trains the models on the ISIC 2020 dataset as well as indivual clinic subsets. The model only looked at images and did not take into account other features that were provided in the CSV files. 

This file consists of the original binary classifier that was trained to determine a baseline for performance on predicting classes of lesions. The EffecientNet_CNN_full_dataset uses the entire dataset from the ISIC 2020 challenge. Alternatively, the EffecientNet_CNN_Single_code contains the code to train a model on only a single clinic from the data. Both of these models use the pre-exisiting EfficientNet B3 Model trained on ImageNet and then use tranfer learning. The CNN_ROC file produces ROC curves to compare the results of a model's predictions and the ground truth. 

### Validation Results when training on the full dataset with no weights:
AUROC: .8535 

Sensitivity: TP / (TP+FN)
52/(52+79)=0.3969  

Specificity: TN / (TN + FP)
373/(373+79)=0.8252 

### Validation Results when training on the MSKCC dataset with no weights:
AUROC: .9322 

Sensitivity: TP / (TP+FN)
24/(24+19)=0.5581 

Specificity: TN / (TN + FP)
98/(98+3)=0.9703

### Validation Results when training on the BCN dataset with no weights:
AUROC: .8362 

Sensitivity: TP / (TP+FN)
19/(19+15)=0.5588  

Specificity: TN / (TN + FP)
90/(90+12)=0.8824 



---

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
https://github.com/haqishen/SIIM-ISIC-Melanoma-Classification-1st-Place-Solution/blob/master/dataset.py
