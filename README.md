# page<html><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">


		<title>Preisbestimmung USB-Powerbank-Großhandel</title>
		
		

		

		<script>
		
		
		 "use strict";
		 function fAuswahl () {
			
			var vAuswahl;
			var vMenge ;
			var vAusgabe;
			var vPreis;
			var vPreisA=8.99;
			var vPreisB=9.99;
			var vPreisC=10.99;
			var vKosten;
			var vRabatt;
			var vRabatt1= 0.00;
			var vRabatt2= 0.05;
			var vRabatt3= 0.10;
			var vRabattineuro ;
			var vGesamtpreismitrabatt;
			
			vAuswahl=document.getElementById("idAuswahl").value;
			
		
		
		vMenge = document.getElementById("idMenge").value; 
		vMenge = parseFloat(vMenge)
		 

			
			 if (vAuswahl=="Powerbank-Spencial") {
			 
				vPreis=vPreisA;
			 
			 }
			 else
			 if (vAuswahl=="Powerbank-Eleganz") {
			 
				vPreis=vPreisB;
			 
			 }
			 else
			if	(vAuswahl=="Powerbank-Avantgarde") {
			 
				vPreis=vPreisC;
			 
			 }
			 
			  vKosten= vPreis * vMenge;
			
			//Erweiterung Heute	 
			  if (vMenge  <50 ) {
			 
				vRabatt = vRabatt1;
			 
			 }
			 else
			 if (vMenge <100) {
			 
				vRabatt = vRabatt2;
			 
			 }
			 else
			 {
			 
				vRabatt = vRabatt3;
			 
			 }
			 
			// Erweiterung Ende 
			
			
			
			 vRabattineuro = vKosten * vRabatt;
			 vGesamtpreismitrabatt = vKosten - vRabattineuro;
			 
			 vAusgabe = "";

			vAusgabe = vAusgabe + "Ausgewähltesprodukt:";
			vAusgabe = vAusgabe + vAuswahl + "</br>" ;
			vAusgabe = vAusgabe + "Der Stückpreis beträgt bei einer Menge von: " ;
			vAusgabe = vAusgabe + vMenge; 
			vAusgabe = vAusgabe + " USB-Powerbankadapter" ;
			vAusgabe = vAusgabe + vPreis + "€" + "</br>" ;
			vAusgabe = vAusgabe + "Der Gesamtpreis inkl. MwSt. beträgt: " ; 
			vAusgabe = vAusgabe + vGesamtpreismitrabatt + "€" + "</br>"; 
			vAusgabe = vAusgabe + "Enthaltener Rabatt:" + vRabattineuro + "€";
			document.getElementById("idAusgabe").innerHTML = vAusgabe ;
			 
		 }
		</script>

	</head>


	<body>
	<div align="center"><h1> Preisbestimmung USB-Powerbank-Großhandel </h1> </div>
	
	<div align="center"> 
	
	<img src="file://lsbk-fs01/23ASS1-16$/Downloads/logo.png"> 
	
	</div>
	
	<br>
	
	<div align="center">
	
	Menge in Stück: <input id="idMenge" type="text" value="10"> Produktauswahl: <select id="idAuswahl"> 
																						<option> Powerbank-Spencial </option>
																						<option>  Powerbank-Eleganz </option>
																						<option> Powerbank-Avantgarde</option>
																						</select>
	</div> <br> <br>
	
	<div align="center">
	
	<button onclick="fAuswahl();">Berechne den Erlös</button> 
	
	</div> <br><br>

    </html>