# ```align\positioned\at\in```
## ```align\positioned\at\in``` - Optionen
* Führen Befehle an anderen Orten aus.
## ```align```
*  Rundet die Achsen wo der Befehl ausgeführt wird.
```json
align <Achsen>
```
* **`<Achsen>`** - Die Achsen die gerundet werden.
### Beispiele

## ```at```
* Führt Befehl an Position einer Entität aus.
* Entsprechen mehrere Entitäten dem Selektor wird der Befehl mehrmals ausgeführt.
* Rotation wird auch übernommen.
```json
at <Ziel>
```
* **`<Ziel>`** - Die Entität an der der Befehl ausgeführt wird.
### Beispiele

## ```in```
* Führt Befehl in bestimmter Dimension aus.
```json
in <overworld|the_nether|the_end>
```
* **`<overworld|the_nether|the_end>`** - Die Dimension in der der Befehl ausgeführt wird.
### Beipiele

## ```positioned```
* Führt Befehl an bestimmter Stelle aus.
* Entsprechen mehrere Entitäten dem Selektor wird der Befehl mehrmals ausgeführt.
```json
positioned as <Ziel>
positioned <Position>
positioned over <Höhenkarte>
```
* **`Ziel`** - Die Peson an dessen Stelle der Befehl ausgeführt wird.
* **`Position`** - Die Position an der der Befehl ausgeführt wird.
* **`Höhenkarte`** - Stelle der Höhenkarte in der Y-Achse auf der der Befehl ausgeführt wird.
### Höhenkarten
* motion_blocking: Blöcke die nicht durchlaufbar sind.
* motion_blocking_no_leaves: Blöcke die nicht durchlaufbar sind außer Blättern.
* ocean_floor: Blöcke außer Luft und Wasser.
* world_surface: Blöcke außer Luft.
### Beipiele
