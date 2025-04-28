---
layout: single
title: Safety_testing
permalink: /safety_testing/

---

![im]({{ site.url }}{{ site.baseurl }}/images/image_000203.png)

## [CODMAX](https://yimingyang-mtu.github.io/profilo.github.io/codmax)
  We utilize WADS, a specialized dataset designed for autonomous vehicles and robot research in inclement winter weather. WADS focuses exclusively on challenging conditions such as heavy snowfall and occasional white-out scenarios, providing a robust platform for testing and development. WADS comprises images captured across diverse conditions, encompassing variations in road surfaces, weather, lighting, and terrain types, etc.

## [thermaltrack](https://yimingyang-mtu.github.io/profilo.github.io/thermaltrack)
  To enhance the robustness and generalization of our model, we performed dataset augmentation, including techniques including random flip, rotation, brightness, contrast, scaling, noise injection, and perspective change to simulate a wider variety of challenging road conditions and improve the model's ability to handle real-world variability. We augmented 951 images to 7608 in total for model training.
  * Training: 70%
  * Validation: 15%
  * Testing: 15%
