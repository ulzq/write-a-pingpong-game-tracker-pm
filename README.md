# GameTracker
Application for hosting Pingpong Tournaments

- Arbeitet in Gruppen von vier bis fünf Leuten
- Verteilt unter euch die Aufgaben

## TODOs
### Benutzeroberfläche (HTML + CSS)
- Erstellt eine Zeichnung oder ein Layout von der Benutzeroberfläche, bevor ihr beginnt HTML und CSS zu schreiben
#### Elemente
- Spielerliste mit Punktzahl jedes Spielers
- Textfeld und Button um Spieler hinzuzufügen
- Button um Spiel zu starten
- Gegner-Namen
- Punkte-Anzeige für beide Gegner eines Spiels


### Logik (JavaScript)
#### Aufbau
- Meisterschaft-Objekt
  - Liste der Spieler
  - Liste der gespielten Spiele
  - Wieviele Spiele noch zu spielen
- Spiel-Objekt
  - Gegner
  - Sieger
- Spieler-Objekt
  - Punkte
  
- Objekt für Einstellungen
  - Anzahl der Sätze pro Spiel
#### Ablauf eines Turniers
- Spielername wird ins Textfeld eingetragen
- Bei Klick auf den Hinzufügen-Button, wird eine Funktion aufgerufen, die ein neues Spieler-Objekt mit dem Namen erstellt und in die Spieler-Liste im Turnier-Objekt hinzufügt
- Wenn alle Spieler eingetragen sind, klickt man auf den Start-Button
- Dies ruft eine Funktion auf, die eine neues Spiel-Objekt erstellt und es in die Spiele-Liste im Turnier-Objekt hinzufügt
- Beim Erstellen des Spiel-Objekts können als Parameter die beiden Gegner übergeben werden(für Final-Runden)
- Wenn keine Spieler übergeben werden, lost das Programm die Gegner aus
- Das spiel wird gestartet, es werden die Gegner-Namen angezeigt und darunter die Spieler-Punkte des aktuellen Spiels
- Unter jedem Gegner-Namen ist ein Button um signalisieren, dass der Gegner den Satz gewonnen hat
- Wenn dieser Button gedrückt wird, wird ein Punkt beim Gewinner hinzugefügt
- Wenn das Spiel zu ende ist, wird der Gewinner im Spiel-Objekt gespeichert
- Daraufhin wird das nächste Spiel mit neuen Gegnern erzeugt
- In den Finalspielen muss das Programm feststellen, wer die Gewwinner der Vorrundenspiele sind um die Gegner zu paaren
  
## Deployment
- Stellt euer Programm auf GitHub pages online

## Hilfe
###### Text aus Textfeld
```html
<input type="text" id="myText">
```
```javascript
var userInput = document.getElementById("myText").value
```

###### Inhalt in HTML-Element einfügen
```html
<ul id="myList">

</ul>
```
```javascript
document.getElementById("myList").innerHTML = "<li>Bees</li><li>Hornets</li>"
```
###### Auf Klick reagieren
```html
<button>Klick mich!<button>
```
```javascript
var button = document.querySelector('button')

function tellClick(){
  alert("Ich wurde geklickt!")
}

button.addEventListener('click', tellClick)
```
