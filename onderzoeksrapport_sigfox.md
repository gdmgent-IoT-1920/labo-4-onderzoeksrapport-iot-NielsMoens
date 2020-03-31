<!----- 
* Naam: Niels Moens
* Klas: 2NMD
* Vak: Internet of Things
* Datum:Tue Mar 31 2020 
----->

# Onderzoeksrapport Sigfox

![alt_text](https://www.flashnet.ro/wp-content/uploads/2017/03/technology_sigfox-.png)


## Inleiding

Voor labo 4 van het vak Internet of Things kregen we de opdracht om een onderzoeksrapport te schrijven over een bepaald onderwerp. Daarnaast moet dit onderzoeksrapport volledig in markdown worden gemaakt. Het onderwerp waarvoor ik gekozen heb is Sigfox. 


## Waarom bestaat sigfox?

Voor dat we ons gaan verdiepen in wat Sigfox juist is moeten we eerst weten waarom Sigfox ontstaan is. 

De vraag naar Machine to machine- en Internet of things appartementen blijft groeien. Om een idee te geven over de hoeveelheid apparaten we spreken. Volgens de recente voorspellingen van gartner zullen er in 2020 zullen er bijna 6 miljard apparaten wereldwijd actief verbonden zijn met het internet. (Redactie iot journal, 2019)

Om deze apparaten met elkaar te kunnen verbinden en te bedienen heb je natuurlijk een netwerk nodig. Wel dit is waar Sigfox er tussen komt. (Engie, 2016)


![alt_text](https://corporate.engie.be/content/uploads/sites/14/cache/2017/02/sigfox-1330x530/1207537336.jpg)


## Wat is Sigfox

Sigfox is een internationaal cellulaire gebaseerd Low Power Wide Area Network of een LPWAN. Deze technologie is ontwikkeld voor het draadloos verbinden van apparaten zoals sensoren[^1], actuatoren[^2],  Machine to machine of M2M applicaties[^3] en Internet of things of IoT apparaten[^4]. Sigfox dekt wereldwijd 70 landen dat is een oppervlakte van maar liefst 5 million km² en heeft 1.1 miljard gebruikers.

Het Sigfox LPWAN netwerk is ontworpen om te werken op een zeer lage stroom. 
Op deze manier is het niet noodzakelijk om aan externe apparaten een constante voeding te geven maar kan dit via batterijen gebeuren die over een lange periode kunnen werken zonder dat connectie problemen zich voordoen.

Daarnaast is het Sigfox LPWAN netwerk zo ontwikkeld dat de communicatie over zeer lange afstanden kan gedaan worden. Een basisstations kan kilometers een communicatie doorsturen. Basisstations zijn Sigfox-antennes die instaan voor het ontvangen en verzenden van berichten en deze dan vervolgens doorsturen naar de Sigfox cloud. Door dat er maar een beperkt aantal basisstations worden gebruikt kan de de kostprijs naar beneden gedrukt worden. 

Door dat Sigfox een cellulair gebaseerd netwerk is kunnen de Sigfox-nodes op afstand communicatie leggen met de basisstations. Deze basisstations hebben een actieve internet connectie. Op deze manier kan je gegevens verzamelen van op afstand, het enige wat je nodig hebt is een internet connectie. (electronicnotes, z.d.)

## Voordelen Sigfox tov traditionele netwerken

Velen vragen zich dan af waarom hebben we nog een netwerk nodig om alle onze Internet of things apparaten met elkaar te verbinden terwijl er al wifi, 4g en 5g netwerken bestaan. 

### Geen roaming

Een groot voordeel van het Sigfox netwerk is het feit dat er geen roaming bestaat binnen het Sigfox netwerk. Roaming is een draadloze telecommunicatie die er voor zorgt dat een gebruiker kan gebruik maken van een netwerk waar hij niet op geregistreerd staat. Een voorbeeld hiervan is als je in het buitenland bent kan je nog steeds bellen en surfen met je gsm op het netwerk van de lokale service provider. Aan roaming kunnen vaak wel service kosten verbonden zijn. (Smith, 2013)

Het Sigfox netwerk maakt gebruikt van licentievrije frequenties 862 tot 928 Mhz. Dit kan van land tot land verschillen door lokale wetten en regelgevingen. (Sigfox, z.d.) 
Door het gebruik van licentievrije frequenties dus geen sprake van roaming en zijn er geen extra kosten die er voor de klant bij komen bij het versturen van data over hun netwerk. Stel dat je een product in België maakt dat gebruikt maakt van het Sigfox netwerk en dit product later over omringende landen gebruikt wordt. Dit kan allemaal zonder dat er extra kosten aan te pas komen.(Engie, 2017)


### Energieverbruik

Door dat Sigfox internationaal zijn eigen Sigfox netwerk gebruikt is er geen SIM-kaart of Gateway nodig om apparaten te verbinden. De Sigfox communicatie technologie verbruikt 200 tot 600 keer minder energie t.o.v. andere mobile netwerken zoals 4g. (Engie, 2017)


## Hoe werkt Sigfox

![alt_text](https://i.ytimg.com/vi/wkyzEnYpxSA/maxresdefault.jpg) (SIGFOX, 2016) 

Sigfox biedt een bidirectioneel datatransport aan voor IoT applicaties. Bidirectioneel datatransport kan je vergelijken met een twee richting straat zodat er berichten ontvangen en verzonden worden door het aangesloten apparaat. 

De meeste apparaten die verbonden zijn op het Sigfox netwerk communiceren niet met woorden zoals mensen met elkaar communiceren. Deze sturen kleine berichten door met hun waarden in. Deze berichten kunnen maar een grote hebben 12 bytes uplink[^5] en 3 bytes downlink[^6]. Per dag kunnen er maar een aantal berichten worden verzonden. Dit kunnen er namelijk maar maximum 140 per dag zijn. Door op deze manier te werken verminderd je batterij afname en verleng je de levensduur van de batterijen in de apparaten van je netwerk. (SIGFOX, 2016)

Een belangrijke service die Sigfox ook aanbiedt is de Sigfox cloud. Dit is een interface tussen de klanten en alle Sigfox partners die geconnecteerd zijn zoals bijvoorbeeld Engie Electrabel die 99% van België dekt voor Iot netwerken. (Engie, z.d.)  
Deze service wordt hoofdzakelijk gebruikt voor het versturen en ontvangen van datapakketjes (kleine berichten data) maar wordt ook gebruikt voor het servicekaart voorspellingen. Zo kan men bijhouden hoeveel gebied het netwerk bereik dekt.

Netwerkoperators kunnen Sigfox cloud ook gebruiken als een tool voor het netwerkbeheer en contractbeheer zo kan de netwerkoperator de contract overeen komsten van zijn klanten overzichtelijk bijhouden. Dit noemt Sigfox het OSS-systeem[^7]. (SIGFOX, 2016) 

Even kort samengevat hoe de levenscyclus van een Sigfox datacommunicatie er uit ziet. 
Op de website van Sigfox bouw wordt dit in een stappenplan omschreven: 

1. Als het apparaat actief is wordt er een klein datapakket verzonden over de radio frequentie.
2. Sigfox lokale basisstations in het gebied ontvangen het datapakket.
3. De basisstations sturen dit dan door naar de Sigfox cloud.
4. De Sigfox cloud stuurt het bericht dan door haar het platform van de klant.

## Sigfox toepassingsvoorbeelden in ons land

Nu we een antwoord hebben op de vragen wat, waarom en hoe Sigfox werkt gaan we eens kijken naar de werkelijke toepassingen die door Sigfox gebruikt wordt in ons land. 

### ENGIE IoT-netwerk

Het Engie Internet of Things netwerk in België is gebaseerd op de Sigfox technologie. Dit netwerk dekt het Belgische grondgebied volledig. Wat is er allemaal verbonden met dit netwerk: 

*   **Pilootproject van waterlink in Antwerpen** met intelligente watermeters die het waterverbruik vereenvoudigen, onderhoud houd van de installaties en waterlekken detecteren. 

*   **TankU IoT **met slimme oliepeilmeters die gebruik maken van een Sigfox netwerkkaart om het niveau in de tank op te meten. 

*   **Nexxtender Mobile **een mobiel oplaadsysteem voor elektrische wagens die gebruik maakt van het draadloze Sigfox netwerk om data uit te wisselen met een beheerplatform voor de gebruikers. 

*   **Autonome rookdetectors **die gebruik maken van de Sigfox technologie. De rookdetector stuur een signaal door naar Sigfox en dit wordt dat in real time doorgestuurd naar de gebruiker. 

*   **Blue **een belgische product dat het water in zwembad water meet. De temperatuur , ph-waarden, zout en chloorwaarden worden doorgestuurd over het Sigfox netwerk. Via een applicatie op de smartphone de gebruiker deze in real time raadplegen.
  
  (Engie, 2016) 

## Verdict

Het komt er dus op neer dat het Sigfox netwerk een betrouwbare, goedkope optie is voor het globaal verbinden van Internet of Things applicaties. 

## Literatuurlijst 

electronicnotes. (z.d.). _What is SIGFOX - M2M IoT » Electronics Notes_. Geraadpleegd op 29 maart 2020, van https://www.electronics-notes.com/articles/connectivity/sigfox/what-is-sigfox-basics-m2m-iot.php

Engie. (z.d.). _Coverage_. Geraadpleegd op 31 maart 2020, van https://www.engiem2m.be/coverage

Engie. (2016, 24 oktober). _The internet of things: vandaag eraan denken om morgen te winnen_. Geraadpleegd op 30 maart 2020, van https://www.engie.be/nl/business/blog/sustainability/internet-of-things-in-uw-business-model-5-redenen-waarom

Engie. (2017, 8 september). _Internet of Things-netwerk van ENGIE dekt nu heel België_. Geraadpleegd op 30 maart 2020, van https://corporate.engie.be/nl/internet-of-things-netwerk-van-engie-dekt-nu-heel-belgie/

Galaxy. (z.d.). _Machine to Machine | Galaxy_. Geraadpleegd op 30 maart 2020, van https://www.galaxymobile.be/be-nl/machine-machine

Geertsma, P. (2020, 7 januari). _Wat is een actuator definitie actuator | TechnischWerken_. Geraadpleegd op 29 maart 2020, van http://www.technischwerken.nl/kennisbank/techniek-kennis/wat-is-een-actuator-definitie-actuator/

Redactie iot journal. (2019, 9 september). _Gartner: “In 2020 zijn er 5,8 miljard IoT-apparaten actief”_. Geraadpleegd op 30 maart 2020, van https://www.iotjournaal.nl/gartner-in-2020-zijn-er-58-miljard-iot-apparaten-actief/

Saleforce. (z.d.). _Het Internet of Things, wat is dat? - Salesforce Nederland_. Geraadpleegd op 31 maart 2020, van https://www.salesforce.com/nl/learning-centre/tech/internet-of-things/

Sigfox. (z.d.). _Radio Configurations | Sigfox build_. Geraadpleegd op 30 maart 2020, van https://build.sigfox.com/sigfox-radio-configurations-rc#rc-technical-details

SIGFOX. (2016, 18 november). _SIGFOX TECHNOLOGY: Sigfox Core Service_. Geraadpleegd op 31 maart 2020, van https://www.youtube.com/watch?time_continue=2&v=6ZBGDtmDGRU&feature=emb_logo

Smith, C. (2013, 27 oktober). _How it Works: Roaming_. Geraadpleegd op 31 maart 2020, van https://www.androidauthority.com/how-it-works-roaming-95498/

Wikipedia-bijdragers. (2019, 15 oktober). _Sensor_. Geraadpleegd op 31 maart 2020, van https://nl.wikipedia.org/wiki/Sensor


<!-- Footnotes themselves at the bottom. -->
## Notes

[^1]:
     Een sensor is een component dat iets kan detecteren in verschillende vormen zoals licht, temperatuur, druk, etc. (Wikipedia-bijdragers, 2019)

[^2]:
     Een actuator is de beslisser die met de juiste waarden een systemen of apparaten kan schakelen. (Geertsma, 2020)

[^3]:
     Machine to Machine is met een realtime communicatie informatie uitwisselen tussen apparaten. (Geertsma, 2020)

[^4]:
     Internet of things zijn apparaten zoals huishoudelijke apparaten, wearables enz, die aan het internet verbonden zijn om zo online gegevens te kunnen verzenden. (Saleforce, z.d.)

[^5]:
     Uplink is het versturen van data het apparaat naar het netwerk.

[^6]:
     Downlink is het ontvangen van data van het netwerk naar het apparaat.

[^7]:
     OSS-systeem is Operation Support System (SIGFOX, 2016) 


<!-- Docs to Markdown version 1.0β20 -->