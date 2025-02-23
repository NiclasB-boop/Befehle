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
* Führt Befehl aus, wenn das Biom einer bestimmten Stelle eine bestimmte Eigenschaft hat oder ein bestimmtes Biom ist.
```json
if|unless biome <Position> <Eigenschaft>
```
* **`<Position>`** - Die Position wo gekuckt wird ob das Biom eine Eigenschaft hat.
* **`<Eigenschaft>`** - Die Eigenschaft oder das Biom nach dem gekuckt wird.
#### Beipiele
```mcfunction
/execute if biome ~ ~ ~ #minecraft:has_structure/village_plains
```
➡ Wenn das Biom, in dem die Person, die den Befehl ausführt, ist, die Struktur Dorf Flachland hat erscheint die Nachricht "Test erfolgreich". Wenn nicht, dann kommt die Nachricht "Test fehlgeschlagen".
```mcfunction
/execute unless biome ~ ~ ~ minecraft:badlands run give @s diamond
```
➡ Wenn das Biom, in dem die Person, die den Befehl ausführt, ist, nicht das Biom Ödland ist bekommt die Person einen Diamanten. Wenn doch, dann nicht.
### Block
* Führt Befehl aus, wenn ein Block an einer bestimmten Stelle eine bestimmte Eigenschaft hat oder ein bestimmter Block ist.
```json
if block <Position> <Eigenschaft>
```
* **`<Position>`** - Die Position wo gekuckt wird ob der Block eine bestimmte Eigenschaft hat oder ein bestimmter Block ist.
* **`<Eigenschaft>`** - Die Eigenschaft\ der Block nach dem gekuckt wird.
#### Beispiele
```mcfunction
/execute if block 46 30 2 minecraft:diamond_block run give @s diamond
```
➡ Wenn der Block auf der Koordinate 46 30 2 ein Diamantblock ist kriegt die Person, die den Befehl ausführt, einen Diamanten.
```mcfunction
/execute unless block ~ ~ ~ #minecraft:climbable
```
➡ Wenn der Block, auf dem die Person, die den Befehl ausführt, ist, nicht kletterbar ist, wird die Nachricht "Test erfolgreich" angezeigt. Wenn doch, dann wird die Nachricht "Test fehlgeschlagen" angezeigt. 
