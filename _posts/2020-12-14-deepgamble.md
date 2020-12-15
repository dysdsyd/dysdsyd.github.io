---
layout: post
published: true
title: DeepGamble
image: /img/deepg.png
subtitle: Unlocking blackjack player intelligence using instance segmentation
---
<center>
<table align=center width=100%>
        <tr>
          <td align=center width=20%>
            <center>
              <span style="font-size:16px"><a href="https://dysdsyd.github.io">Danish Syed*</a></span>
            </center>
          </td>
          <td align=center width=20%>
            <center>
              <span style="font-size:16px"><a href="https://www.linkedin.com/in/namangandhi/">Naman Gandhi*</a></span>
            </center>
          </td>
          <td align=center width=20%>
            <center>
              <span style="font-size:16px"><a href="https://www.linkedin.com/in/arushiarora/">Arushi Arora*</a></span>
            </center>
          </td>
          <br>
          <td align=center width=20%>
            <center>
              <span style="font-size:16px"><a href="https://www.linkedin.com/in/nskadam/">Nilesh Kadam</a></span>
            </center>
          </td>
        </tr>
</table>
  </center>
<br>

DeepGamble is a video recognition system that is based on an extension of the Mask R-CNN model. It digitizes the game of blackjack by detecting cards and player bets in real-time and processes decisions they took in order to create accurate player personas.

> A longer technical report of our ICMLA 2020 paper is available [here]()
<br>

## Overview Video
---
<span style="vertical-align:-80%"> </span>
<figure class="video_container">
  <video controls="true" allowfullscreen="true" width="900" height="300">
    <source src="/img/DeepGamble/DeepGamble_vdo.mp4" type="video/mp4">
  </video>
</figure>
<span style="vertical-align:-80%"> </span>
<br>

## Abstact
---
> DeepGamble System Architecture consists of high-resolution cameras, Raspberry Pis are connected via a gateway to the Google Cloud Platform where inference models are deployed as micro-services to perform inference in real-time. After assimilating the game play, results are pushed to BigQuery for further analysis and real-time dashboards are generated. Our proposed supervised learning approach consists of a specialized three-stage pipeline that takes images from two viewpoints of the casino table and does instance segmentation to generate masks on proposed regions of interests. These predicted masks along with derivative features are used to classify image attributes that are passed onto the next stage to assimilate the gameplay understanding. Our end-to-end model yields an accuracy of ~95% for the main bet detection and ~97% for card detection in a controlled environment trained using transfer learning approach with 900 training examples.

<br>

## DeepGamble in Action
---
<span style="vertical-align:-80%"> </span>
<figure class="video_container">
  <video controls="true" allowfullscreen="true" width="900" height="220">
    <source src="/img/DeepGamble/blackjack_video_recognition.mp4" type="video/mp4">
  </video>
</figure>
<span style="vertical-align:-80%"> </span>
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
