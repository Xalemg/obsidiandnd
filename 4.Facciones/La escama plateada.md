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
>  **Ubicaciones** | `=this.Ubicacion` |
> **Alias** |`=this.aliases` |
> **Tipo** | `=this.Tipo` |
> **Alineamiento** | `=this.Alineamiento` |
> **Lideres** | `=this.Lideres` |
> **Rangos** | ``=this.Rangos`` |
> **Influencia** | `=this.Influencia` |




# 🔍 A simple vista
La escama plateada es un grupo de agentes secretos que actua en la [[Isla de Altalos]]. Su objetivo es un misterio para la mayoría de la gente.
# 📜 Historia

#TBD

# ✏️ Notas

#TBD

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
