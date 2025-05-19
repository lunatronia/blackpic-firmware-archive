Readme.txt zur Database 17  vom 04.04.2008 für PBrennerNG, P18, dsProg und USBurn
(basierend auf MPLAB-IDE 8.00)


Inhalt
======

- Allgemeines
- Warum wird die Database überarbeitet?
- Legende
- wichtige Änderungen im Vergleich zur Database4
- alle Änderungen (auch die unwichtigen) im Vergleich zur Database4




Allgemeines
===========

Die Database enthält folgende Files:
- cekdef03.dat
- cfgdef03.dat
- fildef03.dat
- picdef03.dat
- setdef03.dat
- texdef03.dat
Alle Dateien sind gemeinsam in das Programmverzeichnis des Brennprogramms  PBrennerNG und/oder P18 und/oder dsProg und/oder USBurn zu kopieren. Dort ersetzen sie die gleichnamigen Dateien der vorherigen Database.

- picdef3.dll
Diese Database erfordert die picdef3.dll-Datei in der Version ab 3.2 (vom 23.10.2006) oder jünger. Die passende Version liegt der Database bei.

Diese Text-Datei beschreibt im Folgenden die Änderungen der Database15 im Vergleich zu Database14.



Warum wird die Database überarbeitet?
=====================================

1.
Der Hersteller Microchip passt die Programmierparameter kontinuierlich dem real existierenden Silizium an, diese Änderungen übernehme ich. Dabei handelt es sich meist um eine Verlangsamung des Timings, gelegentlich aber auch um größere Eingriffe in den Ablauf der PIC-Programmierung. Solche Änderungen betreffen meist nur PIC-Typen, die sich erst kurze Zeit auf dem Markt befinden.

2.
Neue PIC-Typen müssen in die Database aufgenommen werden. 

3.
Fehler die ich in der Behandlung einzelner PICs gemacht habe, muss ich korrigieren.





wichtige Änderungen im Vergleich zur Database 16
================================================

Unmgenauigkeiten in der devid.id.mask blockierte die Erkennung von PIC18F2423/2523/4423/4523.

PIC18F2420 :  devid.idmask
PIC18F2520 :  devid.idmask
PIC18F4420 :  devid.idmask
PIC18F4520 :  devid.idmask



wichtige Änderungen im Vergleich zur Database 15
================================================

Wärend der Erstrellung der Database15 hatten sich leider Fehler eingeschlicjhen, die alle dsPIC30F-Typen betrafen.Diese Fehler wurden mit der Database16 korrigiert. Darüberhinaus gab es keine wesentlichen Änderungen.

alt: V. 15 vom 11.01.2008 (410 PIC-Typen) (davon werden 356 PICs durch meine Brennsoftware unterstützt)
neu: V. 16 vom 30.01.2008 (410 PIC-Typen) (davon werden 355 PICs durch meine Brennsoftware unterstützt)




wichtige Änderungen im Vergleich zur Database 14
================================================

Zu folgenden PIC-Typen gab es Änderungen, die sich direkt auf das Programmieren dieser Typen mit US-Burn, P18 oder PBrennerNG auswirken. Aufgelistet sind jeweils die Namen der geänderten Parameter, aber nicht deren Werte.

alt: V. 14 vom 10.09.2007 (390 PIC-Typen) (davon werden 336 PICs durch meine Brennsoftware unterstützt)
neu: V. 15 vom 11.01.2008 (410 PIC-Typen) (davon werden 356 PICs durch meine Brennsoftware unterstützt)



Veränderungen:

dsPIC30F2011es :  pgming.ovrpgm
dsPIC30F2012es :  pgming.ovrpgm
dsPIC33FJ128GP804 :  pgmmem.max 
dsPIC33FJ64GP802 :  pgmmem.max 
PIC24HJ256GP610 :  pgming.ovrpgm
PIC24HJ64GP504 :  devid.id
diverse PIC18FxxJxx: Blocksize



neu aufgenommene Typen die auch unterstützt werden sowie 
schon bekannte Typen, die nun ebenfalls unterstützt werden:

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


Die PIC24/dsPIC33F-Typen werden ab US-Burn 1.7 mit Brenner9/Fw10 unterstützt.
Die PIC10F-Typen und die PIC1xF5x/5xx-Typen werden mit Brenner8/Fw11 unterstützt.



Ende

sprut
(www.sprut.de)






