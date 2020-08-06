---
layout: post
published: false
title: Loss Diary
---




## Classification Losses


### SVM Loss
SVM loss is set up so that the SVM “wants” the correct class for each image to a have a score higher than the incorrect classes by some fixed margin $$\Delta$$. Multiclass SVM Loss for the i-th class would be:

$$ L_{i}=\sum_{j \neq y_{i}} \max \left(0, s_{j}-s_{y_{i}}+\Delta\right) $$
