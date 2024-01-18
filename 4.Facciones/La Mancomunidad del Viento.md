---
fileClass: Faccion
tags:
  - Faccion
aliases:
  - La mancomunidad
icon: "![[z_Assets/Emblemas/emblema mancomunidad.png]]"
Mundo: Aretries

Tipo:
  - Confederación
Alineamiento: LB
Rangos:
  - Emir (Lider)
  - Representante (Bajo el Emir)
Influencia: Muy Alta
Ubicacion: "[[Islas Shamal]]"
Lider: 
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

La mancomunidad está dirigida por el Emir, (un cargo elegido en un enrevesado proceso de votaciones y sorteos) que gobierna junto con los líderes de las naciones integrantes. A grandes rasgos la Mancomunidad se centra en regular el comercio, las relaciones con el extranjero, el aprendizaje de la magia arcana y el culto a los dioses.
> Governantes de los mares, governantes del progreso, governantes de la diversidad
La gran mayoría de las Islas Shamal se encuentra bajo el amparo de la Mancomunidad del Viento.


**Sus principales políticas son:**

1. Cualquier miembro atacado por poderes extranjeros debe ser defendida por todos los miembros.
2. La guerra entre miembros queda totalmente prohibida.
3. Ningún miembro puede intervenir bajo ningún concepto en los conflictos internos de otro de los miembros.

El incumplimiento de estos puntos está castigado con sanciones comerciales y en casos extremos la expulsión.

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.link as Nombre,  join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
WHERE Faccion = this.file.name AND "#NPC"
SORT file.name ASC
