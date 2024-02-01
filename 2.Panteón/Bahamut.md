---
fileClass: Deidad
tags: Deidad
icon: "![[Bahamut_holy_symbol.png]]"
Dominio:
  - Guerra
Sequito:
  - Principalmente dragones metalicos y draconicos
simple: ""
RangoDeidad: Deidad Principal
Alineamiento: LB
Estado: Desconocido
Prohibido: No
Simbolo:
  - Cabeza de un dragón platino
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
![[Bahamut.webp|right tinyl]]
Bahamut fue el primer padre. El junto a Tiamat crearon a los dragones a su imagen y semejanza. Tras la creación del resto de razas por el resto de los dioses, provocó la división entre ellos. Bahamut pensaba que los dragones debían compartir Aretries con el resto de razas mientras que Tiamat quería acabar con el resto de los Dioses. Bahamut tras ver que Tiamat enviaba ordenaba a los dragones cromáticos a aniquilar a los metálicos, creo las Perlas del Alma. Estas permitían a los dragones escapar.

# 🎯Objetivos

Proteger el legado de los dragones metalicos
# 📜 Historia

Bahamut fue el primer padre. El junto a Tiamat crearon a los dragones a su imagen y semejanza. Tras la creación del resto de razas por el resto de los dioses, provocó la división entre ellos. Bahamut pensaba que los dragones debían compartir Aretries con el resto de razas mientras que Tiamat quería acabar con el resto de los Dioses. Bahamut tras ver que Tiamat enviaba ordenaba a los dragones cromáticos a aniquilar a los metálicos, creo las Perlas del Alma. Estas permitían a los dragones escapar.
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
