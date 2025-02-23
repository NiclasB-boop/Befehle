# **`tellraw`-Befehl**

## ✨ Was macht er?
* Sendet eine Nachricht an bestimmte Spieler
* Der Text ist formatierbar (Farbe, Kursiv, etc.)
* Der Text kann anklickbar sein:
  * ✅ Befehle ausführen
  * 🌍 Links öffnen
  * 📋 Text kopieren

---

## 🛠 Syntax
```mcfunction
/tellraw <Spieler> {Optionen}
```
* **`<Spieler>`** – Die Zielperson(en), die die Nachricht erhalten.
* **`{Optionen}`** – JSON-Formatierte Optionen für das Styling und Verhalten des Textes:
  * ```json
    {"text":"<Text>"}
    ```
    ➡ Gibt den Text der Naricht an.
  * ```json
    {"color":"<Farbe>"}
    ```
    ➡ Bestimmt die Farbe des Textes (z. B. `"red"` oder `"#00ff00"`).
  * Weitere Attribute wie **`bold`**, **`italic`**, **`underlined`** sind ebenfalls möglich.

---

## 🔥 Beispiele
```mcfunction
/tellraw @s {"text":"Hallo!", "color":"red"}
```
➡ Zeigt dem ausführenden Spieler den Text **„Hallo!“** in **roter** Farbe.

```mcfunction
/tellraw @a {"text":"Test?!", "color":"#00ff00", "bold":true}
```
➡ Zeigt **allen Spielern** den Text **„Test?!“** in **grüner, fetter** Schrift.

---

📌 *Mehr Infos: [Minecraft-Wiki](https://minecraft.wiki/w/Tellraw)*
