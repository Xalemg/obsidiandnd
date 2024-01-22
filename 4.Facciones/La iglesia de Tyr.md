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
Ubicacion: "[[Isla de Altalos]]"
Rangos: [Obispo Supremo, Obispo, Hermano]
Lider: "[[Anais]]"
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

#TBD

# 🎯Objetivos

#TBD


# 📜 Historia

#TBD

# ✏️ Notas

#TBD

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.name AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
