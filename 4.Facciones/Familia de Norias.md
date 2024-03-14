---
fileClass: Faccion
tags:
  - Faccion
aliases: 
icon: "![[Fortaleza de Norias.webp]]"
Mundo: Aretries
Influencia: Media
Alineamiento: NB
Tipo: Familia Nobiliaria
Rangos: [Cabeza de familia, Hija menor, Padre, Familiar lejano]
Lider: 
Ubicacion: ["[[Isla de Altalos]]", "[[Fortaleza de Norias]]"]
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicaciones** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Alineamiento** | `VIEW[{Alineamiento}][text(renderMarkdown)]` |
> **Lideres** | `VIEW[{Lideres}][text(renderMarkdown)]` |
> **Rangos** | `VIEW[{Rangos}][text(renderMarkdown)]` |
> **Influencia** | `VIEW[{Influencia}][text(renderMarkdown)]` |




# 🔍 A simple vista

La familia de Norias es una de las casas Nobles más influentes de Altalos. Generalmente se ha posicionado del lado de la [[Corona de Altalos]] y suelen tener confesión superiores al resto de los ducados. 

# 🎯Objetivos

Incrementar su influencia en el reino.


# 📜 Historia

Históricamente, se ha considerado su apoyo como uno de los mas importantes durante las guerras civiles del reino.

# ✏️ Notas

#TBD

> [!characters|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
