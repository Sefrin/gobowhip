
# Prozedurale Generierung

brainstorming zu dynamischen inhalten

## Terrain

### Idee: Rasterung

aufteilung von welt in kacheln (quadrate). eine kachel hat einen kacheltyp. kacheltyp definiert, in welchen richtungen (nord, süd, west, ost) die kachel verbunden mit einer anderen bzw. nicht passierbar ist. damit lässt sich eine karte als eine 2d-matrix von integern darstellen. an dem punkt verlagert sich das problem:

1. eine "abbildung" von der datenstruktur (2d-matrix) auf 3d-modelle finden (handwerk)
2. dynamisches generieren der 2d-matrix (kunst). wenn die generierung ein bild als eingabe bekommen würde, dann würde sich das problem wieder verlagern auf das dynamische erzeugen einer bilddatei. 
3. dies hätte den nebeneffekt, dass man zum testen manuell gemalte bilder einfüttern könnte. das bild müsste dann gewissen anforderungen genügen, wie nur zwei mögliche werte (passierbar oder hindernis) oder "anfang" muss mit "ende" verbunden sein oder so.

der vorgang wäre, glaube ich, relativ leicht umzusetzen. das ist ein vorteil. nachteil ist, dass man von bild zu 2d-matrix weniger freiheiten hat. außerdem ist diese rasterung evtl etwas uncool weil steif, aber das kommt vllt auf die umsetzung an.

ich glaube, bei prozeduraler generierung passiert hauptsächlich, dass einzelne bauteile hübsch zusammengesteckt werden. wie aufregend dann das ergebnis ist, hängt von der anzahl und der kombinierbarkeit der bauteile ab. für ein spannendes ergebnis brauchen wir also entweder wenige kleine und sehr flexible bauteile (lego) oder sehr viele, grobe bauteile (playmobil). theoretisch könnte man noch eine zwischenebene einbauen und sagen: wir bauen uns unser playmobil aus lego zusammen. das wäre prozedural hoch zwei und das ergebnis wäre sicherlich sehr fancy. aber das klingt auch irgendwie... nach arbeit. 😊
