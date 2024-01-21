---
fileClass: Faccion
tags:
  - Faccion
aliases: 
icon: "![[z_Assets/Emblemas/altalos.png]]"
Mundo: Aretries
Ubicacion: "[[Islas Shamal]]"
Tipo:
  - Monarquia
Lideres: "[[5.NPCs/Rey Kemdal.md|Rey Kemdal]]"
Influencia: Muy Alta
Rangos:
  - Rey (Lider)
  - Caballero
  - Reina
Alineamiento: LB
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
> **Rangos** | `=this.Rangos` |
> **Influencia** | `=this.Influencia` |




# 🔍 A simple vista

#TBD

# 📜 Historia

La corona de altalos expulso a los Elfos cuando los humanos llegaron a la la [[Isla de Altalos]]. Fundaron la ciudad de [[Crestafria]] 

# ✏️ Notas

#TBD

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
