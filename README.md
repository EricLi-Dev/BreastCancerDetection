# BreastCancerDetection
![text](https://github.com/EricLi-Dev/BreastCancerDetection/blob/main/Images/4_categories.png)
Using CNNs to detect and classify breast cancer histology H&amp;E stained images

# Dataset
![text](https://github.com/EricLi-Dev/BreastCancerDetection/blob/main/Images/4_categories_figure.png)
https://iciar2018-challenge.grand-challenge.org/

The ICIAR 2018 Breast Cancer Histology dataset is from the ICIAR 2018 Grand Challenge on BreAst Cancer Histology (BACH) images for classifying H&E stained breast cancer histology microscopy images into four classes: normal, benign, in situ carcinoma, and invasive carcinoma. The training dataset consists of 100 images per category, making 400 H&E stained images (2048 x 1536 pixels) in TIF format. The entire dataset is ~10gb in size with each image being about 18mb. The image-wise annotation was performed by two medical experts. Another set of 100 images is included in the dataset for testing purposes, in addition to the training set.

# Project Proposal
https://docs.google.com/document/d/19sYryOWhEt3w2-aVUGKgPtFC7XYJKKGoQLJwBXDGkr8/edit?usp=sharing

# Approach
To build a deep learning image classifier to classify breast cancer histology images into Normal, Benign, In Situ Carcinoma, and Invasive Carcinoma with ResNet, VGG, and Inception architectures. 

Build Local-Patch and Global-Patch features on H&E normalized images
Leverage both unsupervised and supervised transfer learning on VGG, ResNet, and Inception for feature extraction

(1) Unsupervised Feature Extraction on Normalized Images
(2) Unsupervised Feature Extraction on Local/Global Patches
(3) Supervised Feature Extraction on Local/Global Patches

Use KNNs, SVMs, and XGBoost for classification predictions. 
Compare the performance of a CNN-based architecture for feature extraction 

# Best Results
- Best 2 Class Carcinoma Accuracy:
  Local/Global Patches + Unsupervised ResNet50 Feature Extraction + SVM -> 0.93
- Best Average Accuracy:
  Local/Global Patches + Supervised VGG16 Feature Extraction + XGBoost -> 0.81
  
# Referenced Papers:
[1]. Rakhlin, Alexander, et al. "Deep convolutional neural networks for breast cancer histology image analysis." Image Analysis and Recognition: 15th International Conference, ICIAR 2018, Póvoa de Varzim, Portugal, June 27–29, 2018, Proceedings 15. Springer International Publishing, 2018.
[2] Nazeri, Kamyar, et al. “Two-Stage Convolutional Neural Network for Breast Cancer Histology Image Classification.” Lecture Notes in Computer Science, 2018, pp. 717–726, https://doi.org/10.1007/978-3-319-93000-8_81. 
[3] Macenko, Marc, et al. “A Method for Normalizing Histology Slides for Quantitative Analysis.” 2009 IEEE International Symposium on Biomedical Imaging: From Nano to Macro, 2009, https://doi.org/10.1109/isbi.2009.5193250. 

