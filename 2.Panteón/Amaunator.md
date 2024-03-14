---
fileClass: Deidad
tags:
  - Deidad
icon: "![[Amaunator.png]]"
Dominio: [Paz, Luz]
Sequito:
  - Principalmente dragones metalicos y draconicos
RangoDeidad: Deidad Principal
Alineamiento: LB
Estado: Muerto
Prohibido: No
Simbolo:
  - Sol dorado
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
> **Prohibido** | `VIEW[{Prohibido}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `VIEW[{Simbolo}][text(renderMarkdown)]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |
# 🔍 A simple vista

El avatar de Amaunator, cuya piel desprendía una luz dorada, tenía el aspecto de un hombre larguirucho, de pelo blanco plateado y largo, con una barba blanca tendida, vestido con un traje largo y fluido, negro o morado, con adornos plateados o dorados, el uniforme de un magistrado.

# 🎯Objetivos

Asegurar la paz en las [[Islas Shamal]] a cualquier precio.
# 📜 Historia
[[Amaunator]] promulgo la necesidad de que los dioses abandonaran [[Aretries]] para que las criaturas que aqui lo habitan pudieran vivir en paz.
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
