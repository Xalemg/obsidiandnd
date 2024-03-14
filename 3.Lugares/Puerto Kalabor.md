---
fileClass: Lugar
tags:
  - Lugar
aliases:
  - La Joya del Mar
icon: "![[Adur.png]]"
Tematica:
  - Politica
  - Ecologismo
  - Desigualdad Social
  - Progreso
Prosperidad: Muy Alto
Mundo:
  - Aretries
Terreno:
  - Urbano
Poblacion: 
Tipo: Region
Ubicacion: "[[Isla de Adur]]"
cssclasses: []
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

# 🔍 A simple vista

#TBD

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Otros
## Mapa
 ```leaflet
 
 
 id: Kalabor
 
 ### Lock pins so they can't be moved
 lock: true
 
 ### If true, view of map will recenter as you zoom out. 
 recenter: true
 
 ### If true, disables mouse scroll for zomming in and out of a map. Button controls still work. 
 noScrollZoom: false
 
 image: [[z_Assets/Mapas/Kalabor.jpg]]

 ### 0 is no zoom. Negative zoom steps away from the map. Positive zoom steps towards the map. 
 minZoom: 1
 
 ### Max zoom is 18. 
 
 maxZoom: 6.5
 
 ### Hover mouse over the Reset Zoom icon to see your current zoom level. 
 
 defaultZoom: 2.5
 
 ### How far it zooms in or out with each step. Can be in decimals. 

 zoomDelta: 0.5
 
 ### This is a string so can be any text. Change it to match your maps measurement scale. 
 
 unit: Kms

 scale: 1

 darkMode: false

 ```

> [!metadata|pois]+ Localizaciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Tematica
FROM #Lugar
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!facciones|facciones]+ Facciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Influencia
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!characters|characters]+ NPCs
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, join(Oficios, ", ") AS "Oficios", Alienamiento
FROM #NPC
WHERE  contains(Ubicacion, [[]]) AND !contains(Estado, "Muerto" )
SORT file.name ASC