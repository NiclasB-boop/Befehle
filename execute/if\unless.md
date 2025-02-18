# ```if\unless```
## if\unless - Optionen
* Führt Befehle aus oder nicht aus, wenn eine bestimmte Bedingung gilt.
* Wenn kein Befehl ausgeführt wird, wird gesagt:"Test erfolgreich" oder "Test fehlgeschalgen"
```json
if|unless <Bedingung>
```
* **`<Bedingung>`** - Die Bedingung die gelten muss damit der Befehl ausgeführt (nicht ausgeführt) wird.
## Bedingungen
### Biome
* Führt Befehl aus, wenn das Biom einer bestimmten Stelle eine bestimmte Eigenschaft hat.
```json
if|unless biome <Position> <Eigenschaft>
```
