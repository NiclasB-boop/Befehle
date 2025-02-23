# ```at\rotated\facing\anchored```
## ```at\rotated\facing\anchored``` - Optionen
* Führt Befehle anders rotiert aus.
## ```at```
* Führt Befehl wie jemand anderes rotiert aus.
* Übernimmt auch Position.
```json
at <Ziel>
```
* **`<Ziel>`** - Die Entität, dessen Rotation übernommen wird.
### Beipiele

## ```rotated```
* Führt Befehl wie jemand anderes rotiert aus.
* Führt Befehl bestimmt rotiert aus.
```json
rotated as <Ziel>
rotated <Rotation>
```
* **`<Ziel>`** - Die Person dessen Rotation übernommen wird.
* **`<Rotation>`** - Die Rotation mit der der Befehl ausgeführt wird.
### Beipiele

## ```facing```
* Führt Befehl auf eine bestimmte Position rotiert aus.
```json
facing entity <Ziel> <eyes|feet>
facing <Position>
```
* **`Ziel`** - Die Entität auf die der Befehl rotiert wird.
* **`<eyes|feet>`** - Auf welche Stelle der Entität rotiert wird.
* **`Postition`** - Die Position auf die der Befehl rotiert ist.
### Beispiel

## ```anchored```
* Bestimmt von wo aus rotiert ist.
```json
anchored <eyes|feet>
```
* **`<eyes|feet>`** - Die Position von der der Befehl rotiert ist.
### Beispiele
