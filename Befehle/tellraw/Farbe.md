# 🎨 Option-Farbe

```json
"color"
```

## 📌 Farboptionen
Die Farben können als **Hex-Code** oder als **Wort** angegeben werden:
```json
"color":"<Farbe>"
```
💡 **\<Farbe>** wird durch den gewünschten Farbnamen oder Hex-Code ersetzt.

---

### 🌈 Verfügbare Farben:
> 🖤 **black** `#000000`  
> 🔵 **dark_blue** `#0000AA`  
> 🟢 **dark_green** `#00AA00`  
> 🔷 **dark_aqua** `#00AAAA`  
> ❤️ **dark_red** `#AA0000`  
> 💜 **dark_purple** `#AA00AA`  
> 🟠 **gold** `#FFAA00`  
> ⚪ **gray** `#AAAAAA`  
> ⚫ **dark_gray** `#555555`  
> 🔵 **blue** `#5555FF`  
> 🟢 **green** `#55FF55`  
> 🔷 **aqua** `#55FFFF`  
> ❤️ **red** `#FF5555`  
> 💗 **light_purple** `#FF55FF`  
> 💛 **yellow** `#FFFF55`  
> ⚪ **white** `#FFFFFF`

---

## 🛠 Beispiele
```mcfunction
/tellraw @s {"text":"Gelb", "color":"yellow"}
```
➡ Zeigt den Text **„Gelb“** in **Gelb**.

```mcfunction
/tellraw @s {"text":"Rot", "color":"#FF5555"}
```
➡ Zeigt den Text **„Rot“** in **Rot**.

```mcfunction
/tellraw @s {"text":"Blau", "color":"#5555FF"}
```
➡ Zeigt den Text **„Blau“** in **Blau**.
