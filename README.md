# Lennfotainment
## Einleitung
Lennfotainment ist eine moderne, minimalistische Innenanzeige nach Vorbild der "Infotainment"-Anzeige von LAWO.

## Bilder
![Screenshot 1](https://raw.githubusercontent.com/ma7t3s-OMSI-Sammlung/Lennfotainment/refs/heads/main/Screenshot/Screenshot%20(1).jpg)
![Screenshot 2](https://raw.githubusercontent.com/ma7t3s-OMSI-Sammlung/Lennfotainment/refs/heads/main/Screenshot/Screenshot%20(2).jpg)
![Screenshot 3](https://raw.githubusercontent.com/ma7t3s-OMSI-Sammlung/Lennfotainment/refs/heads/main/Screenshot/Screenshot%20(3).jpg)
![Screenshot 4](https://raw.githubusercontent.com/ma7t3s-OMSI-Sammlung/Lennfotainment/refs/heads/main/Screenshot/Screenshot%20(4).jpg)
![Screenshot 5](https://raw.githubusercontent.com/ma7t3s-OMSI-Sammlung/Lennfotainment/refs/heads/main/Screenshot/Screenshot%20(5).jpg)

### Features:
- Anzeigen der nächsten 4 Haltestellen, Linie, Ziel und Uhrzeit
- Haltewunsch
- dynmaische Verspätungsanzeige
- automatischer Dark Mode

**<ins>Achtung:</ins> Das ganze ist noch Beta, Fehler etc. können immer Auftreten, diese bitte gerne Issues melden, genau so, wie Verbesserungsvorschläge! :)**

---

## Einbau
Grundsätzlich am besten vorher eine alte, ggf. vorhandene Innenanzeige vollständig ausbauen, um Konflikte zu vermeiden :)
An sich lässt sich das ganze Relativ einfach einbauen, bereitgestellt werden die notwendigen model(mesh)-Dateien, Texturen und Scripts direkt in der passenden Ordnerstruktur, einfach in den Bus der Wahl kopieren.
Das Mesh muss natürlich ggf. mithilfe einer Daueranimation oder Blender an die richtige Stelle bewegt werden.
Außerdem liegt es als FBX-Datei zum selbst-exportieren bei.

als "model (Ausschnit).cfg" liegt ein Model.cfg-Abschnitt bei, den ihr euch in die model.cfg eures Busses einfügen müsst, Texttextur-Einträge müssen natürlich ggf. angepasst werden, ansonsten sollte der bereits so, angezeigt werden.

Damit sie auch das tut, was sie soll, brauchen wir noch die Macro-Auswführungen, dazu müsst ihr einmal in die main-Datei des Busses gehen (die sollte einen frame- und init-Abschnitt haben) und dort jeweils folgendes hinzufügen:
- `(M.L.Lennfotainment_frame)` unter `{frame}`

Dann noch in der *.bus-Datei folgendes hinzufügen:

**unter Varlist:**
- script\Lennfotainment\varlist.txt

**unter Strinvarlist:**
- script\Lennfotainment\stringvarlist.txt

**unter Script:**
- script\Lennfotainment\script.osc

Zuletzt braucht ihr noch die Open Sans-Font, dazu einfach das, was im Ordner "Fonts" bereitgestellt wird, entsprechend in den OMSI-Font-Ordner ziehen.

---

Das war tatsächlich schon alles. Derzeit ist die Innenanzeige nur mit dem [Nuntius-FIS](https://github.com/ma7t3s-OMSI-Sammlung/Nuntius) kompatibel, damit sollte es aber problemlos funktionieren.

**Viel Spaß!**
