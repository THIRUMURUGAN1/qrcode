
<html>
<head>
	<meta charset="utf-8">
	<title> Display Web cam </title>
	
	<style>
	#container {
	
		margin: 0px auto;
		width: 500px;
		height: 375px;
		border: 10px #333 solid;
		
	}
	
$videoElement{
	width: 500px;
	height: 375px;
	background-color: #666;
	}
	
	</style>
	</head>
	
	<body>
		<center> Scan me </center>
		<div id="container">
			<video autoplay="true" id="videoElement">
			
			</video>
			
		</div>
		
		<script>
			var video= document.querySelector("#videoElement");
			
			if (navigator.mediaDevices.getUserMedia){
				.then(function stream){
					video.srcObject = stream;
					})
					.catch(function(erroe){
						console.log("something went wrong!");
						});
						}
		</script>
		
	</body>
	</html>


