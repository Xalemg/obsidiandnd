---
fileClass: Deidad
tags:
  - Deidad
icon: "![[umberlee.png]]"
Dominio:
  - Tempestad
Sequito:
  - Piratas, corsarios, contrabandistas y marinos que temen el mar
RangoDeidad: Deidad Intermedia
Alineamiento: CM
Estado: Vivo
Prohibido: Si
Simbolo:
  - Holas abriendose a izquierda y derecha
---

> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
> **Dominio** | `=this.Dominio` |
> **Rango Deidad** | `=this.RangoDeidad` |
> **Alineamiento** | `=this.Alineamiento` |
> **Estado** | `=this.Estado` |
> **Prohibido** | `=this.Prohibido` |
> **Alias** |`=this.aliases` |
> **Simbolo Sagrado** | `=this.Simbolo` |
> **Sequito** | `=this.Sequito` |
# 🔍 A simple vista

El avatar de la reina del mar, pocas veces visto, era una mujer gigante con el cuerpo coloreado como el mar, de azules y verdes. Sus manos tenían garras. Sus codos tenían aletas. Tenía el pelo verde de las algas marinas. Sus ojos blancos recordaban a las perlas, y su voz sonaba como la más feroz tormenta marina, retumbando con las olas rompiendo.
>Lo que importa son las monedas. Y para ganar monedas, uno necesita carreteras... o el amor de Umberlee.
# 🎯Objetivos

#TBD
# 📜 Historia

#TBD
# ✏️ Notas

#TBD

> [!metadata|pois]+ Localizaciones de culto
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Tematica
FROM #Lugar
WHERE  contains(Religion, [[]])
SORT file.name ASC

> [!metadata|characters]+ Seguidores
> ```dataview
table without ID file.name AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
