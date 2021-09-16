# Binary Classifier
A melanoma classifier model built on the EffecientNet B3 model using transfer learning. 

This file consists of the original binary classifier that was trained to determine a baseline for performance on predicting classes of lesions. The EffecientNet_CNN_full_dataset uses the entire dataset from the ISIC 2020 challenge. Alternatively, the EffecientNet_CNN_Single_code contains the code to train a model on only a single clinic from the data. Both of these models use the pre-exisiting EfficientNet B3 Model trained on ImageNet and then use tranfer learning. The CNN_ROC file produces ROC curves to compare the results of a model's predictions and the ground truth. 
