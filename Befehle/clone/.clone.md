# 🏰 **`clone`-Befehl** 🏰  
## 🔍 **Was macht er?**  
✨ Er kopiert ein bestimmtes Gebäude an eine bestimmte Stelle.  

## 📝 **Syntax**  
```mcfunction
/clone <Von> <Bis> <Ziel> filtered|masked|replace force|move|normal
```
🔹 **`<Von>`** – Die Startkoordinate des Kopierbereichs.  
🔹 **`<Bis>`** – Die Endkoordinate des Kopierbereichs.  
🔹 **`<Ziel>`** – Die Zielkoordinaten, an die das Gebäude kopiert wird.  

## 🏰 **Modi (`filtered | masked | replace`)**  
🔸 **`filtered`** – Kopiert nur bestimmte Blöcke.  
🔹 **`masked`** – Kopiert alle Blöcke außer Luft.  
🔹 **`replace`** – Kopiert alle Blöcke.  

## 🚀 **Beispiele**  
📌 **Kopiert alle Blöcke, auf denen Tiere spawnen können**  
```mcfunction
/clone ~1 ~-1 ~1 ~-1 ~-1 ~-1 ~-1 ~4 ~ filtered #minecraft:animals_spawnable_on
```
➡ **Kopiert Blöcke aus einem 3×3 Bereich unter dem Spieler und platziert sie vier Blöcke über ihm.**  

📌 **Kopiert alle Blöcke außer Luft**  
```mcfunction
/clone ~1 ~-1 ~1 ~-1 ~-1 ~-1 ~-1 ~4 ~ masked
```
➡ **Alle nicht-leeren Blöcke werden kopiert und vier Blöcke über dem Spieler platziert.**  

📌 **Kopiert alle Blöcke**  
```mcfunction
/clone ~1 ~-1 ~1 ~-1 ~-1 ~-1 ~-1 ~4 ~ replace
```
➡ **Alle Blöcke werden aus einem 3×3 Bereich unter dem Spieler exakt kopiert.**  
