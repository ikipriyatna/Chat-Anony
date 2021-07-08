

<html lang="in">

<head>

				<title>AnonyChat</title>

				<link href="anonychatcss" rel="stylsheet">

				<style>

								body{

				background-color:gainsboro;

}

.head{

				position:fixed;

				top:0;

				left:0;

				right:0;

				background-color:gray;	padding:14px;			

}

.span{

				background-color:gray;
				width:27px;
				height:4px;
				opacity:;
				margin-left:20px;
				display:flex;
				justify-content:space-between;
				flex-direction:column;
				margin-top:10px; margin-bottom:-30px;

}

.span span{

				background-color:white;
				color:red;
				width:17px;
				height:3px;
				display:block;	
				margin-left:-3px; margin-bottom:-30px;

}

.nama{

				text-align:center;

				font-family:cursive,"Brush Script MT";

	     color:white;

				margin-top:-21px;

}

.wa{

				width:60%;

				padding:10px;

				border:none;

				text-decoration:none;

				border-radius:3px;

				margin:auto;

				display:block;

}

.kirim{

				margin:auto;

				display:block;

				border:none;

				text-decoration:none;

				width:20%;

				background-color:black;

				color:white;

				padding:10px;

				border-radius:3px;

				font-size:10px;

				

				

}

.inpo{

				width:70%;

				font-size:9px;

				margin:auto;

				display:block;

}

.bawah{

				position:fixed;

				bottom:0;

				left:0;

				right:0;

				background-color:gray;

				padding:5px;

}

.copy{

				text-align:center;

				font-size:12px;

				color:white;

}

.sedang{

				text-align:center;

				display:none;

}

				</style>

				<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

</head>

<body>

				<div class="head">

								<button class="span" id="span">

								<span></span>

								<span></span>

								<span></span>

								</button>

								<h2 class="nama">Anony Chat</h2>

				</div>

				

				<div id="semua">

				

				<div class="info" id="info">

								<p class="inpo"> ⚠ <em>>Web ini di buat untuk kalian yang ingin mengungkapkan sesuatu kepada seseorang tapi kalian tidak berani bicara secara langsung</em></p>

				</div>

				<br><br><br><br>

				

				<div class="awal" id="awal">

							<form name="Anony-chat">

					

					<input type="text" placeholder="Nomor WhatsApp" class="wa" name="Nomor WhatsApp">

					<br>

					<input type="text" placeholder="Isi pesan" class="wa" name="Pesan">

					<br>

					<button class="kirim" id="kirim" type="submit">Kirim</button>

					</form>

					</div>

					

				</div>

		<br><br><br><br><br><br><br>

		

		<h2 class="sedang" id="sedang">Sedang di proses...</h2>

		<script>

						$(document).ready(function(){

  $("#kirim").click(function(){

    $("#sedang").fadeIn(1000);

    $("#semua").fadeOut(100);

    $("#kirim").fadeOut(100);

    

  });

});

		</script>

		

		<script>

						const scriptURL = 'https://script.google.com/macros/s/AKfycbze0NRRwbZg6NFzWm1j1x-ZT8SdytQiv6ZfNgC2uOLTTrbZFRJL_-1zDZvTIIyyYYYGEQ/exec'

  const form = document.forms['Anony-chat']

  form.addEventListener('submit', e => {

    e.preventDefault()

    fetch(scriptURL, { method: 'POST', body: new FormData(form)})

      .then(response => console.log('Success!', response))

      .catch(error => console.error('Error!', error.message))

  })

		</script>

		

				

				

				

				

				<div class="bawah">

								<p class="copy">Prytna Web Deisgn, Copyright &copy; 2021</p>

				</div>

				

</body>

</html>

