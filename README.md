# AskSinPP-Collection-HM-RC-4-Homematic

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/Bild%201.jpg)


AskSinPP Collection HM-RC-4 Homematic
 
Achtung! Dies ist ein DIY Projekt! Dieses Gerät hat kein CE Zeichen und ist auch nicht getestet! Verwendung auf eigene Gefahr, der Designer übernimmt keine Haftung!
Danksagung: Vielen Dank an Jerome Pecht, Papa aus dem Homematicforum, Christoph Wichert und Ronny Thomas. Ohne Euch würde es keine Homematic Selbstbauprojekte geben.
https://www.youtube.com/watch?v=ih9aKctOBqA&feature=youtu.be

Materialliste:

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/material.jpg)
 
•	1 mal M2 Mutter
•	1 mal M2 Zylinderkopfschraube 2* 8 mm 
https://www.ebay.de/itm/Sortiment-Set-Edelstahlschrauben-DIN-933-912-7991-603-ISO-7380-VA-A2-V2A-A4-V4A/282511902775?ssPageName=STRK%3AMEBIDX%3AIT&var=581669311814&_trksid=p2057872.m2749.l2649

•	1 mal Streifenlochraster Platine 2,54 mm Rastermaß L/B = 43,2 * 15,7 mm 
https://www.ebay.de/itm/10x-Lochraster-Kupferplatine-verzinnt-2-54mm-Punkte/192927197041?hash=item2ceb5b6771:g:2qYAAOxy7odR5Zvi

•	4 mal Sourcingmap® Metalle Batterie-Federplatte der AA-Batterien
https://www.amazon.de/gp/product/B00O9XV66Q/ref=ppx_yo_dt_b_asin_title_o08_s00?ie=UTF8&psc=1

•	4 Micro schrauben M1,2 *5 mm
https://www.ebay.de/itm/100x-Miniatur-Blechschrauben-Schraube-mini-Schrauben-Blechschraube-micro/362429856292?hash=item546280ba24:m:mJtqVx7XlX0KviVUEFpc3Ag 

•	1 mal Platine (Micro) von Ronny Thomas 
https://github.com/ronnythomas/HB-Micro Kontakt siehe Github link.

•	1 mal Arduino Pro Mini ATmega328P (3.3V/8MHz)
https://de.aliexpress.com/item/32342672626.html?spm=a2g0s.9042311.0.0.27424c4dEtMdJk

•	1 mal CC1101 Funkmodul (868 MHz)
https://de.aliexpress.com/item/32852371777.html?spm=a2g0s.9042311.0.0.27424c4dEtMdJk

•	1 mal FTDI Adapter (wird nur zum flashen benötigt)
https://www.ebay.de/c/783482994

•	5 mal Taster 6*6
o	https://www.ebay.de/itm/10X-MIKROSCHALTER-MICRO-TASTER-SCHALTER-MINI-SMD-MINIATUR-6X6X5MM-50MA/263833669383?hash=item3d6db64f07:m:mkAIpszraMfYR8TxEA2aWUg

•	1 mal LED Rechteckig 2x5x7mm 
https://www.ebay.de/itm/LED-Rechteckig-Blau-Klar-2x5x7mm-1-10-25-50-Stuckzahl-wahlbar-2x5mm-C3649/292916276045?hash=item44332bab4d:m:mhM67zhQZfejVZ2-7A0JYmg

•	1 mal Widerstand 330 Ohm
https://www.ebay.de/itm/300-Metallfilm-Widerstande-30-Werte-x-10-Stuck-Widerstand-Sortiment-Set-Kit/253032009728?hash=item3ae9e21000:g:5hQAAOSwqxdb33eO

•	DC/DC Wandler BL8530
https://www.ebay.de/itm/10Pcs-BL8530-BL8531-0-8-3-3V-To-3-3V-DC-DC-Converter-Step-Up-Boost-Module/392313683179?hash=item5b57b7bceb:g:xScAAOSwXMxb45ad

•	Stiftpolleiste RM 2.0
https://www.reichelt.de/10pol-stiftleiste-gerade-rm-2-00-sl-1x10g-2-00-p51693.html?&GROUP=C141&START=0&SORT=artnr&OFFSET=16

•	Div. Litzendraht



Grundlagen / flashen / Anlernen an die CCU:
https://asksinpp.de/
Sketch:
https://github.com/jp112sdl/Beispiel_AskSinPP/blob/master/examples/HM-PBI-4-FM/HM-PBI-4-FM.ino

1.	Teile Ausdrucken https://www.thingiverse.com/thing:3667980
-	1 mal No.1  Oberschale.lst / Support setzten!
-	2 mal No. 2 Unterschale.lst
-	1 mal Tasten 1-4.lst

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/Bild%202.JPG)
 
2.	Platine zusammen löten. Als Antenne kann man einfach einen „Klingeldraht“  benutzen (8,3 mm lang)

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/Bild%203.JPG)


Wichtig! LED Rechteckig 2x5x7mm muss wie im Bild um 90 Grad umgebogen werden und so abgelötet werden

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/Bild%204.jpg)
 

3.	6 Litzen (ca. 10 cm lang) am Arduino anlöten, Siehe Bezeichnung auf Platine 

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/Bild%205.JPG)
 

4.	Lochraster Platine 
-	Lochraster hat die exakten Masse 42,2 * 15,7 mm, zur Orientierung die „Kupferfelder“ zählen und auf dieses Maß zu sägen
-	4 Löcher mit 1,5 mm Bohrer wie im Bild aufbohren
-	Mircotaster wie abgebildet auf Lochraster positionieren und verlöten
 
 ![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/bild%206.jpg)

-	Tasten in die Oberschale einlegen
-	Lochraster mit Micotaster einbauen und festziehen

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/tasten.jpg)
 
5.	BL8580 DC/DC Step-Up und Batterie-Federplatte wie im Bild einsetzten und Litzendrähe anlöten

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/bild%207.jpg)

6.	Arduino in die Oberschale einschieben. Antenne seitlich um den Pro Mini legen. 
 
![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/bild%208.jpg)

7.	M2 Mutter in die Unterschale einkleben
 
![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/bild%209.jpg)

 
8.	Arduino mit Isoband abkleben, das ist nötig da die Litzendrähte sich leicht an den Lötpins verhacken

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/bild%2010.JPG)
 
9.	Ober- und Unterschale vorsichtig zusammen setzen und mit M2 Schraube sichern 

![alt text](https://github.com/Schmelzerboy/AskSinPP-Collection-HM-RC-4-Homematic/blob/master/bild%2011.JPG)


Fertig


