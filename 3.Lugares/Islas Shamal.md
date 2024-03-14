---
fileClass: Asentamiento
tags:
  - Lugar
  - favoritos
aliases: 
icon: "![[Costa de Altalos.png]]"
Poblacion: Alrededor de 12 millones, principalmnete Gnomos, Enanos y humanos, aunque casi todas las razas pueden ser vistas en las ciudade
Tematica:
  - Diversidad
  - Comercio
  - Exploración
Tipo: Continente
Prosperidad: Alta
Mundo:
  - Aretries
Terreno:
  - Archipielago
Gobierno: 
Ubicacion: "[[Aretries]]"
Defensas: 
Religion: 
cssclasses:
  - wide
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
> **Prosperidad** | `VIEW[{Prosperidad}][text(renderMarkdown)]` |
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
Las [[Islas Shamal]]  se encuentran entre los Imperios élficos del Amanecer (al este de las Islas) y del Atardecer (al oeste de las Islas). La principal entidad política es la Mancomunidad del viento, una Alianza entre países a los que la mayor parte de los humanoides que las habitan pertenecen.

Aunque la raza dominante es la Gnomo existen numerosos territorios pertenecientes a otras razas. Hay una gran cultura marítima y comercial en las Islas y se dice que las rutas marinas son más seguras que los caminos. En la Mancomunidad todo lanzador de magia Arcana debe estar abalado por una de las torres de hechicería, y aquellos que la practican sin su permiso, son perseguidos. Magos y artificieros tienen un gran prestigio, mientras que la magia divina esta vista como un poder menor y orientado a la curación. En la Mancomunidad a ciertos dioses se les ha prohibido el culto.

## Cultura de las Islas

Existe una gran cultura comerciante y maritima en las Islas propulsada por Adur y su población gnoma. Aun asi en las [[Islas Shamal]]  existen una gran cantidad Naciones independientes.

## Folclore

Existen dos historias que todo habitante de la mancomunidad conoce:

**Los últimos días de los dioses**: Hace mas de mil años los dioses caminaban la tierra y su influencia sobre la vida de la gente estaba muy presente. Algunos dioses se aliaron para crear grietas que conectaban el plano material con otros, y a través de ellas criaturas extra planares atacaron las islas. Los habitantes de las Islas formaron otra alianza con ciertos dioses para cerrar la grietas. Esto produjo una gran guerra que acabó con la muerte de los principales dioses.

**Las guerras del Mar**: Hace varios siglos los Imperios del Amanecer y del Atardecer formaban un único Imperio conocido como el Imperio del Sol. Un intento de invasión de este Imperio provocó que los humanoides se unieran en la Mancomunidad del Viento. La victoria de la Mancomunidad les garantizó la exclusividad para el comercio entre los dos continentes del Imperio del Sol.
# 📜 Historia

#TBD

# ✏️ Notas

# Mapa
>[]
> ```leaflet
> 
> 
> id: Islas
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
> image: [[Islas Shamal Upscale 50.jpg]]
> 
> ### Map Pixel Height x 1 / (Pixels between Bar Scale / 100)
> ### Map Pixel Width x 1 / (Pixels between Bar Scale / 100) 
> ### Note that this formula requires adjustments depending on your map. The idea is to determine the number of units between your bar scale. We divide by 100 here because my bar scale measures in 100 units. If your maps scale bar measures in units of 50 them you should divide by 50 instead. The idea is to calculate how many pixels are equal to 1 unit. 
> 
> bounds: [[0,0], [429.15, 606.92]]
>
> ### Use this [LINK](https://docs.google.com/spreadsheets/d/1jKQxktYSUFcCJhEkAAPr1wMVBTqUdpEfA5XveUXI17I/edit?usp=sharing) to work out your map's bounds.
>
> height: 700px
> 
> width: 640px
>
> ### This sets where the map starts by default. Set it to the middle (half) of your bounds. 
> lat: 214
>
> long: 303
>
> ### 0 is no zoom. Negative zoom steps away from the map. Positive zoom steps towards the map. 
> minZoom: 0
> 
> ### Max zoom is 18. 
> 
> maxZoom: 3
> 
> ### Hover mouse over the Reset Zoom icon to see your current zoom level. 
> 
> defaultZoom: 0
> 
> ### How far it zooms in or out with each step. Can be in decimals. 
>
> zoomDelta: 0.5
> 
> ### This is a string so can be any text. Change it to match your maps measurement scale. 
> 
> unit: Kms
>
> scale: 2
>
> darkMode: false
>
> ```
