[TOC]



## Classical CNN
**Fully Convolutional Networks for Semantic Segmentation [FCN](https://arxiv.org/pdf/1411.4038)**
* End-to-end, pixel to pixel CNN segmentations, a down-sampling step, and a up-sampling step for segmentation.

**Rich feature hierarchies for accurate object detection and semantic segmentation [RCNN](https://arxiv.org/pdf/1311.2524)**
* For each image, generate ~2k random regions and feed each to CNN and use SVM for classification. Usually is slow.

**Fast R-CNN [Fast R-CNN](https://arxiv.org/pdf/1504.08083)**
* Use the full image and choose the related region for the region of interest, and convert the region feature to a fixed size feature. Use softmax for every ROI. 

**Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks [Faster R-CNN](https://arxiv.org/pdf/1506.01497)**
* Use a network to generate proposed anchors as the ROI, and output bbox and classification.

**You Only Look Once: Unified, Real-Time Object Detection [YOLO](https://arxiv.org/pdf/1506.02640)**
* End-to-end, no region proposal, segment the image as S \times S, and each patch is responsible for generate the bbox of the object, centering at the patch.


**YOLO9000: Better, Faster, Stronger [YOLOv2](https://arxiv.org/pdf/1612.08242)**
* Use k-mean on labeled data find better anchor shapes. Use sigmoid estimating the shift of left top corner of the patch to the anchor center. 

**YOLOv3: An Incremental Improvement [YOLOv3](https://arxiv.org/pdf/1804.02767)**
* Change network structure, change softmax to multiplease logistic for multi-labels.



## Self-supervised Learning
**Emerging Properties in Self-Supervised Vision Transformers [DINO](https://arxiv.org/pdf/2104.14294)**
* A teacher model and a student model with same architecture. Crop one image into two different size and feed to teacher and student model, teacher model has extra batch center step, and try to align the distributions. Can capture the main part of the images.



## Efficiency and Optimization
**Token Merging: Your ViT But Faster [paper](https://arxiv.org/pdf/2210.09461)**
* On every layer, use matching method to merge a fixed number of tokens, use the key vector than the feature vector.




## Generative Models

**Denoising Diffusion Probabilistic Models [diffusion](https://arxiv.org/pdf/2006.11239)**
* each step add a small noise until the image becomes pure noise. And recover step is denoising.





## Segmentation

**Deciphering ‘What’ and ‘Where’ Visual Pathways from Spectral Clustering of Layer-Distributed Neural Representations [paper](https://arxiv.org/pdf/2312.06716)**

* Using Laplacian matrix for segmentation, replacing the elements with Q,K,V, from the attentions.