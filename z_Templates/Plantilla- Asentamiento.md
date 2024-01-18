---
fileClass: Asentamiento
tags:
  - Lugar
aliases: 
icon: "![[z_Assets/Misc/PlaceholderImage.png]]"
Poblacion: 
Tematica:
  - ""
Tipo: Ciudad
Prosperidad: 
Mundo: Aretries
Terreno:
  - Urbano
Ubicacion: 
Defensas: 
Gobierno: 
Religion:
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][link]` |
> **Alias** |`=this.aliases` |
> **Tipo** | `=this.Tipo` |
> **Población** | `=this.Poblacion` |
> **Temática** | `=this.Tematica` |
> **Terreno** | `=this.Terreno`|
> ###### Política
>  |
> ---|---|
> **Lideres** | `=this.Lideres` |
> **Tipo de gobierno** | `=this.Gobierno` |
> **Defensas** | `=this.Defensas` |
> **Religiones** | `=this.Religiones` |
> **Prosperidad** | `=this.Prosperidad` |

# 🔍 A simple vista
#TBD 

# Información detallada

## 🏤 Política

_¿Qué tipo de gobierno existe? ¿Cómo y quién gobierna? ¿Quiénes se le oponen? ¿Qué facciones son las más influyentes?_

## 🛡️ Defensa

_¿Quiénes se encargan de su defensa? ¿Cómo son estas? ¿Qué peligros corre la ciudad?_

## 💰 Comercio y economía

_¿Cómo se mueve el dinero en la ciudad? ¿Cómo se entretiene la gente? ¿Qué rutas se frecuentan a la ciudad?_

## 🧾 Historia

_Descripción de la historia de la ciudad_
# ✏️ Notas


# Otros
> [!metadata|map]+ Map
> ```leaflet
> 
> 
> id: TBD
> 
> ### Lock pins so they can't be moved
> lock: true
> 
> ### If true, view of map will recenter as you zoom out. 
> recenter: true
> 
> ### If true, disables mouse scroll for zomming in and out of a map. Button controls still work. 
> noScrollZoom: false
> 
> image: [[PlaceholderImage.png]]
> 
> ### Map Pixel Height x 1 / (Pixels between Bar Scale / 100)
> ### Map Pixel Width x 1 / (Pixels between Bar Scale / 100) 
> ### Note that this formula requires adjustments depending on your map. The idea is to determine the number of units between your bar scale. We divide by 100 here because my bar scale measures in 100 units. If your maps scale bar measures in units of 50 them you should divide by 50 instead. The idea is to calculate how many pixels are equal to 1 unit. 
> 
> bounds: [[0,0], [221.92, 330.18]]
>
> ### Use this [LINK](https://docs.google.com/spreadsheets/d/1jKQxktYSUFcCJhEkAAPr1wMVBTqUdpEfA5XveUXI17I/edit?usp=sharing) to work out your map's bounds.
>
> height: 600px
> 
> width: 640px
>
> ### This sets where the map starts by default. Set it to the middle (half) of your bounds. 
> lat: 110.96
>
> long: 330.18
>
> ### 0 is no zoom. Negative zoom steps away from the map. Positive zoom steps towards the map. 
> minZoom: 1
> 
> ### Max zoom is 18. 
> 
> maxZoom: 6.5
> 
> ### Hover mouse over the Reset Zoom icon to see your current zoom level. 
> 
> defaultZoom: 1
> 
> ### How far it zooms in or out with each step. Can be in decimals. 
>
> zoomDelta: 0.5
> 
> ### This is a string so can be any text. Change it to match your maps measurement scale. 
> 
> unit: Kms
>
> scale: 1
>
> darkMode: false
>
> ```

> [!metadata|pois]+ Localizaciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Tematica
FROM #Lugar
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!metadata|groups]+ Facciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Influencia
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!metadata|characters]+ NPCs
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, join(Oficios, ", ") AS "Oficios", Alienamiento
FROM #NPC
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!metadata]- Encuentros Aleatorios
> ![[Encuentros Urbanos]]