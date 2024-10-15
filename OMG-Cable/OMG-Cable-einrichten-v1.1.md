# OMG Cable & Ducky Script

## OMG Cable einrichten


### 1. Installation

- Firmware herunterladen & Python installieren:
	- [Firmeware herunterladen](https://github.com/O-MG/O.MG-Firmware)
	- [Treiber herunterladen](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
	- [Python herunterladen](https://www.python.org/) (Version 3.7 oder höher)

	- `pyserial module` installieren:
	```
	$ python -m pip install pyserial
	oder
    $ python3 -m pip install pyserial
	```

- `Entpacken der zip-Pakete nicht vergessen !`



### 2. flashen

- Für den Flash-Vorgang wird ein Programmer benötigt, der zwischen den PC und dem OMG-Cable gesteckt wird !

- Programmer zwischen OMG-Cable und den PC stecken
- Flasher starten:
	- Terminal öffnen, auf das richtige Laufwerk wechseln und mit dem Befehl `$ cd` in den Ordner wechseln, wo sich das Flash-Skript befindet.


- Befehl eingeben:
	- Windows:
	```
	$ python ./flash.py 
	oder
	$ python3 ./flash.py
	```
	- Linux: 
	```
	$ sudo python3 ./flash.py
	```

- SSID = WLAN Anzeigename

- Wenn das Flashen fertig ist, das Kabel und den Programmer entfernen und NUR das Kabel direkt in den USB Port stecken.
- Etwas warten und schauen, ob das WLAN aktiv ist und mit diesem verbinden (Natürlich wird es keine Internetverbindung geben).



--------------------------------------------------------------------------------------------------------------------------------------



### 3. WLAN-Verbindung & WEB UI

- Mit dem WLAN des OMG-Cable verbinden und im Browser `http://192.168.4.1` eingeben, um auf die WEB-UI zu gelangen.
- Bei der ersten Verbindung kann die Geschwindigkeit variieren.
- Wichtig: Das Gerät muss für die WLAN-Verbindung 2.4 Ghz (WLAN) unterstützen !



### 4. Payloads / Skripte

- In der WEB-UI gibt es einige Beispielskripte.
- Weitere Skripte sind in diesem Reopsitory zu finden.



### 5. OMG Cable Specs:

Hinweis: Je nach OMG-Cable Version/ Modell können die Spezifikationen abweichen !


- Interface: USB-C & USB-A
- Radio: 802.11b/g/n (2.4GHz)
- Power: 5v, 500mA
- Cable passthrough speed: USB 2.0 (480mhz)
- Cable passthrough charging: compatible with 5v power sources and USB PD sources (5v supplied with USB PD)
- Capacity: ~650,000 keystrokes of storage for Keylogger Edition
- Payload Syntax: DuckyScript, with modifications to support extra features




### 6. Links

> [Github-OMG](https://github.com/O-MG/O.MG-Firmware/wiki)

> [OMG-Setup](https://o.mg.lol/setup/OMGCable/)

> [Python3](https://www.python.org/)

> [install Python on Linux](https://docs.python-guide.org/starting/install3/linux/)



--------------------------------------------------------------------------------------------------------------------------------------
