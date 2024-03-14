---
fileClass: Lugar
tags:
  - Lugar
aliases: 
icon: "![[PlaceholderImage.png]]"
Tematica: 
Prosperidad: 
Mundo: Aretries
Terreno: 
Poblacion: 
Tipo: Region
Ubicacion:
---


> [!infobox| background-black ]+
> `VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** | `= aliases  `|
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Población** | `=this.Poblacion` |
> **Temática** | `VIEW[{Rangos}][text(renderMarkdown)]` |
> **Terreno** | `VIEW[{Terreno}][text(renderMarkdown)]`|
>   ## NPCs
>   ```dataview
table without ID  file.link AS Nombre, Raza
FROM #NPC
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC
>```
> ## Localizaciones
>   ```dataview
table rows.file.link AS Nombre
FROM #Lugar
WHERE  contains(Ubicacion, [[]])
GROUP BY Tipo
SORT file.name ASC
>```
>   ## Facciones
> ```dataview
table without ID  file.link AS Nombre
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.Tipo ASC
# 🔍 A simple vista

#TBD

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Mapa
 ```leaflet
 
 
 id: Lugar
 
 ### Lock pins so they can't be moved
 lock: true
 
 ### If true, view of map will recenter as you zoom out. 
 recenter: true
 
 ### If true, disables mouse scroll for zomming in and out of a map. Button controls still work. 
 noScrollZoom: false
 
 image: [[PlaceholderImage.png]]
 
 ### Map Pixel Height x 1 / (Pixels between Bar Scale / 100)
 ### Map Pixel Width x 1 / (Pixels between Bar Scale / 100) 
 ### Note that this formula requires adjustments depending on your map. The idea is to determine the number of units between your bar scale. We divide by 100 here because my bar scale measures in 100 units. If your maps scale bar measures in units of 50 them you should divide by 50 instead. The idea is to calculate how many pixels are equal to 1 unit. 
 
 bounds: [[0,0], [221.92, 330.18]]

 ### Use this [LINK](https://docs.google.com/spreadsheets/d/1jKQxktYSUFcCJhEkAAPr1wMVBTqUdpEfA5XveUXI17I/edit?usp=sharing) to work out your map's bounds.

 height: 600px
 
 width: 640px

 ### This sets where the map starts by default. Set it to the middle (half) of your bounds. 
 lat: 110.96

 long: 330.18

 ### 0 is no zoom. Negative zoom steps away from the map. Positive zoom steps towards the map. 
 minZoom: 1
 
 ### Max zoom is 18. 
 
 maxZoom: 6.5
 
 ### Hover mouse over the Reset Zoom icon to see your current zoom level. 
 
 defaultZoom: 1
 
 ### How far it zooms in or out with each step. Can be in decimals. 

 zoomDelta: 0.5
 
 ### This is a string so can be any text. Change it to match your maps measurement scale. 
 
 unit: Kms

 scale: 1

 darkMode: false

 ```
