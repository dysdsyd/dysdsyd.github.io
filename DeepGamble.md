<script src="http://www.google.com/jsapi" type="text/javascript"></script> 
<script type="text/javascript">google.load("jquery", "1.3.2");</script>

<style type="text/css">
	body {
		font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; 
		font-size:16px;
		color: #404040;
		margin-left: auto;
		margin-right: auto;
		width: 1100px;
	}
	p {
	  line-height: 1.15;
	  margin: 30px 0;
	}
	
	h1 {
		font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
		font-size:32px;
		font-weight:300;
	}
	
	.disclaimerbox {
		background-color: #eee;		
		border: 1px solid #eeeeee;
		border-radius: 10px ;
		-moz-border-radius: 10px ;
		-webkit-border-radius: 10px ;
		padding: 20px;
	}

	video.header-vid {
		height: 140px;
		border: 1px solid black;
		border-radius: 10px ;
		-moz-border-radius: 10px ;
		-webkit-border-radius: 10px ;
	}
	
	img.header-img {
		height: 140px;
		border: 1px solid black;
		border-radius: 10px ;
		-moz-border-radius: 10px ;
		-webkit-border-radius: 10px ;
	}
	
	img.rounded {
		border: 1px solid #eeeeee;
		border-radius: 10px ;
		-moz-border-radius: 10px ;
		-webkit-border-radius: 10px ;
	}
	
	a:link,a:visited
	{
		color: #1367a7;
		text-decoration: none;
	}
	a:hover {
		color: #208799;
	}
	
	td.dl-link {
		height: 160px;
		text-align: center;
		font-size: 22px;
	}
	
	.layered-paper-big { /* modified from: http://css-tricks.com/snippets/css/layered-paper/ */
		box-shadow:
		0px 0px 1px 1px rgba(0,0,0,0.35), /* The top layer shadow */
		5px 5px 0 0px #fff, /* The second layer */
		5px 5px 1px 1px rgba(0,0,0,0.35), /* The second layer shadow */
		10px 10px 0 0px #fff, /* The third layer */
		10px 10px 1px 1px rgba(0,0,0,0.35), /* The third layer shadow */
		15px 15px 0 0px #fff, /* The fourth layer */
		15px 15px 1px 1px rgba(0,0,0,0.35), /* The fourth layer shadow */
		20px 20px 0 0px #fff, /* The fifth layer */
		20px 20px 1px 1px rgba(0,0,0,0.35), /* The fifth layer shadow */
		25px 25px 0 0px #fff, /* The fifth layer */
		25px 25px 1px 1px rgba(0,0,0,0.35); /* The fifth layer shadow */
		margin-left: 10px;
		margin-right: 45px;
	}

	.paper-big { /* modified from: http://css-tricks.com/snippets/css/layered-paper/ */
		box-shadow:
		0px 0px 1px 1px rgba(0,0,0,0.35); /* The top layer shadow */

		margin-left: 10px;
		margin-right: 45px;
	}


	.layered-paper { /* modified from: http://css-tricks.com/snippets/css/layered-paper/ */
		box-shadow:
		0px 0px 1px 1px rgba(0,0,0,0.35), /* The top layer shadow */
		5px 5px 0 0px #fff, /* The second layer */
		5px 5px 1px 1px rgba(0,0,0,0.35), /* The second layer shadow */
		10px 10px 0 0px #fff, /* The third layer */
		10px 10px 1px 1px rgba(0,0,0,0.35); /* The third layer shadow */
		margin-top: 5px;
		margin-left: 10px;
		margin-right: 30px;
		margin-bottom: 5px;
	}
	
	.vert-cent {
		position: relative;
		top: 50%;
		transform: translateY(-50%);
	}
	
	hr
	{
		border: 0;
		height: 1px;
		background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
	}
</style>

