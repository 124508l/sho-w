<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
		<!--
        	作者：2216944627@qq.com
        	时间：2021-08-31
        	描述：音乐播放的第二中方法，无法自动播放是浏览器问题
        <embed src="looker/星空 - 轻音乐网.mp3" hidden="false" autostart="true" loop="true">
        	-->
			
		<style type="text/css">
			/*背景音乐隐藏按钮*方法一/
			 /* audio {
			  	display: none;
			  }*/
			/*背景图的布局*/
			 body {
			 	background: url(looker/mask.jpg) no-repeat center center;
			 	background-size: cover;
			 	background-attachment: fixed;
			 	background-color: #CCCCCC;
			 }

			.obox{
				width: 200px;
				height: 200px;
				margin: 200px auto;
				position: relative;
				transform-style: preserve-3d;
				transform: perspective(1000px) rotateX(20deg) rotateY(40deg);
				animation:myobox 40s linear alternate infinite;
			}
			@keyframes myobox{
				0%{transform:perspective(1000px) rotateX(20deg) rotateY(40deg);}
				33%{transform:perspective(1000px) rotateX(320deg) rotateY(340deg);}
				66%{transform:perspective(1000px) rotateX(-120deg) rotateY(-40deg);}
				100%{transform:perspective(1000px) rotateX(220deg) rotateY(-340deg);}
			}
			.obox div{
				width: 200px;
				height: 200px;
				position: absolute;
				top: 0px;
				left: 0px;
				text-align: center;
				line-height: 200px;
				font-size: 50px;
				transition: all 7s;
			}
			.obox img{
				display: block;
				width: 100%;
				height: 100%;
			}
			.obox div:nth-child(1),.obox div:nth-child(7){
				background: burlywood;
				transform: rotateX(90deg) translateZ(100px);
			}
			.obox div:nth-child(2),.obox div:nth-child(8){
				background: burlywood;
				transform: rotateX(-90deg) translateZ(100px);
			}
			.obox div:nth-child(3),.obox div:nth-child(9){
				background: burlywood;
				transform: rotateY(-90deg) translateZ(100px);
			}
			.obox div:nth-child(4),.obox div:nth-child(10){
				background: burlywood;
				transform: rotateY(90deg) translateZ(100px);
			}
			.obox div:nth-child(5),.obox div:nth-child(11){
				background: green;
				transform: translateZ(100px);
			}
			.obox div:nth-child(6),.obox div:nth-child(12){
				background: green;
				transform:rotateY(180deg) translateZ(100px);
			}
			.obox:hover div:nth-child(7){
				transform: rotateX(90deg) translateZ(200px);
			}
			.obox:hover div:nth-child(8){
				transform: rotateX(-90deg) translateZ(200px);
			}
			.obox:hover div:nth-child(9){
				transform: rotateY(-90deg) translateZ(200px);
			}
			.obox:hover div:nth-child(10){
				transform: rotateY(90deg) translateZ(200px);
			}
			.obox:hover div:nth-child(11){
				transform: translateZ(200px);
			}
			.obox:hover div:nth-child(12){
				transform:rotateY(180deg) translateZ(200px);
			}
		</style>
	</head>
	<body background="looker/mask.jpg">
		<div class="obox" >
			<div >
			<img src="img/b1.jpg"/>
			</div>
			<div >
				<img src="img/a6.jpg"/>
			</div>
			<div >
				<img src="img/a8.jpg"/>
			</div>
			<div >
				<img src="img/a9.jpg"/>
			</div>
			<div >
				<img src="img/b4.png" />
			</div>
			<div >
				<img src="img/b5.png" />
			</div>
			
			<div>
				<img src="img/a7.jpg"/>
			</div>
			<div>
				<img src="img/a1.jpg"/>
			</div>
			<div>
				<img src="img/a2.jpg"/>
			</div>
			<div>
				<img src="img/a3.jpg"/>
			</div>
			<div>
				<img src="img/a4.jpg"/>
			</div>
			<div>
				<img src="img/a5.jpg"/>
			</div>
			
		</div>
		<!--
        	作者：2216944627@qq.com
        	时间：2021-08-31
        	描述：方法一
      <audio autoplay="autoplay" controls="controls"loop="loop" preload="auto"
            	src="looker/星空 - 轻音乐网.mp3">
      		你的浏览器版本太低，不支持audio标签
      		</audio>
  -->
	</body>
	<iframe src="looker/星空 - 轻音乐网.mp3" allow="autoplay" style="display:none" id="iframeAudio"></iframe>
</html>
