# cycleGan-classifier
A melanoma classifier with a cycleGan to improve the classification results. 

The use of convolutional neural networks (CNNs) has allowed for the classification of images into different classes. However, a limitation of CNNs is that they are only reliable on images that are within their domain. Image augmentation tactics have been employed to diversify the domain and prevent overfitting, but when a model is trained on a specific domain and then tested on another domain the model does not achieve the same Area Under the Receiver Operating Characteristic Curve (AUROC). The misclassification of images outside of the domain, specifically for melanoma, was investigated in this article [Stress Testing Reveals Gaps in Clinic Readiness of Image-Based Diagnositc Artificial Intelligence Models](https://www.nature.com/articles/s41746-020-00380-6). 

As an attempt to try to solve the out of domain classification problem, CNN classification models were first trained on images from one domain (ISIC 2020 Barcelona Clinic and Memorial Sloan Kettering Cancer Center) and then tested on images from another domain. The classification models were trained on a smaller subset of the larger data in order to solve the class imbalance. 

![BCN ROC](https://github.com/mikylab/cycleGan-classifier/blob/63d449907f4838e506d9634589fcc5eaa671d852/resources/BCN%20Small%20Dataset%20ROC.png)![MSKCC ROC](https://github.com/mikylab/cycleGan-classifier/blob/f37f69f19a92ce8fde45010bfd3a30fb5d74c675/resources/MSKCC%20Small%20Dataset%20ROC.png)
