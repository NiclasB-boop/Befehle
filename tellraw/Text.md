# Text-Optionen
```json
"text",  "selector", "nbt", "score", "keybind", "translate"
```
## Algemein
* In Anführungszeichen wird die Option ausgewählt.
* Danach kommt ein Doppelpunkt.
* Zum Schluss kommt der Wert der Aktion in Anführungszeichen.

## ```"text"```
* Zeigt einen Text.  
```json
"text":"<Text>"
```
### Beispiele:  
```mcfunction
/tellraw @s {"text":"Hallo, Welt!"}
```
➡ Zeigt den Text "Hallo, Welt!".  
```mcfunction
/tellraw @s {"text":"Text"}
```
➡ Zeigt den Text "Text".
## ```"selector"```
* Zeigt einen Selektor.  
```json
"selector":"<Selektor>"
```
### Beispiele:  
```mcfunction
/tellraw @s {"selector":"@s"}
```  
➡ Zeigt dem Spieler, der den Befehl ausführt, den Namen des Spielers der den Befehl ausführt.
```mcfunction
/tellraw @a {"seleector":"@e"}
```
➡ Zeigt jedem Spieler den Namen jedes Spielers.
## ```nbt```
* Zeigt eine bestimmte Nbt-Data.  
```json
"nbt":"<Nbt Data>","entity":"<Ziel>"
```  
### Beispiele:  
```mcfunction
/tellraw @a {"nbt":"Health","entity":"@s"}
```  
➡ Zeigt jedem Spieler die Lebensanzahl des Spielers der den Befehl ausführt.
```mcfunction
/tellraw @a {"nbt":"Air","entity":"@e"}
```  
➡ Zeigt jedem Spieler wie lange jeder Entity noch Atmen kann.
## ```score```
* Zeigt einen Wert eines scoreboards.
```json
"score":{"name":"<Ziel>","objective":"<Scoreboard>"}
```
### Beispiele:  
```mcfunction
/tellraw @a {"score":{"name":"@s","objective":"Punkte"}}
```
➡ Zeigt jedem Spieler den score des Scoreboards "Punkte" von dem Spieler der den Befehl ausführt.
## ```keybind```
* Zeigt denjenigen die die Nachricht geschickt bekommen ihre Tastenbelegung, die sie in dem Moment in dem der Befehl ausgeführt wird haben, einer bestimmten Aktion (Vorwärts laufen, Angreifen/Abbauen, ...). Ist die Aktion nicht belegt wird "Nicht belegt gesendet".
```json
"keybind":"<Aktion>"
```
### Beispiele:  
```mcfunction
/tellraw @a {"keybind":"key.forward"}
```  
➡ Zeigt jedem Spieler seine Tastenbelegung für's Vorwärts laufen.  
## ```translate```
* Zeigt einen in die Sprache des Spielers übersetzen Text (nur das was in den Minecraft Daten ist (Diamant, Einzelspieler, ...)).
```json
"translate":"<Wort>"
```
### Beispiele:  
```mcfunction
/tellraw @a {"translate":"block.minecraft.dirt"}
```
➡ Zeigt jedem Spieler eine Übersetzung des Wortes Erde.
```mcfunction
/tellraw @a {"translate":"block.minecraft.black_concrete"}
```
➡ Zeigt jedem Spieler die Übersetzung des Wortes Schwarzer Beton.
