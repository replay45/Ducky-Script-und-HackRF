# "Replay Attack" über den HackRF mit einem PortaPack


`Für diese Anleitung wurde ein PortaPack H1 verwendet.`

`verwendete Software: Meyhem v1.7.4`

`Diese Anleitung wurde am 13.8.2023 verfasst.`


> [Link zum HackRF](https://greatscottgadgets.com/hackrf/one/)

> [Link zum verwendeten PortaPack H1](https://store.sharebrained.com/products/portapack-for-hackrf-one-kit)

-----------------------------------------------------------------------------------------------------------------


## WICHTIG:
`Es muss eine Antenne angeschlossen sein !`


-----------------------------------------------------------------------------------------------------------------


1. Freuenz herausfinden

- Häufig schafft eine Google-Suche bei der ungefähren Suche nach der Frequenz Abhilfe.

- Um die genaue Frequenz herauszufinden, kann der `Scanner` verwendet werden.
	- Hierbei muss eine Frequenz als Start- und eine weitere als End-Frequenz für die Suche unter `SEARCH START` und `SEARCH END` angegeben werden.
	- Wenn eine Frequenz gefunden wurde, wird diese gelb angezeigt.
	- Die angezeigte Frequenz kann nun notiert werden.

Somit wurde die Frequenz ausfindig gemacht.



-----------------------------------------------------------------------------------------------------------------


2. Aufnehmen


- Die herausgefundene Frequenz einstellen:
	- Mit einem Klick auf die Frequenz direkt unter Capture, kann die gewünschte Frequenz eingegeben werden.
	- Optional kann diese mit "save" auch gespeichert werden.

- `Rate` beschreibt die Geschwindigkeit und Sichtweite des Wasserfalls.
   Sollte daher kein markierter Bereich zu erkennen sein, sollte die `Rate` verkleinert werden !

- Sobald ein Signal auf dem Wasserfall zu sehen ist, kann der Button `Rec` betätigt werden.
   Um die Aufnahme zu stoppen, muss einfach nur der nun erscheinende `Stop` Button betätigt werden.

- Nun wurde die Aufnahme lokal gespeichert und kann unter 
	- "utilities" 
	- "File manager"
	- "CAPTURES"

   gefunden werden.


-----------------------------------------------------------------------------------------------------------------


3. Wiedergeben

- Im Menü den Reiter `Replay` öffnen.
- Nun kann das `+` Symbol betätigt werden.
- Jetzt kann die letzte Datei geöffnet werden.
- Nach dem Klicken auf `OK`, ist die Datei nun ausgewählt.
- Optional kann `Loop` ausgewählt werden, um die Datei im loop zu senden.
- Beim Klicken auf das `Play-Symbol` wird die Datei abgespielt.
- Bei erfolgreichem Abspielen, erscheint der Wasserfall.




Der "Repaly-Attack" wurde erfolgreich ausgeführt.

-----------------------------------------------------------------------------------------------------------------
