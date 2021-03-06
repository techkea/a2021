---
layout: default
title: Lek 5 - Client/Server arkitektur
nav_order: 80
description: ""
---

# Client / Server arkitektur 

## Læringsmål
* Du skal kunne beskrive Clientens (feks. browseren) og Serverens (feks. Tomcat) ansvarsområder. (Ex. hvor bliver koden i et konkret eksempel eksekveret)  
* Du skal have en basal forståelse af HTTP protokollen, herunder kunne forklare forskellen på GET og POST og vise hvordan i kan bruge det.
* Du skal forstå Request/Response i forhold til en Spring Boot Applikation.
* Du skal forstå og kunne bruge @GetMapping og @PostMapping i en Spring Boot Applikation. 
* Kunne bruge browserens inspect tool til at analysere en webapplikations request & responces. 

## Læringsforløb
* Introduktion
	* Et ultra simplet Spring Boot projekt, med fokus på Client/Server og kommunikation imellem dem.
* Studiegrupper
	* Lav øvelser
* ca. 15.15 mødes vi samlet og laver opsamling, afrunding og snak.

## Materiale
* [i kan finde en løsning på 404 fejlen i forhold til jeres webserver opgave her](https://techkea.github.io/Dat-20-b-og-c-semesterplan/3.html#exporter-en-webapp-til-war)
* [Client–server model](https://en.wikipedia.org/wiki/Client%E2%80%93server_model)
* [Hypertext Transfer Protocol (HTTP)](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:the-internet/xcae6f4a7ff015e7d:web-protocols/a/hypertext-transfer-protocol-http)
* [Kodeeksempler fra undervisningen i dag](https://github.com/techkea/client_server_kodeeksempel_fra_undervisningen)
### Ip adresser og Domain Name Server
![](../../assets/images/img/1.jpg)
### Client / Server
![](../../assets/images/img/2.jpg)

### Hvad foregår på serveren og hvad foregår på klienten?
![](../../assets/images/img/3.jpg)

## Øvelser
### Et ultra simpelt Spring Boot projekt.
Lav et ultra simpelt spring boot projekt. Projektet skal minde meget om det i lige har fået demonstreret af Claus.   

#### Del 1    

1. Projektet skal ved oprettelsen bruge **"war packaging"**
2. Projektet skal have følgende dependencies:	
	* Web: Spring Web
	* Template engines: Thymeleaf
3. Projektet skal have en controller package med en klasse i som hedder HomeController.
	* I HomeController klassen skal i have en index metode som returnerer en index.html side
	* index.html siden skal ligge i Templates mappen og have et 
		
        ````
		<h1>Dagens Citat</h1>
		<p>Topstyrret social ingenørkunst</p>
	````
4. Kør projektet og åben det via http://localhost:8080
5. Fra din mobiltelefon prøv om du kan se siden som kommer fra din computer. (Computer er serveren mobilen er clienten).
6. Forklar (for din gruppe, eller dig selv) flowet (step by step og så detaljeret som muligt) fra at du skriver 192.168.0.16:8080 (eller en anden adresse) til at du får et http response tilbage fra serveren.

#### Del 2
1. Tilføj et logo (billede) til din html side, og et ekstern style sheet.
	* Stylesheetet skal ligge i static mappen.
2. Med fokus på billedet og styleshettet. Forklar (for din gruppe, eller dig selv) flowet (step by step, og så detaljeret som muligt) fra at du skriver 192.168.0.16:8080 (eller en anden adresse) til at du får et http response tilbage fra serveren.  

#### Del 3
1. Tilføl 2 metoder til din controller.
	* De skal begge have navnet citat()
	* Den ene skal reagerer på et **Get request** og den anden på et **Post Request**.
2. Du skal lave en tilhørende citat.html side som indeholder en form og tager imod input (et nyt citat).
3. Med fokus på det nye kode. Forklar (for din gruppe, eller dig selv) flowet (step by step, og så detaljeret som muligt) fra at du skriver 192.168.0.16:8080/citat (eller en anden adresse) til at du får et http response tilbage fra serveren. 


 
