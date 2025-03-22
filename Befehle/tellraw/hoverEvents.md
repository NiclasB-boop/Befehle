# hoverEvents
## Was sind hoverEvents
* Wenn man über den Text gleitet, wird ein bestimmter Text gezeigt.
## Verfügbare hoverEvents
```json
"show_text", "show_item", "show_entity"
```
## Algemeine Syntax:
```json
"hoverEvent":{"action":"<hoverEvent>","value":"<Text/Link/Befehl>"}
```
## hoverEvents
### ```show_text```
* Zeigt einen Text, wenn du über den Text gleitest
```json
"hoverEvent":{"action":"show_text","contents":<Text>}
```
#### Beispiele:
```mcfunction
/tellraw @s {"text":"Hallo, Welt!","hoverEvent":{"action":"show_text","contents":{"text":"Hallo, Welt!"}}}
```
➡ Zeigt dem Spieler, der den Befehl ausführt, den Text Hallo, Welt! und wenn er über den Text gleitet wird der Text Hallo, Welt! gezeigt.
```mcfunction
/tellraw @s {"nbt":"Health","entity":"@s","hoverEvent":{"action":"show_text","contents":{"nbt":"Health","entity":"@s"}}}
```
➡ Zeigt dem Spieler, der den Befehl ausführt, Lebensanzahl die er zu dem Zeitpunkt als er den Befehl ausgeführt hat hatte und wenn er über den Text gleitet wird die Lebensanzahl die er zu dem Zeitpunkt als er den Befehl ausgeführt hat hatte gezeigt.
### ```show_item
* Zeigt wie ein Item im Inventar aussehen würde, wenn man darüber gleitet.
```json
"hoverEvent":{"action":"show_item","contents":{"id":"<Item>"}}
```
#### Beispiele
```mcfunction
/tellraw @s {"translate":"item.minecraft.diamant","hoverEvent":{"action":"show_item","contents":{"id":"diamond"}}}
```
➡ Zeigt den Text Diamant und wenn über ihn gegleitet wird, werden die Tooltips eines Diamanten angezeigt.
```mcfunction
/tellraw @s {"translate":"item.minecraft.diamant","color":"aqua","hoverEvent":{"action":"show_item","contents":{"id":"diamond","tag":"{display:{Name:'{\"translate\":\item.minecraft.diamond\",\"color\":\"aqua\"}'}}"}}}
```
➡ Zeigt den Text Diamant in Aqua und wenn über ihn gegleitet wird, werden die Tooltips eines Diamanten der Diamant in Aqua genannt wurde angezeigt.
