---
fileClass: Faccion
tags:
  - Faccion
aliases:
  - Reino de Altalos
icon: "![[z_Assets/Emblemas/altalos.png]]"
Mundo:
  - Aretries
Ubicacion: "[[Islas Shamal]]"
Tipo:
  - Monarquia
Lideres: "[[5.NPCs/Rey Kemdal.md|Rey Kemdal]]"
Influencia: Muy Alta
Rangos:
  - Rey (Lider)
  - Caballero
  - Reina
  - Consejero Principal
  - Aprendiz de mago
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

El principal reino humano de todas las Islas, es el segundo mayor poder militar y político de la Mancomunidad. Altalos es un reino de caballeria valor y guerra. El choque entre su tradicional espiritu caballeresco y militar y el avance social de las [Islas Shamal](https://www.notion.so/Islas-Shamal-af54fc3c476941eb9b59243abb9a5ecb?pvs=21) constituyen el mayor reto al que se enfrenta el Reino. La fe de [Tyr](https://www.notion.so/Tyr-fa8b9ab1d1ab4831a2037552cc9307c8?pvs=21) es la principal de sus fes, aunque existen cada vez más seguidores de [Trithereon](https://www.notion.so/Trithereon-3204e07a48fc409daef59c72270bfb4c?pvs=21).

## Mercenarios

Numerosas bandas mercenarias viajan por este reino prestando servicio a aquellos que pueden permitírselo.

### Compañía del Grifo

Guardia de elite del rey

### La legión ardiente

Compañía rebelde que juro vengar la ofensa de la familia real y que se opone a esta en cada conflicto posible

### Los colmillos quebrados

Compañía dedicada a la protección del pueblo llano, en conflictos importantes tienden a aliarse con

# 📜 Historia

La corona de altalos llego junto a las migraciones humanas que abandonaron Tramonto tras la plaga gris aproximadamente en el -2000AM. En Altalos expulsaron a los Elfos tras su llegada a la [[Isla de Altalos]] y fundaron la ciudad de [[Crestafria]]. Desde entonces el reino se ha visto rodeado en una serie de guerras, principalmente internas.
# ✏️ Notas

#TBD

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]]) AND !contains(Estado, "Muerto")
SORT file.name ASC
