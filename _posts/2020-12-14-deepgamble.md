---
layout: post
published: true
title: DeepGamble
image: /img/deepg.png
---
## About
---
DeepGamble is a video recognition system that is based on an extension of the Mask R-CNN model. It digitizes the game of blackjack by detecting cards and player bets in real-time and processes decisions they took in order to create accurate player personas.

> A longer technical report of our ICMLA 2020 paper is available [here]()
<br>

## Overview Video
---


<figure class="video_container">
  <video controls="true" allowfullscreen="true" width="640" height="480">
    <source src="/img/DeepGamble/DeepGamble_vdo.mp4" type="video/mp4">
  </video>
</figure>
<br>

## Abstact & Method
---
DeepGamble System Architecture consists of high-resolution cameras, Raspberry Pis are connected via a gateway to the Google Cloud Platform where inference models are deployed as micro-services to perform inference in real-time. After assimilating the game play, results are pushed to Google BigQuery for further analysis and real-time dashboards are generated.

![](/img/DeepGamble/architecture.png)

Our proposed supervised learning approach consists of a specialized three-stage pipeline that takes images from two viewpoints of the casino table and does instance segmentation to generate masks on proposed regions of interests. These predicted masks along with derivative features are used to classify image attributes that are passed onto the next stage to assimilate the gameplay understanding. Our end-to-end model yields an accuracy of ~95% for the main bet detection and ~97% for card detection in a controlled environment trained using transfer learning approach with 900 training examples.

![](/img/DeepGamble/model.png)

## DeepGamble in Action
---

<figure class="video_container">
  <video controls="true" allowfullscreen="true" width="640" height="480">
    <source src="/img/DeepGamble/blackjack_video_recognition.mp4" type="video/mp4">
  </video>
</figure>
<br>

## Paper
---
<table align=center width=450px>
  <tr>
    <td><a href=""><img class="layered-paper-big" style="height:175px" src="/img/DeepGamble/paper.png"/></a></td>
			<td><span style="font-size:14pt">D. Syed*, N. Gandhi*, A. Arora* & N. Kadam<br>
				<b>DeepGamble</b><br>
				ICMLA, 2020.<br>
				(<a href="">ArXiv</a>)<br>
				</span>
			</td>
		</tr>
</table>
<br>

## Citing us
---
If you would like to cite us, you could use the following BibTeX entry.

```
@article{deepgamble,
    author  = { Danish Syed and Naman Gandhi and  Arushi Arora and Nilesh Kadam },
    title   = { DeepGamble: Towards unlocking real-time player intelligence using multi-layer instance segmentation and attribute detection },
    journal = { arXiv },
    year    = { 2020 },
}
```
<br>

## Acknowledgements
---
The authors would like to thank Arun Shastri, Rasvan Dirlea, Mike Francis, Akshat Rajvanshi, Manoj Bheemineni, Brendan Riley, Geoff Cohn, Jayendu Sharma, Thompson Nguyen and others who contributed, supported, guided and collaborated with us during the development and deployment of our system.
  