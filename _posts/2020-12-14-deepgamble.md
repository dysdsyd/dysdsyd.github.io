---
layout: post
published: true
title: DeepGamble
subtitle: >-
  Towards unlocking real-time player intelligence using multi-layer instance
  segmentation and attribute detection
image: /img/deepg.png
---
<table align=center width=80%>
## About

DeepGamble is a video recognition system that is based on an extension of the Mask R-CNN model. It digitizes the game of blackjack by detecting cards and player bets in real-time and processes decisions they took in order to create accurate player personas.

> A longer technical report of our ICMLA 2020 paper is available [here]()
<br>

## Overview Video

<div style="text-align:center">

<iframe width="560" height="315" src="/img/DeepGamble/DeepGamble_ediited.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<br>

## Abstact & Method

DeepGamble System Architecture consists of high-resolution cameras, Raspberry Pis are connected via a gateway to the Google Cloud Platform where inference models are deployed as micro-services to perform inference in real-time. After assimilating the game play, results are pushed to Google BigQuery for further analysis and real-time dashboards are generated.

<center>
  <table align=center width=850px>
    <tr>
      <td width=260px>
      <center>
        <img class="round" style="width:100%" src="/img/DeepGamble/architecture.png"/>
       </center>
		</td>
	</tr>
  </table>
</center>


Our proposed supervised learning approach consists of a specialized three-stage pipeline that takes images from two viewpoints of the casino table and does instance segmentation to generate masks on proposed regions of interests. These predicted masks along with derivative features are used to classify image attributes that are passed onto the next stage to assimilate the gameplay understanding. Our end-to-end model yields an accuracy of ~95% for the main bet detection and ~97% for card detection in a controlled environment trained using transfer learning approach with 900 training examples.

<center>
  <table align=center width=850px>
    <tr>
      <td width=260px>
      <center>
        <img class="round" style="width:100%" src="/img/DeepGamble/model.png"/>
       </center>
		</td>
	</tr>
  </table>
</center>
<br>

## DeepGamble in Action

<div style="text-align:center">

<iframe width="560" height="315" src="/img/DeepGamble/blackjack_video_recognition.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<br>

## Paper
<table align=center width=450px>
  <tr>\
    <td><a href=""><img class="layered-paper-big" style="height:175px" src="/img/DeepGamble/paper.png"/></a></td>
			<td><span style="font-size:14pt">D. Syed*, N. Gandhi*, A. Arora* & N. Kadam<br>
				<b>DeepGamble</b><br>
				ICMLA, 2020.<br>
				(hosted on <a href="">ArXiv</a>)<br>
				</span>
			</td>
		</tr>
</table>
<br>

## Citing us

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
The authors would like to thank Arun Shastri, Rasvan Dirlea, Mike Francis, Akshat Rajvanshi, Manoj Bheemineni, Brendan Riley, Geoff Cohn, Jayendu Sharma, Thompson Nguyen and others who contributed, supported, guided and collaborated with us during the development and deployment of our system.
  
</table>