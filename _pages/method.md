---
layout: single
title: Method
permalink: /method/

---

## Self-supervised labeling
![im]({{ site.url }}{{ site.baseurl }}/images/projected_wheel_tracks_2images.png)
  * Get vehicle trajectories from recorded GNSS/LiDAR data
  * Calculate wheel track contact points from vehicle trajectories
  * Project wheel track contact points to images as labels

## Image fusion
![im]({{ site.url }}{{ site.baseurl }}/images/Input_3d.png)
  * The RGB image and thermal image are downsampled to 512 x 512 pixels
  * Image alignment via a static homography transformation
  * Contrast Limited Adaptive Histogram Equalization (CLAHE) is applied to enhance the contrast of aligned images

## Encoder-decoder design
![im]({{ site.url }}{{ site.baseurl }}/images/neural_network_design.png)
  * Use ResNet-18 as backbone of encoder
  * Attention Gates focus on wheel tracks by amplifying rare pixel classes (addressing severe class imbalance).
  * Atrous Convolutions preserve boundaries with multi-scale context. (handling spatial imbalance).

## Model training and validation
  * 10 epochs with batch size of 4 and image size of 512 x 512
  * Adam optimizer with a learning rate schedule start at 1e-4
  * L2 regularizer

## Predicted probability map
![im]({{ site.url }}{{ site.baseurl }}/images/probability_map.png)
  * The designed neural network outputs a pixel-wise probability map
  * Each value ∈ [0,1] represents the predicted likelihood of the corresponding image pixel belonging to a wheel track