<html>
<head>
	<title>DeepGamble</title>
	<meta property="og:image" content="Path to my teaser.png"/> <!-- Facebook automatically scrapes this. Go to https://developers.facebook.com/tools/debug/ if you update and want to force Facebook to rescrape. -->
	<meta property="og:title" content="Creative and Descriptive Paper Title." />
	<meta property="og:description" content="Paper description." />

	<!-- Get from Google Analytics -->
	<!-- Global site tag (gtag.js) - Google Analytics -->
	<script async src=""></script> 
	<script>
		window.dataLayer = window.dataLayer || [];
		function gtag(){dataLayer.push(arguments);}
		gtag('js', new Date());

		gtag('config', 'UA-75863369-6');
	</script>
</head>

<body>
	<br>
	<br>
	<br>
	<center>
		<span style="font-size:30px">DeepGamble: Towards unlocking real-time player intelligence using multi-layer instance segmentation and attribute detection</span>
		<table align=center width=700px>
			<table align=center width=700px>
				<tr>
					<td align=center width=200px>
						<center>
							<span style="font-size:20px"><a href="https://dysdsyd.github.io">Danish Syed*</a></span>
						</center>
					</td>
					<td align=center width=200px>
						<center>
							<span style="font-size:22px"><a href="https://www.linkedin.com/in/namangandhi/">Naman Gandhi*</a></span>
						</center>
					</td>
					<td align=center width=200px>
						<center>
							<span style="font-size:22px"><a href="https://www.linkedin.com/in/arushiarora/">Arushi Arora*</a></span>
						</center>
					</td>
					<br>
					<td align=center width=200px>
						<center>
							<span style="font-size:22px"><a href="https://www.linkedin.com/in/nskadam/">Nilesh Kadam</a></span>
						</center>
					</td>
				</tr>
			</table>
			
			<table align=center width=250px>
				<tr>
					<td align=center width=120px>
						<center>
							<span style="font-size:20px"><a href=''>[Paper]</a></span>
						</center>
					</td>
<!-- 					<td align=center width=120px>
						<center>
							<span style="font-size:20px"><a href='https://github.com/richzhang/webpage-template'>[GitHub]</a></span><br>
						</center>
					</td> -->
				</tr>
			</table>
		</table>
	</center>
	<br>
	<center>
		<table align=center width=850px>
			<tr>
				<td width=260px>
					<center>
						<img class="round" style="width:100%" src="/DeepGamble/architecture.png"/>
					</center>
				</td>
			</tr>
		</table>
		<table align=center width=850px>
			<tr>
  	              <td width=400px>
  					<center>
  	                	<span style="font-size:14px"><i>DeepGamble System Architecture. High-resolution cameras, Raspberry Pis are connected via a gateway to the Google Cloud Platform where inference models are deployed as micro-services to perform inference in real-time. After assimilating the game play, results are pushed to Google BigQuery for further analysis and real-time dashboards are generated.</i>
					</center>
  	              </td>
			</tr>
		</table>
	</center>
<br><br>
	<hr>

	<table align=center width=850px>
		<center><h1>Abstract</h1></center>
		<tr>
			<td>
				Annually the gaming industry spends approximately $15 billion in marketing reinvestment. However, this amount is spent without any consideration for the skill and luck of the player. For a casino, an unskilled player could fetch ~4x more revenue than a skilled player. This paper describes a video recognition system that is based on an extension of the Mask R-CNN model. Our system digitizes the game of blackjack by detecting cards and player bets in real-time and processes decisions they took in order to create accurate player personas. Our proposed supervised learning approach consists of a specialized three-stage pipeline that takes images from two viewpoints of the casino table and does instance segmentation to generate masks on proposed regions of interests. These predicted masks along with derivative features are used to classify image attributes that are passed onto the next stage to assimilate the gameplay understanding. Our end-to-end model yields an accuracy of ~95% for the main bet detection and ~97% for card detection in a controlled environment trained using transfer learning approach with 900 training examples. Our approach is generalizable and scalable and shows promising results in varied gaming scenarios and test data. Such granular level gathered data, helped in understanding player's deviation from optimum strategy and thereby separate the skill of the player from the luck of the game. Our system also assesses the likelihood of card counting by correlating player's betting pattern to the deck's scaled count. Such a system lets casinos flag fraudulent activity and calculate expected personalized profitability for each player and tailor their marketing reinvestment decisions.
				
			</td>
		</tr>
	</table>
	<br><br>

	<hr>
	<center><h1>Video</h1></center>
	<p align="center">
		<iframe width="80%" height="30%" src="/DeepGamble/blackjack_video_recognition.mp4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen align="center"></iframe>
	</p>

	  <!-- <center><h2>How to interpret the results</h2></center> -->
