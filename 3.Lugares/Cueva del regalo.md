---
fileClass: Asentamiento
tags:
  - Lugar
  - Relevante
aliases: 
icon: "![[cueva del regalo.png]]"
Poblacion: Kobolds y un dragon blanco joven
Gobernantes: 
Tematica:
  - Congelacion
  - Historia
Tipo: Mazmorra
Prosperidad: Bajo
Terreno:
  - Mazmorra
Mundo:
  - Aretries
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Población** | `=this.Poblacion` |
> **Temática** | `VIEW[{Rangos}][text(renderMarkdown)]` |
> **Terreno** | `VIEW[{Terreno}][text(renderMarkdown)]`|
> ###### Política
>  |
> ---|---|
> **Lideres** | `VIEW[{Lideres}][text(renderMarkdown)]` |
> **Tipo de gobierno** | `VIEW[{Gobierno}][text(renderMarkdown)]` |
> **Defensas** | `VIEW[{Defensas}][text(renderMarkdown)]` |
> **Religiones** | `VIEW[{Religiones}][text(renderMarkdown)]` |
> **Prosperidad** | `VIEW[{Prosperidad}][text(renderMarkdown)]` |
>   ## NPCs
>   ```dataview
table without ID  file.link AS Nombre, Raza
FROM #NPC
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC
>```
>   ## Facciones
> ```dataview
table without ID  file.link AS Nombre
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.Tipo ASC

# 🔍 A simple vista

La cueva del regalo es una cueva abandonada por [[Gath Igeo]] y actualmente ocupada por Kobolds y un dragón helado. Han estado atacando las aldeas cerca. Los kobolds acaban de conseguir destilar cebada y estan montando una fiesta de aupa mientras  

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Ubicaciones
### Estatua de la bienvenida
Estatua de una mujer entregando algo con la mano que no existe.
A sus pies enterrada en la nieve una inscripción reza: "Si tu corazón es puro y digno entra en la cueva y recibe el legado de plata. Se el escudo del mundo y gana tu entrada en [[La escama plateada]]"
### Pila de Huesos congelada
Es una enorme pila de huesos. Estos son restos de los dragones plateados que habitaban la cueva, incluidos también los hermanos de [[Lisa]].
### Trampas
#### Suelo resbaladizo
#### Cable
### Destileria
Los kobolds han logrado fermentar un enorma carro de cebada que robaron.
### Pista de gogos
Unos kobolds bailan alegremente tras obtener su ultimo botín
### Meadero
Aquí cagan y mean los kobolds para después esconderlo entre la nieve
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
> image: [[La cueva del sabio.png]]
> 
> ### Map Pixel Height x 1 / (Pixels between Bar Scale / 100)
> ### Map Pixel Width x 1 / (Pixels between Bar Scale / 100) 
> ### Note that this formula requires adjustments depending on your map. The idea is to determine the number of units between your bar scale. We divide by 100 here because my bar scale measures in 100 units. If your maps scale bar measures in units of 50 them you should divide by 50 instead. The idea is to calculate how many pixels are equal to 1 unit. 
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

> [!metadata]- Encuentros Aleatorios
> ![[Encuentros Montaña]]