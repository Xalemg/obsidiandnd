---
fileClass: Faccion
tags:
  - Faccion
  - Relevante
aliases: 
icon: "![[La escama plateada.png]]"
Mundo:
  - Aretries
Influencia: Alta
Alineamiento: NB
Tipo: Agentes secretos
Ubicacion: "[[Isla de Altalos]]"
Rangos: Dragona (Lider)
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
La escama plateada es un grupo de agentes secretos que actua en la [[Isla de Altalos]]. Su objetivo es un misterio para la mayoría de la gente.
# 📜 Historia

#TBD

# ✏️ Notas

#TBD

> [!characters|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
