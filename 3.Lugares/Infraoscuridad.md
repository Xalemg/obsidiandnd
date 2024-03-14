---
fileClass: Lugar
tags:
  - Lugar
aliases: 
icon: "![[infraoscuridad.jpeg]]"
Tematica: [Alienigena, Supervivencia]
Prosperidad: Muy Bajo
Mundo: Aretries
Terreno: Cavernas, cuevas, mares subterraneos
Poblacion: 
Tipo: Region
Ubicacion: "[[Aretries]]"
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

La Infraoscuridad no es una caverna gigante bajo [[Aretries]]  , sino más bien muchas redes enormes de cavernas y cuevas. Por ello, no siempre era posible viajar de un extremo a otro de la Infraoscuridad. La Infraoscuridad estaba dividida en varios dominios que eran similares a los continentes del mundo superior. Aunque era posible viajar de un lugar a otro dentro de un dominio, los dominios separados solían tener muy pocos pasajes que los unieran.

La oscuridad superior Altaoscuridad Las primeras 3 millas (4,8 kilómetros) por debajo de la superficie. Es aquí donde los habitantes de la superficie y los de la Infraoscuridad se encuentran con más frecuencia. Mediaoscuridad situada entre 4,8 y 16 kilómetros por debajo de la superficie, esta capa era donde se encontraban la mayoría de las ciudades de la Infraoscuridad. Bajaoscuridad A 16 kilómetros (10 millas) o más por debajo de la superficie, la BajaOscuridad era el lugar donde incluso los que conocían la Infraoscuridad se resistían a ir

## Clima

Varia bastante, en general es un clima estable y moderado. Aunque el agua tiende a estar congelada.

## Comercio

Existen valiosas gemas y artefactos en el interior de la infraoscuridad.

# 📜 Historia

La historia de la Infraoscuridad es anterior y paralela a la del mundo de la superficie. Las razas progenitoras surgieron en la Infraoscuridad y se extinguieron con el tiempo o fueron asesinadas cuando sus equivalentes se retiraron bajo tierra ante la oposición de nuevas razas como los elfos y los enanos. Las razas antiguas, como los kuo-toas, desaparecieron de la superficie antes de que se registrara la historia humana o élfica. Las pruebas del origen de los illithids son escasas, pero los sabios creen que los destructores de mentes surgieron casi al mismo tiempo que los kuo-toas o invadieron desde otro plano durante el apogeo de ese imperio. Los aboletos también son antiguos, pero la historia de sus maquinaciones desde la baja Infraoscuridad ha quedado sin registrar.

# ✏️ Notas

#TBD

# Otros

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