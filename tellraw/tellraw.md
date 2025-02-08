# **tellraw**-Befehl

## Was macht er?
* Text an bestimmte Spieler schicken
* Der Text is formattierbar (Farbe, Kursiv, etc.)
* Er kann angeklickt werden:
  * Befehle ausführen
  * Links öffnen
  * Text kopieren

 ## Syntax
* ``` tellraw $Spieler$ {Optionen} ```
* **$Spieler$** ist die Zielperson, die die Naricht erhält.
* **$Optionen$** sind die Optionen, die man eingeben kann. Diese werden jeweils in Anführungstrichen geschrieben, danach folgt ein Doppelpunkt und dann entweder "true/false" ohne Anführungszeichen oder etwas anderes in Anführungszeichen. Mehrere Optionen werden mit Kommas getrennt.
  * ``` "text":"$Text$"``` : Gibt den Text der Naricht an
  * ``` "color":$Farbe$ ```: Gibt die Farbe des Textes an
 
## Beispiele
* ``` tellraw @s {"text":"Hallo!", "color":"red"} ```: Zeigt dem Spieler, der den Befehl ausführt, den Text "Hallo!" in roter Farbe.
* ``` tellraw @a {"text":"Test?!", "color":"#00ff00", "bold":true} ```: Zeigt jedem Spieler den Text "Test?" in grüner Farbe und dicker Schrift.
