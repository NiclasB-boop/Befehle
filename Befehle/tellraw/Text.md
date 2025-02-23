# Text-Optionen für `tellraw`

## Verfügbare Text-Optionen
```json
"text", "selector", "nbt", "score", "keybind", "translate"
```

### Allgemeine Syntax
- Die Option wird in **Anführungszeichen** geschrieben.
- Danach folgt ein **Doppelpunkt** (`:`).
- Der Wert der Option wird ebenfalls in **Anführungszeichen** gesetzt.

---

## 📜 `"text"`
Zeigt einfachen Text an.

```json
{"text":"<Text>"}
```

### Beispiele
```mcfunction
/tellraw @s {"text":"Hallo, Welt!"}
```
➡ Zeigt den Text **"Hallo, Welt!"** an.

```mcfunction
/tellraw @s {"text":"Text"}
```
➡ Zeigt den Text **"Text"** an.

---

## 🎯 `"selector"`
Zeigt den Namen eines Selektors (z. B. Spielername oder Entity-Name).

```json
{"selector":"<Selektor>"}
```

### Beispiele
```mcfunction
/tellraw @s {"selector":"@s"}
```
➡ Zeigt dem Spieler, der den Befehl ausführt, seinen eigenen Namen.

```mcfunction
/tellraw @a {"selector":"@e"}
```
➡ Zeigt jedem Spieler die Namen aller Entitäten an.

---

## 📦 `"nbt"`
Zeigt bestimmte NBT-Daten eines Entitäts- oder Block-Attributs an.

```json
{"nbt":"<NBT-Daten>","entity":"<Ziel>"}
```

### Beispiele
```mcfunction
/tellraw @a {"nbt":"Health","entity":"@s"}
```
➡ Zeigt jedem Spieler die **Lebenspunkte** des ausführenden Spielers an.

```mcfunction
/tellraw @a {"nbt":"Air","entity":"@e"}
```
➡ Zeigt jedem Spieler, wie lange jede Entität noch atmen kann.

---

## 🎮 `"score"`
Zeigt den Wert eines **Scoreboards** an.

```json
{"score":{"name":"<Ziel>","objective":"<Scoreboard>"}}
```

### Beispiele
```mcfunction
/tellraw @a {"score":{"name":"@s","objective":"Punkte"}}
```
➡ Zeigt jedem Spieler den **Punktewert** seines Scoreboards an.

---

## ⌨ `"keybind"`
Zeigt die **Tastenbelegung** für eine bestimmte Aktion, basierend auf den aktuellen Einstellungen des Spielers.

```json
{"keybind":"<Aktion>"}
```

### Beispiele
```mcfunction
/tellraw @a {"keybind":"key.forward"}
```
➡ Zeigt jedem Spieler die **Tastenbelegung** für **Vorwärts laufen** an.

Falls keine Taste belegt ist, wird „Nicht belegt“ angezeigt.

---

## 🌍 `"translate"`
Übersetzt Begriffe ins **Spielersprache**, sofern sie in Minecraft vordefiniert sind.

```json
{"translate":"<Übersetzbarer Begriff>"}
```

### Beispiele
```mcfunction
/tellraw @a {"translate":"block.minecraft.dirt"}
```
➡ Zeigt jedem Spieler das übersetzte Wort für **„Erde“** an.

```mcfunction
/tellraw @a {"translate":"block.minecraft.black_concrete"}
```
➡ Zeigt jedem Spieler das übersetzte Wort für **„Schwarzer Beton“** an.
