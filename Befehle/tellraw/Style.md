# ✨ Style-Optionen

```json
"bold", "italic", "obfuscated", "strikethrough", "underlined"
```

## 🔧 Wie funktionieren sie?
✅ Zuerst wird die Option in **Anführungszeichen** angegeben.  
✅ Dann folgt ein **Doppelpunkt**.  
✅ Zum Schluss kommt entweder `true` oder `false`, um die Option zu **aktivieren** oder **deaktivieren**.  
✅ Standardmäßig ist alles **deaktiviert**.  
✅ Mehrere Optionen werden mit **Kommas** getrennt.  

**Beispiel:**
```json
{"bold":true}
```
➡ Aktiviert die **fettgedruckte** Darstellung.

---

## 🎨 Welche Optionen gibt es?
| Option         | Bedeutung      |
|---------------|---------------|
| bold       | 🖋 Fett        |
| italic       | ✍ Kursiv       |
| obfuscated | 🔀 Unlesbar    |
| striketrough | ❌ Durchgestrichen |
| underlined | 📏 Unterstrichen |

## 🛠 Beispiele
```mcfunction
/tellraw @s {"text":"Gelb", "bold":true}
```
➡ Zeigt den Text **„Fett“** **fettgedruckt**.

```mcfunction
/tellraw @s {"text":"Rot", "italic":true, "striketrough":true}
```
➡ Zeigt den Text **„Kurisiv und Durchgestrichen“** **kursiv** und **durchgestrichen**.

```mcfunction
/tellraw @s {"text":"Nichts", "underlined":false}
```
➡ Zeigt den Text **„Nichts“** **ohne** extra Style-Optionen.
