---
fileClass: Deidad
tags:
  - Deidad
icon: "![[moradin symbol.png]]"
Dominio:
  - Forja
  - Conocimiento
Sequito:
  - Herreros e historiadores, especialmente enanos.
RangoDeidad: Deidad Intermedia
Alineamiento: LB
Estado: Vivo
Prohibido: No
Simbolo:
  - Martillo y llama
---

> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
> **Dominio** | `=this.Dominio` |
> **Rango Deidad** | `=this.RangoDeidad` |
> **Alineamiento** | `=this.Alineamiento` |
> **Estado** | `=this.Estado` |
> **Prohibido** | `=this.Prohibido` |
> **Alias** |`=this.aliases` |
> **Simbolo Sagrado** | `=this.Simbolo` |
> **Sequito** | `=this.Sequito` |
# 🔍 A simple vista
![[Moradin.png |left banner	]]

Juez severo pero justo, era la fuerza de voluntad encarnada. Inspiró los inventos de los enanos y buscó constantemente la mejora de su raza, fomentando una existencia bondadosa, inteligente y armoniosa con otras razas buenas, al tiempo que luchaba contra su orgullo y sus tendencias aislacionistas.
>Cada caída del martillo sobre el yunque, cada fuego avivado en la fragua, es un paso en un viaje que me ha marcado el propio Moradin.
# 🎯Objetivos

#TBD
# 📜 Historia

Según los mitos enanos, Moradin se encarnó en la roca, la piedra y el metal, y su alma era una brasa de fuego. Se decía que forjó a los primeros enanos a partir de metales y gemas y que les insufló alma cuando sopló sobre sus creaciones para enfriarlas. Moradin fue el responsable de desterrar a los dioses malignos de los derro y duergar de la superficie.
# ✏️ Notas

#TBD

> [!metadata|pois]+ Localizaciones de culto
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Tematica
FROM #Lugar
WHERE  contains(Religion, [[]])
SORT file.name ASC

> [!metadata|characters]+ Seguidores
> ```dataview
table without ID file.name AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
