US-Burn (für USB-Portbrenner Brenner8/9) V1.8a3 (10.08.2008)
============================================================

Das ist die dritte Version von US-Burn 1.8. Sie unterstützt den Brenner8 für 5V-PICs wie auch den Brenner9, der 3,3V-PICs-brennen kann.



Allgemeines
===========

Dies ist ein Windowsprogramms zur Ansteuerung meines Brenners8/9.

Mit einem Brenner 8 werden 14- und 16-Bit-Kern-PICs sowie einige 24-Bit Signalcontroller unterstützt. 
Das sind die Serien PIC18Fxxxx, PIC16Fxxx, dsPIC30Fxxxx und viele PIC12Fxxx.
Das Programm benötigt dafür einen Brenner8 mit Firmware 0.10 und der Database 16. All das befindet sich in dieser ZIP-Datei

Mit einem Brenner 9 werden 3,3V-PICs der Serien PIC24F, PIC24H, dsPIC33 sowie PIC18FxxJxx unterstützt. 
Das Programm benötigt dafür einen Brenner9 mit Firmware 3.10 und der Database 16. All das befindet sich in dieser ZIP-Datei



Das Programm wurde von mit für viele PIC-Typen unter WinXP/Win2k getestet, kann aber prinzipiell unter WinXP, Win2k, WinNT, WinVista sowie Win98/me brennen.
Für Win98/me empfehle ich die Nutzung aber nicht.



Installation:
============
Das Zip-File in einen Ordner entpacken. Den Treiber 
(Unterverzeichnis driver) gleich installieren, oder nach dem Anschluß 
des Brenner8/9 auf Forderung von Windows installieren.

Es gibt zwei unterschiedliche Treiber zur "Auswahl". Der ältere unterstützt noch Win98/me wärend der neuere WinVista unterstützt. Für Win2k und WinXP sind beide Treiber geeignet.

Die 6 im ZIP-File enthaltenen Dateien xx03.dat müssen ebenfalls 
in das gleiche Verzeichnis wie usburnxx.exe kopiert werden. Sie stellen die Database dar.

Beim Start legt US-Burn eine Datei namens usburn.ini im
Programmverzeichnis an.



Umstieg von US-Burn1.7
======================
Wenn der Brenner8/9 einen Botloader enthält, kann die Firmware 0.11 (b8_fw_0_11.hex) bzw 3.10 (brenner9fw10.hex)
von US-Burn in den Brenner geladen werden. Ansonsten zuerst den Bootloader mit einem anderen Brenner in den SteuerPIC brennen.
Ich empfehle beim Brenner8 danach den Punkt 3 der Kalibrierung zu wiederholen. Dafür
ist keine Messtechnik nötig. Für den Brenner9 ist keine Kalibrierung nötig



Bekannte Probleme:
==================

- 16F639 wird als 16F636 behandelt (kein wirkliches Problem)
- 16F83 muß als 16F84 gebrannt werden
- 60- & 80-polige PICs müssen über die ICSP-Verbindung gebrannt werden.
- dsPIC30F-Typen müssen über die ICSP-Verbindung gebrannt werden.
- alle 3,3V-Typen müssen über die ICSP-Verbindung gebrannt werden.



Änderung in US-Burn V1.8a3
===========================
- Anpassung an Konfigurationsoptinen mit mehr als 16 Einstellmöglichkeiten


Änderung in US-Burn V1.8a2
===========================
- kann HEX-Files verarbeiten, die unter Linux erstellt wurden


Änderung in US-Burn V1.8a1
===========================
- Erkennung und Vermeidung der "ICD/ICSP PortEnable bit"-Falle
- "Reanimierung" von PIC18Fxxxx, die nach korrektem Brennen nicht mehr erkannt werden
- Bugfix im Reassembler für 12-Bit-Kern-PICs


Änderung in US-Burn V1.7a6
===========================
- Verbesserte PIC-Typ-Auswahl
- Vorbereitung für das Brennen von 12-Bit-PICs (PIC10F20x u.ä.) mit der Fw11


Änderung in US-Burn V1.7a2
===========================
- USBurn bietet nun nur die PIC-Familien zum Brennen an, die von der Brennerhardware auch unterstützt werden.
- Reassembler für dsPIC30/33/PIC24 integriert


Änderung in US-Burn V1.7a1
===========================
- Integration des Brenner9 mit PIC24, dsPIC33 und PIC18FxxJxx


Änderung in US-Burn V1.5rc2
===========================
- kleinere Korrekturen
- Laden des HEX-Feiles ist erst nach korrekter PIC-Typ-Erkennung möglich
- Unterstützung der Speisung von Testplatinen mit 5V/100mA (ab Fw 0.9)
 

Änderung in US-Burn V1.5rc1
===========================
- Unterstützung der dsPIC30Fxxx
 

Änderung in US-Burn V1.4
========================
- Unterstützung der RUN-Funktion ab Firmware 0.8
- Bugfix für PIC18F2410 / PIC18F2420 / PIC18F2450 
             PIC18F4410 / PIC18F4420 / PIC18F4450 


Änderung in US-Burn V1.3
========================
- unsinnige OSCCAL-Behandlung bei einigen PIC18Fxxxx deaktiviert 
- Memory-Map an PIC18Fxxxx angepaßt 
- kann mit Firmware V0.6 die Kalibrierdaten im Brenner speichern 
- Bugfix: Auslesen von PICs mit mehr als 256 Byte EEPROM 
- Bugfix: Auslesen von PIC18Fxxxx 
- kann Firmware in den Steuerpic schreiben 
  (wenn mindestens FW V0.6 & Bootloader V1.0 im Brenner sind)


Änderung in US-Burn V1.2a
=========================
- Absturz beim auslesen leerer PIC16Fxxx beseitigt
- Absturz beim Reassemblieren einiger PIC16F-Hex-Files beseitigt


Änderung in US-Burn V1.2
========================
- Fehler beim Brennen genau einer EEPROM-Zelle behoben
- Unterstützung für PIC18F-Typen


Änderung in US-Burn V1.1g
=========================
- Unterstützung für PIC18F-Typen (ohne Memory Map)
- überarbeitete Vpp-Regelung
- benötigt Firmware V 0.5
- kleine Bugfixes


Änderung in US-Burn V1.1(e)f1
=============================
- Prüfung der bebrannten Config verbessert für PICs mit Bandgap-Einstellung
  und für PICs mit unbenutzten Config-Bits (z.B. 12F675)


Änderung in US-Burn V1.1(e)
===========================
- Brennfehler bei Config und ID einer Typen (16F87xA) beseitigt
- viele kleinere Bugs beseitigt
- benötigt Brenner8-Firmware 0.4
- benötigt Database 10



Änderung in US-Burn V1.1(c)
===========================
- Bug verursachet Ansturz beim Brennen leerer ID-Zellen



Über positive und 
negtive Erfahrungen berichtet bitte an:
mailto: sprut@sprut.de


sprut 10.08.2008
http://www.sprut.de
