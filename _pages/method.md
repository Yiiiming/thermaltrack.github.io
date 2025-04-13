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
![im]({{ site.url }}{{ site.baseurl }}/images/image_fusion.png)
  * The RGB image and thermal image are downsampled to 512 x 512 pixels
  * Image alignment via a static homography transformation
  * Contrast Limited Adaptive Histogram Equalization (CLAHE) is applied to enhance the contrast of aligned images

## Encoder-decoder design
![im]({{ site.url }}{{ site.baseurl }}/images/neural_network_design.png)
  * Get vehicle trajectories from recorded GNSS/LiDAR data
  * Calculate wheel track contact points from vehicle trajectories
  * Project wheel track contact points to images as labels

## Model training and validation
  * Get vehicle trajectories from recorded GNSS/LiDAR data
  * Calculate wheel track contact points from vehicle trajectories
  * Project wheel track contact points to images as labels

## Predicted probability map
![im]({{ site.url }}{{ site.baseurl }}/images/probability_map.png)
  * Get vehicle trajectories from recorded GNSS/LiDAR data
  * Calculate wheel track contact points from vehicle trajectories
  * Project wheel track contact points to images as labels