<div class="disclaimerbox">
	  		 <span style="color:#646464">
	  		  	<center><span style="font-size:28px"><b>DeepGamble in real-time</b></span></center>

	  		  	<br>
				
				<i> Welcome! Computer vision algorithms often work well on some images, but fail on others. Ours is like this too. We believe our work is a significant step forward in solving the colorization problem. However, there are still many hard cases, and this is by no means a solved problem. Some failure cases can be seen <a href="#vgg_res">below</a> and the figure <a href="./resources/images/imnet_failures.jpg">here</a>.

			</span>

			</div>
  		  <br><br>
	<hr>

<!-- 	<center><h1>Code</h1></center>

	<table align=center width=420px>
		<center>
			<tr>
				<td>
				</td>
			</tr>
		</center>
	</table>
	<table align=center width=400px>
		<tr>
			<td align=center width=400px>
				<center>
					<td><img class="round" style="width:450px" src="./resources/method_diagram.png"/></td>
				</center>
			</td>
		</tr>
	</table>
	<table align=center width=850px>
		<center>
			<tr>
				<td>
					Short description if wanted
				</td>
			</tr>
		</center>
	</table>
	<table align=center width=800px>
		<br>
		<tr><center>
			<span style="font-size:28px">&nbsp;<a href='https://github.com/richzhang/webpage-template'>[GitHub]</a>
			</center>
		</span>
	</table>
	<br>
	<hr> -->
	<table align=center width=450px>
		<center><h1>Paper and Supplementary Material</h1></center>
		<tr>
			<td><a href=""><img class="layered-paper-big" style="height:175px" src="/DeepGamble/paper.png"/></a></td>
			<td><span style="font-size:14pt">D. Syed*, N. Gandhi*, A. Arora* & N. Kadam<br>
				<b>DeepGamble</b><br>
				ICMLA, 2020.<br>
				(hosted on <a href="">ArXiv</a>)<br>
				(<a href="./resources/camera-ready.pdf">camera ready</a>)<br>
				<span style="font-size:4pt"><a href=""><br></a>
				</span>
			</td>
		</tr>
	</table>
	<br>

	<table align=center width=600px>
		<tr>
			<td><span style="font-size:14pt"><center>
				<a href="./resources/bibtex.txt">[Bibtex]</a>
			</center></td>
		</tr>
	</table>
<br><br>
	<hr>
	<br>

	<table align=center width=900px>
		<tr>
			<td width=400px>
				<left>
					<center><h1>Acknowledgements</h1></center>
					The authors would like to thank Arun Shastri, Rasvan Dirlea, Mike Francis, Akshat Rajvanshi, Manoj Bheemineni, Brendan Riley, Geoff Cohn, Jayendu Sharma, Thompson Nguyen and others who contributed, supported, guided and collaborated with us during the development and deployment of our system.
				</left>
			</td>
		</tr>
	</table>
	<br>
	<br>
	<hr>
	<br>
	<table align=center width=900px>
		<tr>
			<td width=400px>
				<left>
					<!-- <center><h1>Acknowledgements</h1></center> -->
					This template was originally made by <a href="http://web.mit.edu/phillipi/">Phillip Isola</a> and <a href="http://richzhang.github.io/">Richard Zhang</a> for a <a href="http://richzhang.github.io/colorization/">colorful</a> ECCV project; the code can be found <a href="https://github.com/richzhang/webpage-template">here</a>.
				</left>
			</td>
		</tr>
	</table>

<br>
</body>
</html>

