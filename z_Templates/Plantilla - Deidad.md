---
fileClass: Deidad
aliases: 
tags:
  - Deidad
icon: "![[placeholderImage.png]]"
Dominio: 
Sequito:
  - ""
simple: ""
Simbolo: 
Prohibido: 
Estado: 
RangoDeidad: 
Alineamiento: 
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
> **Prohibido** | `=this.=this.Simbolo
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `INPUT[inlineList:Simbolo]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |
# 🔍 A simple vista

#TBD
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
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
