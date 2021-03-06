# Deep Joint Depth Estimation and Color Correction from Monocular Underwater Images based on Unsupervised Adaptation Networks

This repo implements the training and testing of unsupervised adaptation networks for "Deep Joint Depth Estimation and Color Correction" by Xinchen Ye, Zheng Li, and et al. at DLUT.

Specifically, a style adaptation network (SAN) is first proposed to learn a style-level transformation to adapt in-air images to the style of underwater domain. Then, we formulate a task network (TN) to jointly estimate the scene depth and correct the color from a single underwater image by learning domain-invariant representations.

## The framework of style adaptation network (SAN) and task network (TN).

![](https://github.com/DLUT-ZhengLi/DESN-CCSN/blob/master/images/frame.png)

## The detailed framework of task network (TN).

<img src="https://github.com/DLUT-ZhengLi/DESN-CCSN/blob/master/images/TNframe.png"  width="500" height="500">

Our stacked conditional GANs architecture for joint depth estimation and color correction. Gc is sketched out briefly and the domain adaptation modules on both generators are omitted for saving space.


## Results
![](https://github.com/DLUT-ZhengLi/DESN-CCSN/blob/master/images/SAN.png)

*Fig. 1. Evaluation on SAN from the perspective of training details and rendering results. (a) and (b) show the loss curves of training process from WaterGAN and ours. (c-e) present three visual examples for clearly observing the rendering results. From top to bottom are the results from WaterGAN, ours, and the real underwater images, respectively.*

![](https://github.com/DLUT-ZhengLi/DESN-CCSN/blob/master/images/TN.png)

*Fig. 2. Qualitative comparison on real underwater images under different module configurations: (a)DESN or CCSN separately; (b) DESN + CCSN, (c) DESN with DA + CCSN, (d) DESN with DA + CCSN with DA, (e) DESN + CCSN with DA. The depth maps are colored with red for farther distance, while blue for closer distance. We use red rectangles to direct readers to focus on those specific areas to compare the difference under different cases.*

![](https://github.com/DLUT-ZhengLi/DESN-CCSN/blob/master/images/TN2.png)

*Fig. 3. Qualitative comparison of depth estimation on real underwater images: (a) underwater images; Results estimated by (b) Laina et al. , and (c) Ours.*

![](https://github.com/DLUT-ZhengLi/DESN-CCSN/blob/master/images/TN3.png)

*Fig. 4. Qualitative comparison of color correction on real underwater images: (a) underwater images. Results recovered by (b) FIP , (c) CBF , (d) R-cycle , (e) Pix2Pix , and (f) Ours.*

## Dependences

Python 2.7.14 

conda 4.3.30

Tensorflow 1.8.0

## Open Source

The source code, trained model, and some results will be available on the github if well prepared.

## Citation 
If you find this code useful, please cite:

` Xinchen Ye* et al., Deep Joint Depth Estimation and Color Correction from Monocular Underwater Images based on Unsupervised Adaptation Networks. `


