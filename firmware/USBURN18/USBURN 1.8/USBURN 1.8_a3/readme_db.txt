Readme.txt zur Database 17  vom 04.04.2008 f�r PBrennerNG, P18, dsProg und USBurn
(basierend auf MPLAB-IDE 8.00)


Inhalt
======

- Allgemeines
- Warum wird die Database �berarbeitet?
- Legende
- wichtige �nderungen im Vergleich zur Database4
- alle �nderungen (auch die unwichtigen) im Vergleich zur Database4




Allgemeines
===========

Die Database enth�lt folgende Files:
- cekdef03.dat
- cfgdef03.dat
- fildef03.dat
- picdef03.dat
- setdef03.dat
- texdef03.dat
Alle Dateien sind gemeinsam in das Programmverzeichnis des Brennprogramms  PBrennerNG und/oder P18 und/oder dsProg und/oder USBurn zu kopieren. Dort ersetzen sie die gleichnamigen Dateien der vorherigen Database.

- picdef3.dll
Diese Database erfordert die picdef3.dll-Datei in der Version ab 3.2 (vom 23.10.2006) oder j�nger. Die passende Version liegt der Database bei.

Diese Text-Datei beschreibt im Folgenden die �nderungen der Database15 im Vergleich zu Database14.



Warum wird die Database �berarbeitet?
=====================================

1.
Der Hersteller Microchip passt die Programmierparameter kontinuierlich dem real existierenden Silizium an, diese �nderungen �bernehme ich. Dabei handelt es sich meist um eine Verlangsamung des Timings, gelegentlich aber auch um gr��ere Eingriffe in den Ablauf der PIC-Programmierung. Solche �nderungen betreffen meist nur PIC-Typen, die sich erst kurze Zeit auf dem Markt befinden.

2.
Neue PIC-Typen m�ssen in die Database aufgenommen werden. 

3.
Fehler die ich in der Behandlung einzelner PICs gemacht habe, muss ich korrigieren.





wichtige �nderungen im Vergleich zur Database 16
================================================

Unmgenauigkeiten in der devid.id.mask blockierte die Erkennung von PIC18F2423/2523/4423/4523.

PIC18F2420 :  devid.idmask
PIC18F2520 :  devid.idmask
PIC18F4420 :  devid.idmask
PIC18F4520 :  devid.idmask



wichtige �nderungen im Vergleich zur Database 15
================================================

W�rend der Erstrellung der Database15 hatten sich leider Fehler eingeschlicjhen, die alle dsPIC30F-Typen betrafen.Diese Fehler wurden mit der Database16 korrigiert. Dar�berhinaus gab es keine wesentlichen �nderungen.

alt: V. 15 vom 11.01.2008 (410 PIC-Typen) (davon werden 356 PICs durch meine Brennsoftware unterst�tzt)
neu: V. 16 vom 30.01.2008 (410 PIC-Typen) (davon werden 355 PICs durch meine Brennsoftware unterst�tzt)




wichtige �nderungen im Vergleich zur Database 14
================================================

Zu folgenden PIC-Typen gab es �nderungen, die sich direkt auf das Programmieren dieser Typen mit US-Burn, P18 oder PBrennerNG auswirken. Aufgelistet sind jeweils die Namen der ge�nderten Parameter, aber nicht deren Werte.

alt: V. 14 vom 10.09.2007 (390 PIC-Typen) (davon werden 336 PICs durch meine Brennsoftware unterst�tzt)
neu: V. 15 vom 11.01.2008 (410 PIC-Typen) (davon werden 356 PICs durch meine Brennsoftware unterst�tzt)



Ver�nderungen:

dsPIC30F2011es :  pgming.ovrpgm
dsPIC30F2012es :  pgming.ovrpgm
dsPIC33FJ128GP804 :  pgmmem.max 
dsPIC33FJ64GP802 :  pgmmem.max 
PIC24HJ256GP610 :  pgming.ovrpgm
PIC24HJ64GP504 :  devid.id
diverse PIC18FxxJxx: Blocksize



neu aufgenommene Typen die auch unterst�tzt werden sowie 
schon bekannte Typen, die nun ebenfalls unterst�tzt werden:

PIC10F200 
PIC10F202 
PIC10F204 
PIC10F206 
PIC10F220
PIC10F222 
PIC12F510 
PIC12F519 

PIC16F506 
PIC16F526 

PIC18F6393 
PIC18F6493 
PIC18F8393 
PIC18F8493 

dsPIC30F6010es

dsPIC33FJ16GP304
dsPIC33FJ16MC304
dsPIC33FJ32GP202 
dsPIC33FJ32GP204
dsPIC33FJ32MC202 
dsPIC33FJ32MC204 

PIC24FJ16GA002 
PIC24FJ16GA004 
PIC24FJ48GA002 
PIC24FJ48GA004 
PIC24HJ16GP304 

PIC24HJ32GP202
PIC24HJ32GP204 
PIC24HJ64GP502

PIC18F24K20
PIC18F25K20
PIC18F26K20 
PIC18F44K20 
PIC18F45K20 
PIC18F46K20 


Die PIC24/dsPIC33F-Typen werden ab US-Burn 1.7 mit Brenner9/Fw10 unterst�tzt.
Die PIC10F-Typen und die PIC1xF5x/5xx-Typen werden mit Brenner8/Fw11 unterst�tzt.



Ende

sprut
(www.sprut.de)






