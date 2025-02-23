# ```as\on```
## ```as\on```-Optionen
* Führt Befehle als jemand anderes aus.
```json
on\as <Ziel>
```
* **`Ziel`** - Die Person die den Befehl ausführt
## ```as```
* Führt Befehl als bestimmter Selektor (@e,@a,NiclasB) aus.
### Beispiele

## ```on```
* Führt Befehl als jemand der zu jemandem in Verbindung steht aus.
```json
on <Verbindung>
```
* **`Verbindung`** - Die Art wie sie in Verbindung stehen.
### Verbindungen
* attacker: Von wem die Entität in den letzten fünf Sekunden angegriffen wurde.
* controller: Die Entität die die Entität steuert (z.B ein Boot wird von einem Spieler gesteuert)
* leasher: Die Entität die, die Entität an einer Leine hält.
* origin: Die Entität die zum Entstehen der Entität geführt hat (z.B ein Skelett schießt einen Pfeil).
* owner: Besitzer der Entität (z.B. der Besitzer eines Hundes).
* passengers: Die Entitäten die auf der Entität reiten bzw. sitzen.
* target: Das Ziel einer Entität (z.B. ein Zombie möchte einen Dorfbewohner angreifen).
* vehicle: Entität auf der geritten bzw. gesessen wird.
### Beispiele
