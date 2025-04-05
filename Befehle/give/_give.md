# **`give`-Befehl**
## Was macht er?
* Gibt einem bestimmten Spieler einen bestimmten Gegenstand
```json
/give <Ziel> <Gegenstand>{<nbt-Data>} <Anzahl>
```
* ***```<Ziel>```*** - Wer den Gegenstand bekommt.
* ***```<Gegenstand>```*** - Der Gegenstand den die Person bekommt.
* ***```<nbt-Data>```*** - Die nbt-Data des Gegenstands.
* ***```<Anzahl>```*** - Wieviele er bekommt.
## Beispiel
```mcfunction
/give @s diamond 1
```
➡ Gibt dem Spieler, der den Befehl ausführt, einen Diamanten.
```mcfunction
/give @a minecraft:light_blue_dye{display:e{Name:'{"translate":"item.minecraft.diamond","color":"#55ffff"}'}} 64
```
➡ Gibt jedem Spieler 64 hellblaue Farbstoffe die Diamant in Aqua heißen.