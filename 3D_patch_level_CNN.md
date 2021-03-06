## Classification of MR brain images by combination of multi-CNNs for AD diagnosis (2017)
> [`paper`](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/10420/1042042/Classification-of-MR-brain-images-by-combination-of-multi-CNNs/10.1117/12.2281808.short?SSO=1)
### **Dataset**
> - MRI
### **Training**
> - 2 class classification (AD/CN)
> - Extract multiple local patches
> - Pre-training each CNN
> - Combine each CNN with Fully Connected(FC) layer and fine-tuning
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/00_model1.PNG" width="700"/>  
### **Result**
> - Comparison of different method
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/00_result1.PNG" width="500"/>
---
#
#
#
## Multi-modality cascaded convolutional neural networks for Alzheimer’s disease diagnosis (2018)
> [`paper`](https://link.springer.com/article/10.1007/s12021-018-9370-4)
### **Dataset**
> - MRI, PET
### **Training**
> - 2 class classification (AD/CN, pMCI/CN, sMCI/CN)
> - Divide into 3x3x3 size from whole brain image --> extract 27 patches
> - Extract feature with 3D ConvNet
> - Combined feature vector of MRI and PE
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/02_model1.PNG" width="700"/>  
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/02_model2.PNG" width="700"/>
### **Result**  
> - Comparison of different method
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/02_result1.PNG"/>
---
#
#
#
## Alzheimer's disease diagnosis based on multiple cluster dense convolutional networks (2018)
> [`paper`](https://www.sciencedirect.com/science/article/abs/pii/S089561111830199X)
### **Dataset**
> - MRI
### **Training**
> - 2 class classification (AD/CN, MCI/CN)
> - Find the groups of patches by K-means clustering (32x32x32 size)
> - Reduce feature dimension by PCA (32x32x32 --> 2000 dim)
> - Fine-tuning pre-trained 3D DenseNet
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/03_model1.PNG" width="700"/>  
### **Result**  
> - Comparison of different model
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/03_result1.PNG" width="700"/>

> - Comparison of different feature extraction
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/03_result2.PNG" width="700"/>
---
#
#
#
## Hierarchical Fully Convolutional Network for Joint Atrophy Localization and Alzheimer's Disease Diagnosis using Structural MRI (2018)
> [`paper`](https://ieeexplore.ieee.org/document/8585141)
### **Dataset**
> - MRI
### **Training**
> - 2 class classification (AD/CN, pMCI/sMCI)
> - Data Augmentation (random flipping, ditorting, shifting)
> - Process each patch by patch-level sub-networks (shared parameter) and concat each ouput feature
> - Repeat feature encoding by region-level and subject-level networks
> Delete uninformative sub-networks (Network Pruning)
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/04_model1.PNG" width="800"/>  

> - Hybrid loss function (cross entropy with patch-/region-/subject-level networks)
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/04_loss1.PNG" width="500"/>
### **Result**  
> - Comparison of different model
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/04_result1.PNG"/>

> - Visualize patch-, region-level locations
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/04_vis1.PNG" width="600"/>
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/04_vis2.PNG" width="600"/>
---
#
#
#
## Anatomical landmark based deep feature representation for MR images in brain disease diagnosis (2018)
> [`paper`](https://ieeexplore.ieee.org/abstract/document/8253440)
### **Dataset**
> - MRI
### **Training**
> - 2 class classification (AD/CN)
> - Find landmark locations and projected to images
> - Extract patches from each landmark locations and learn features
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/05_model1.PNG" width="700"/>  
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/05_model2.PNG" width="700"/>
### **Result**  
> - Comparison of different model
> <img src="https://github.com/SSinyu/Alzheimer-Prediction-Review/blob/master/img/3D_patch_level_CNN/05_result1.PNG"/>
