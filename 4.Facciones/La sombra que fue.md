---
fileClass: Faccion
tags:
  - Faccion
  - relevante
aliases: 
icon: "![[la sombra que fue.png]]"
Mundo: Aretries
Tipo:
  - Demoniaca
Alineamiento: CM
Influencia: Baja
Ubicacion: 
Rangos:
  - Padre(Lider)
  - Hija menor
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
