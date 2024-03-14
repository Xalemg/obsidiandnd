---
fileClass: Punto de interes
tags:
  - "#PuntoDeInteres"
  - "#Lugar"
aliases: 
icon: "![[Fortaleza de Norias.webp]]"
Tematica:
  - Caballerosidad
  - Intriga
Tipo: Fortaleza
Prosperidad: Medio
Defensas:
  - Una guarnición de unos 200 soldados defienden el perimetro de la muralla y de la torre
Ubicacion: "[[Crestafria]]"
Mundo:
  - Aretries
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Temática** | `VIEW[{Tematica}][text(renderMarkdown)]` |

# 🔍 A simple vista

La fortaleza de Norias es la tercera más grande de la ciudad.

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Otros

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