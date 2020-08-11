---
layout: post
published: false
title: Loss Diary - WIP
---
![](/img/wip.jpg)

## Content
- [Classification Loss](#cls)

<a name="cls"></a>
---
### Classification Losses
 
**Notations:**  
$$f$$ = Classification Model  
$$x$$ = Input  
$$y$$ = Target Class  
$$s_{i} = f\left(x_{i}, W\right)$$ = Score for the i-th class  

#### Multiclass SVM Loss / Hinge Loss
SVM loss is set up so that the SVM “wants” the correct class for each image to a have a score higher than the incorrect classes by some fixed margin $$\Delta$$. Multiclass SVM Loss for the i-th class would be:

$$ 
L_{i}=\sum_{j \neq y_{i}} \max \left(0, s_{j}-s_{y_{i}}+\Delta\right)  
$$

#### Cross-Entropy Loss
We interpret the scores as the unnormalized log probabilities for each class and we define Cross-Entropy loss as:

$$L_{i}=-\log \left(\frac{e^{f_{y_{i}}}}{\sum_{j} e^{f_{j}}}\right) \quad \text { or equivalently } \quad L_{i}=-f_{y_{i}}+\log \sum_{j} e^{f_{j}}$$
