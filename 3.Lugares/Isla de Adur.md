---
fileClass: Lugar
tags:
  - Lugar
aliases: 
icon: "![[Adur.png]]"
Poblacion: ""
Nacion: "-"
Gobernantes:
  - "-"
Tematica:
  - Naturaleza
  - Progreso
  - Ecologismo
Tipo: Subcontinente
Prosperidad: Alto
Importaciones: 
Mundo: Aretries
Ubicacion: "[[3.Lugares/Islas Shamal.md|Islas Shamal]]"
Terreno: [Archipielagos]
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `=Ubicacion` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Población** | `=this.Poblacion` |
> **Temática** | `VIEW[{Rangos}][text(renderMarkdown)]` |
> **Terreno** | `VIEW[{Terreno}][text(renderMarkdown)]`|

# 🔍 A simple vista

#TBD

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Otros

> [!metadata|pois]+ Localizaciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Tematica
FROM #Lugar
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!facciones|facciones]+ Facciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Influencia
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!characters|characters]+ NPCs
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, join(Oficios, ", ") AS "Oficios", Alienamiento
FROM #NPC
WHERE  contains(Ubicacion, [[]]) AND !contains(Estado, "Muerto" )
SORT file.name ASC