## Gilded Rose opdracht

## Installatie

PHP 7.1 + geinstalleerd, of gebruik vagrant:

```
vagrant up
vagrant ssh
```

## Opdracht

======================================
Gilded Rose Requirements Specificatie
======================================

Welcome bij het Gilded Rose team. Zoals je misschien weet zijn we een kleine herberg in een prominente stad, 
gerund door een vriendelijke herbergier genaamd Allison. 
Wij kopen en verkopen alleen de beste goederen. 
Helaas gaan onze goederen achteruit in kwaliteit wanneer deze dichter bij de 
verkoopdatum komen. We hebben een systeem wat onze voorraad bijhoudt. 
Dit systeem is gemaakt door een knul genaamd Leeroy, wie sindsdien verder is gegaan met andere avonturen. 
Jouw taak is om het systeem te verbeteren en beter onderhoudbaar te maken. Allereerst een introductie van het systeem:

Alle goederen hebben een ‘sell_in’ waarde welke het aantal dagen aangeeft 
dat we hebben om deze te verkopen.
Alle goederen hebben een ‘quality’ waarde welke de waarde aangeeft
Aan het eind van de dag gaan deze allebei met een omlaag

Simpel toch? Maar dit is waar het interessant wordt:

* Zodra de verkoop datum voorbij is vergaat iets twee keer zo snel
* De waarde is nooit negatief
* “Aged Brie” wordt juist meer waard, hoe ouder het wordt.
* De kwaliteit kan nooit meer dan 50 zijn.
* “Sulfuras, Hand of Ragnaros'”, een legendarisch item, gaat nooit achteruit in kwaliteit, of in verkoopdatum.
* “Backstage passes to a TAFKAL80ETC concert”, net als “Aged Brie”, worden meer waard naarmate ze dichter bij de verkoop datum worden;
  * De waarde gaat met 2 omhoog wanneer er 10 of minder dagen tot de verkoopdatum zijn, en zelfs met 3 wanneer er 5 of minder dagen zijn tot de verkoopdatum. Maar de waarde daalt naar 0 op het moment dat de verkoopdatum verstreken is.

En ter duidelijkheid, een item kan nooit een kwaliteit hoger hebben dan 50, behalve “Sulfuras, Hand of Ragnaros'”, 
omdat deze legendarisch is. Deze kan een kwaliteit van maximaal 80 hebben. Wij zorgen ervoor dat de Items de correcte 
waardes hebben als we ze invoeren, dus dit hoeft het systeem niet na te kijken.

## Jouw opdracht

Jouw opdracht bestaat uit de volgende punten:

1. Zorg dat alle oude functionaliteit hetzelfde blijft.
2. Refactor de code zodat deze leesbaarder wordt.

Je mag zoveel aanpassingen maken in de ‘tick’ methode, zolang alles maar blijft werken zoals het nu doet. 
De Item class, en de constructor van de Store class mag je niet aanpassen. 
Deze gebruiken we ook nog in andere systemen, dus die zouden kapot gaan als je deze aanpast.


## Belangrijk

Omdat we zeker willen weten dat alles goed blijft werken, zal je moeten checken of dingen nog werken met behulp van de
`test.php` file. Door `php test.php` te runnen kan je zien hoe de lijst er na elke dag uit ziet. Je kan zelfs nog het
aantal dagen specificeren (`php test.php 5`) draait voor 5 dagen.

## Inleveren

Om het in te leveren kan je `./pack.sh` runnen in je terminal (git bash voor windows).
Vervolgens kan je de `results.tar.gz` file inleveren. De link voor het inleveren krijg je aan het begin van de opdracht.
Mocht je problemen hebben bij het inleveren dan moet je dit maar even laten weten.
