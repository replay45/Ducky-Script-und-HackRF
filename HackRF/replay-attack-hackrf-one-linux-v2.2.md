# "Replay Attack" mit einem HackRF one


`Betriebssystem des PCs: Kali Linux (in einer virtuellen Maschine)`

`Der HackRF one ist über USB an den PC angeschlossen.`

`Diese Anleitung wurde am 10.8.2023 verfasst.`


> [Link zum HackRF](https://greatscottgadgets.com/hackrf/one/)


----------------------------------------------------------------------------------------------------------------


- zusätzliche Information:
	- Es wird nur die Komandozeile benötigt.


## Hinweis zum PortaPack:
`Der Hackrf muss entweder mit der originalen Software (ohne Zubehör) betrieben werden, oder sofern ein mobiles "porta-pack" vorliegt,
in den "hackrf-mode" geschaltet werden, um diesen mit dem PC nutzen zu können !`

## WICHTIG
`Es muss eine Antenne am HackRF angeschlossen sein !`


----------------------------------------------------------------------------------------------------------------


1. Installation von [GQRX](https://www.gqrx.dk/) (SDR-Software)

```
$ sudo apt install gqrx-sdr
```


----------------------------------------------------------------------------------------------------------------


2. optionaler Schritt

Um Informationen über den angeschlossenen HackRF zu erhalten, den Befehl ausführen:

```
$ hackrf_info
```


----------------------------------------------------------------------------------------------------------------


3. Aufzeichnen der angegebenen Frequenz, um diese zu einem späteren Zeitpunkt über den HackRF zu senden:

```
$ hackrf_transfer -r hier-der-dateiname.raw -f 433900000 -l 20 -g 20
```

a) `.raw` ist das Dateiformat der Aufnahme.

b) Die Zahl `433900000` ist die Frequenz in Mhz die aufgezeichnet wird.

c) Der Parameter `-r` beschreibt den Dateinamen der `.raw` Datei.

d) Die Parameter `-l` und `-g` geben die Werte der Signalverstärkung an.


----------------------------------------------------------------------------------------------------------------


4. Die Aufzeichnung der angegebenen Frequenz wird über diesen Befehl gesendet, um die "Attacke" auszuführen:

```
$ hackrf_transfer -t hier-der-dateiname.raw -f 433900000 -x 40
```

a) `.raw` ist das Dateiformat der Aufnahme.

b) Die Zahl `433900000` ist die Frequenz in Mhz die aufgezeichnet wird.

c) Der Parameter `-t` beschreibt den Dateinamen der `.raw` Datei, die gesendet werden soll.

d) Der Parameter `-x` gibt die Werte der Signalverstärkung an.



`Nun wurde die aufgenommene Frequenz gesendet und der "Replay-Attack" wurde ausgeführt !`




----------------------------------------------------------------------------------------------------------------
