---
fileClass: Deidad
tags:
  - Deidad
icon: "![[adur2.png]]"
Dominio:
  - Naturaleza
Sequito:
  - Principalmente en Adur por aquellos que buscan defender la naturaleza.
RangoDeidad: Deidad Intermedia
Alineamiento: NB
Estado: Vivo
Prohibido: No
Simbolo:
  - perfil de un caballo blanco de crin dorada y rosas en el cuello
Ubicaciones:
---

> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
> **Dominio** | `VIEW[{Dominio}][text(renderMarkdown)]` |
> **Rango Deidad** | `VIEW[{RangoDeidad}][text(renderMarkdown)]` |
> **Alineamiento** | `VIEW[{Alineamiento}][text(renderMarkdown)]` |
> **Estado** | `VIEW[{Estado}][text(renderMarkdown)]` |
> **Prohibido** | `VIEW[{Prohibido}][text(renderMarkdown)]`
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `INPUT[inlineList:Simbolo]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |
# 🔍 A simple vista

Dios de la naturaleza que aparece como un caballo de crin dorada. Nacido de la antigua y difunta diosa de la naturaleza
>Aquel que riega una flor acabara cultivando un jardín.
# 🎯Objetivos

Disfrutar de la libertad
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
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
