---
fileClass: Faccion
tags:
  - Faccion
aliases: 
icon: "![[tyr simbolo.png]]"
Mundo: Aretries
Influencia: Alta
Alineamiento: LB
Tipo: Teologica
Ubicacion: ["[[Crestafria]]", "[[Isla de Altalos]]"]
Rangos:
  - Obispo Supremo
  - Obispo
  - Hermano
Lider: "[[Anais]]"
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

#TBD

# 🎯Objetivos

#TBD


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
