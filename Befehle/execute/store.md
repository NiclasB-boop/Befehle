# ```store``` - Optionen
## ```store```
* Kann den Wert den ein Befehl ausführt speichern.
```json
store result\sucess <Speicherort> <Speicherformat>
```
* **`<Speicherort>`** - Der Ort wo gespeichert (z.B. bossbar, nbt-data).
* **`<Speicherformat>`** - Das Format in dem gespeichert wird (z.B. byte, double)
## ```result\sucess```
* result: speichert den Wert den der Befehl gibt.
* sucess: speichert ob der Befehl funktioniert hat.
## Speicherorte
### ```block```
* Speichert in einem bestimmten Block.
```json
store result\sucess block <Position> <Weg> <Speicherformat>
```
* **`<Position>`** - Position des Blockes.
* **`<Weg>`** - Der Nbt-Weg in dem der Wert gespeichert werden soll.
* **`<Speicherformat>`** - Das Format in dem gespeichert wird. 
