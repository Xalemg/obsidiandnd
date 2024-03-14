---
fileClass: Deidad
tags: Deidad
icon: ![[z_Assets/Misc/PlaceholderImage.png
Dominio: []
Sequito: ""
simple: ""
---

> [!infobox| background-black ]+
> `=this.Ubicacion`
> ###### Info
>  |
> ---|---|
> **Dominio** | `VIEW[{Dominio}][text(renderMarkdown)]` |
> **Rango Deidad** | `INPUT[rangoDeidadTemplate][:Estado]` |
> **Alineamiento** | `VIEW[{Alineamiento}][text(renderMarkdown)]` |
> **Estado** | `VIEW[{Estado}][text(renderMarkdown)]` |
> **Prohibido** | `VIEW[{Prohibido}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `VIEW[{Simbolo}][text(renderMarkdown)]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |
> **Lugares de culto** | `=this.Ubicaciones` |> **Lugares de culto** | `INPUT[suggester(optionQuery(#lugar), defaultValue(-),option(Ninguna, Ninguna)): Culto]` |

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
