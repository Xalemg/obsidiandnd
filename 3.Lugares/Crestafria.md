---
fileClass: Asentamiento
tags:
  - Lugar
  - Relevante
aliases: 
icon: "![[CrestaFria.png]]"
Poblacion: ""
Tematica:
  - Agricultura
Tipo: Ciudad
Prosperidad: Alta
Mundo: Aretries
Terreno:
  - Isla
Gobierno: Monarquia
Ubicacion: "[[3.Lugares/Isla de Altalos.md|Isla de Altalos]]"
Defensas:
  - La guardia real
Religion:
  - "[[Tyr]]"
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `=this.Ubicacion` |
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
> **Religiones** | `=this.Religion` |
> **Prosperidad** | `=this.Prosperidad` |

# 🔍 A simple vista

Crestafria, la ciudad inconquistable, la llave del reino y la ciudad de los fuertes. Crestafria es un símbolo de la monarquía de Altalos. Se considera que aquel que controla la ciudad controla el reino y suele ser coronado como tal. Es imposible comprender el Reino de Altalos su historia, su cultura y su política sin comprender Crestafria.
A simple vista Crestafria destaca su enfoque militar. Las casas tienen murallas por paredes y saeteras por ventas. Los distintos castillos que aqui se encuentran tienen grandes torres que luchan por sobrepasar a las de alrededor, para asi obtener la ventaja aerea. Todos los edificios marcan varias 

Con más de 2 millones de habitantes se trata de la ciudad más habitada del reino y la segunda de todas las [[Islas Shamal]]  . Está dividida en tres niveles que están habitados por sus correspondientes estratos sociales, la falda (por el pueblo), la ladera (por la nobleza) y la cima (por la corona y su corte).

Se sitúa en el punto estratégico más importante de la isla, su centro físico y un cruce entre las 3 principales zonas del reino, controlando de esta forma las dos únicas vías de comunicación terrestres seguras del reino. A demás su escarpado acantilado hace casi imposible ningún asalto desde el valle. Es por esto que las principales familias nobles y gobernantes del reino construyen sus mayores fortalezas aquí. Durante las múltiples guerras civiles que han asolado esta nación, sus calles tienden a convertirse en un campo de batalla más. En la que la nobleza, tele transportando a sus tropas a sus fortalezas, luchan calle a calle por hacerse con la cima. Los ciudadanos suelen acabar uniéndose a alguno de los bandos, por defender su propiedad, adueñarse de la del vecino o acabar con la tiranía de su señor. Eso es lo que da a la ciudad su aspecto tan militar, no es de extrañar encontrarse panaderías con fosos, molinos con barricadas o casas con saeteras y torres.

Durante estas ocasiones las partes altas solo son capaz de sustentarse gracias a los múltiples templos y a la importantísima y renombrada torre de magia de Crestafria, ya que al hallarse a más de 2 kilómetros de altura la agricultura es prácticamente inexistente.


# Información detallada

## 🏤 Política
La [[Corona de Altalos]] dirige la ciudad, al igual que el resto de las tierras del Rey. Por otro lado cada una de las casas del reino tiene una fortaleza y representación en la ciudad.

## 🛡️ Defensa

En Cresafria no existe una guardia propia, en su lugar cada una de las Familias Nobles de la ciudad tiene su propia protección. Según la dedicación de cada familia, estas tienden a enviar patrullas a la falda o a patrullar las calles. 
Clerigos de [[Tyr]] tienden a patrullar tambien las calles y cualquier acto delictivo es juzgado frente a la presencia 

## 💰 Comercio y economía

Crestafria al contrario de la mayoria de las ciudades no es un gran motor económico. Las principales

## 🧾 Historia

_Descripción de la historia de la ciudad_

# Otros
> [!metadata|map]+ Map
> ```leaflet
> 
> 
> id: Crestafria
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
> image: [[Crestafria.jpeg]]
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
### Sitios de Interes
#### Tabernas Kalberin
mas decoradas con pinturas caballerescas
#### Posada del caballero descansado
#### Taberna los coros de la redención
Un paladin con lazos con la iglesia de [[Tyr]] regenta la taberna los clérigos cantan en tramontes todos los días dando 2d6+2 puntos de golpe temporales a los parroquia que escuchan
#### El emporium imperium
Tienda de armas mas variada del reino, encantadas y imbuidas en distintos efectos magicos.
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
WHERE  contains(Ubicacion, [[]]) AND !contains(Estado, "Muerto" ) AND !contains(Estado, "Muerto" )
SORT file.name ASC

> [!metadata]- Encuentros Aleatorios
> ![[Encuentros Urbanos]]