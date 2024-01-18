---
fileClass: Deidad
tags:
  - Deidad
icon: "![[vecna.png]]"
Dominio:
  - Muerte
  - Arcano
  - Conocimiento
Sequito:
  - Eruditos sin moral que buscan conocimientos perdidos o necroticos
RangoDeidad: Deidad Menor
Alineamiento: CM
Estado: Vivo
Prohibido: Si
Simbolo:
  - Mano y ojo
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

Vecna tiene apariencia de lich. Le falta un ojo y la mano, mientras que el derecho brilla con una luz verde intensa.
# 🎯Objetivos

#TBD
# 📜 Historia

Vecna fue un lich antaño humano de Oerth que ascendió a la divinidad Su comandante se llamaba Kas
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
