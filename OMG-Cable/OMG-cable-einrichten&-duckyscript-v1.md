# OMG Cable & Ducky Script



# 1. OMG Cable einrichten


### 1. Installation
- Firmware Herunterladen & Python installieren:
	- Firmeware downloaden: https://github.com/O-MG/O.MG_Cable-Firmware/releases/tag/v2.0-20210923
	- Driver herunterladen: https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers
	- Python herunterladen: (Version 3.7 oder höher)

	- `"pyserial module"` installieren:
	```
	$ python -m pip install pyserial <-oder-> $ python3 -m pip install pyserial
	```

- `Entpacken der zip Pakete nicht vergessen !`



### 2. flashen

- Programmer und OMG-Cable in den PC einstecken
- Flasher starten:
	- Terminal öffnen, auf das richtige Laufwerk wechseln und mit dem Befehl `$ cd` in den Ordner wechseln, wo sich das Flash Skript befindet.


- Befehl eingeben:
	- Windows:
	```
	$ python ./flash.py <-oder-> $ python3 ./flash.py
	```
	- Linux: 
	```
	$ sudo python3 ./flash.py
	```

- SSID = WLAN Anzeigename

- Wenn das Flashen fertig ist, das Kabel und den Programmer entfernen und NUR das Kabel direkt in den USB Port stecken.
- Etwas warten und schauen, ob das WLAN aktiv ist und mit diesem verbinden (Natürlich wird es keine Internetverbindung geben).



--------------------------------------------------------------------------------------------------------------------------------------



### 3. WEB UI Verbindung

- Mit dem WLAN verbinden und im Browser `192.168.4.1` eingeben.
- Bei der ersten Verbindung kann die Geschwindigkeit variieren.
- Wichtig: Das Gerät muss für die Verbindung mit der WEB-UI, 2.4 Ghz (WLAN) unterstützen !



### 4. Payloads / Skripte
- In der WEB-UI gibt es einige Beispielskripte.
- Weitere Skripte sind in diesem Reopsitory zu finden.



### 5. OMG Cable Specs:
Hinweis: Je nach OMG-Cable Version/ Modell können die Spezifikationen abweichen !


- Interface: USB-C & USB-A
- Radio: 802.11b/g/n (2.4GHz)
- Power: 5v, 500mA
- Cable passthrough speed: USB 2.0 (480mhz)
- Cable passthrough charging: compatible with 5v power sources and USB PD sources(5v supplied with USB PD)
- Capacity: ~650,000 keystrokes of storage for Keylogger Edition
- Payload Syntax: DuckyScript, with modifications to support extra features




### 6. Webseiten
> [Github-OMG](https://github.com/O-MG/O.MG_Cable-Firmware/wiki)

> [OMG-Setup](https://o.mg.lol/setup/OMGCable/)

> [Python3](https://www.python.org/)

> [install Python on Linux](https://docs.python-guide.org/starting/install3/linux/)



--------------------------------------------------------------------------------------------------------------------------------------



# 2. Befehlsübersicht von DuckyScript


## 1. Übersicht:

- REM: Der REM-Befehl wird verwendet, um Kommentare im Skript einzufügen, die nicht ausgeführt werden.
- DELAY: Der DELAY-Befehl legt eine Verzögerung zwischen den Befehlen fest, die ausgeführt werden.
- STRING: Der STRING-Befehl wird verwendet, um Text in das Ziel-System einzufügen.
- MENU: Der MENU-Befehl wird verwendet, um das Kontextmenü aufzurufen.
- RUN: Der RUN-Befehl wird verwendet, um ein bestimmtes Programm oder eine Datei auszuführen.




## 2. Tastatur-Optionen:

- ENTER: Der ENTER-Befehl simuliert das Drücken der Eingabetaste.
- TAB: Der TAB-Befehl simuliert das Drücken der Tabulatortaste.
- SHIFT: Der SHIFT-Befehl wird verwendet, um die Umschalttaste zu drücken.
- ALT: Der ALT-Befehl wird verwendet, um die Alt-Taste zu drücken.
- GUI: Der GUI-Befehl wird verwendet, um die Windows- oder Command-Taste auf einem Mac zu drücken.
- CONTROL: Der CONTROL-Befehl wird verwendet, um die Strg-Taste zu drücken.
- UP und DOWN: Diese Befehle können verwendet werden, um Pfeiltasten auf der Tastatur zu simulieren.
- ESC: Der ESC-Befehl wird verwendet, um die Escape-Taste zu drücken.
- CAPSLOCK: Aktiviert oder deaktiviert die Caps-Lock-Taste.
- NUMLOCK: Aktiviert oder deaktiviert die Num-Lock-Taste.
- SCROLLLOCK: Aktiviert oder deaktiviert die Scroll-Lock-Taste.
- HOME und END: Simulieren die Home- und End-Tasten.
- PAGEUP und PAGEDOWN: Simulieren die Page-Up- und Page-Down-Tasten.




## 3. Maus-Optionen:

- MOUSEMOVE: Bewegt die Maus an eine bestimmte Position auf dem Bildschirm.
- CLICK: Klickt mit der linken Maustaste.
- RIGHTCLICK: Klickt mit der rechten Maustaste.
- MIDDLECLICK: Klickt mit der mittleren Maustaste.
- DOUBLECLICK: Doppelklickt mit der linken Maustaste.
- SCROLL: Scrollt aufwärts oder abwärts.



-------------------------------------------------------------------------------------------------------------------------------------
