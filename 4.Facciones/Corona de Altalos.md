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
Rangos: [Rey (Lider), Caballero, Reina, Consejero Principal]
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

La corona de altalos llego junto a las migraciones humanas que abandonaron Tramonto tras la plaga gris aproximadamente en el -2000AM. En Altalos expulsaron a los Elfos tras su llegada a las [[Isla de Altalos]]y fundaron la ciudad de [[Crestafria]]. Desde entonces el reino se ha visto rodeado en una serie de guerras, principalmente internas.
# ✏️ Notas

#TBD

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
