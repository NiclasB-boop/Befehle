# Itemnamen nbt-Data
## Was macht er?
* Er macht, dass das Item das dem Spieler gegeben wird einen bestimmten Namen hat.
```json
display:{Name:'<Name>',Lore:[<Lehre>]}
```
* ***```<Name>```*** - Name des Items.
* ***```<Lehre>```*** - Die Lehre des Items als Liste.
* Formatierung siehe [tellraw](../tellraw/_tellraw)
## Besipiele
```mcunction
/give @s diamond{display:{Name:'"Hallöle"'}}
```
➡ Gibt dem Spieler, der den Befehl ausführt, einen Diamanten der Hallöle heißt
```mcfuntion
/give @a diamond{display:{Lore:['[{"text":"Hallo"},{"text":"Nochmal Hallo"}]','{"text":"zu viele Hallos"}']}}
```
➡ Gibt jedem Spieler einen Diamanten mit der Lehre HalloNochmal Hallozu viele Hallos.
