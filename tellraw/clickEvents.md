# clickEvents
## Was sind clickEvents
* Wenn man den Text anklickt, wird etwas bestimmtes ausgeführt.
## Verfügbare clickEvents
```json
run_command, suggest_command, copy_to_clipboard, open_url
```
## Algemeine Syntax:
* Statt " muss \" geschrieben werden.
```json
"clickEvent":{"action":"<clickEvent>","value":"<Text/Link/Befehl>"}
```
## ```run_command```
* Führt einen Befehl aus, wenn der Text angeklickt wird.
```json
"clickEvent":{"action":"run_command","value":"<Befehl>"}
```
### Beispiele:
```mcfunction
/tellraw @a {"text":"Diamant","clickEvent":{"action":"run_command","value":"/give @s diamond"}}
```
➡ Zeigt jedem Spieler den Text "Diamant" und wenn er angeklickt wird kriegt derjenige einen Diamanten.
```mcfunction
/tellraw @a {"nbt":"Health","entity":"@s","clickEvent":{"action":"run_command","value":"/kill @s"}}
```
➡ Zeigt jedem Spieler den Text die Lebensanzahl des Spielers der den Befehl ausführt und wenn er angeklickt wird stirbt derjenige der ihn angeklickt hat.
## ```suggest_command```
* Schreibt etwas in die Textzeile, wenn der Text angeklickt wird.
```json
"clickEvent":{"action":"suggest_command","value":"<Text>"}
```
### Beispiele:
```mcfunction
/tellraw @a {"text":"Hallo","clickEvent":{"action":"suggest_command","value":"Hallo"}}
```
➡ Zeigt jedem Spieler den Text "Hallo" und wenn der Text angeklickt wird, wird "Hallo" in die Textzeile geschrieben.
```mcfunction
/tellraw @a {"text":"\"Hallo\"","clickEvent":{"action":"suggest_command","value":"\"Hallo\""}}
```
➡ Zeigt jedem Spieler den Text ""Hallo"" und wenn der Text angeklickt wird, wird ""Hallo"" in die Textzeile geschrieben.
## ```copy_to_clipboard```
* Kopiert einen Text, wenn der Text angeklickt wird.
```json
"clickEvent":{"action","copy_to_clipboard","value":"<Text>"}
```
### Beipiele:
```mcfunction
/tellraw @a {"text":"Hallo, Welt!","clickEvent":{"action":"copy_to_clipboard","value":"Hallo, Welt!"}}
```
➡ Zeigt den Text "Hallo, Welt!" und wenn der Text angeklickt wird, wird der Text "Hallo, Welt!" kopiert.
```mcfunction
/tellraw @a {"text":"Blau Hex Code","color":"blue","clickEvent":{"action":"copy_to_clipboard","value":"#5555FF"}}
```
➡Zeigt den Text "Blau Hex Code" in der Farbe blau und wenn der Text angeklickt wird, wird der Text "#5555FF" kopiert
## ```open_url```
* Öffnet einen Link, wenn es angeklickt wird.
```json
"clickEvent":{"action":"open_url","value":"<Link>"}
```
