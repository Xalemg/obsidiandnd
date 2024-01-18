---
fileClass: Deidad
tags:
  - Deidad
icon: "![[karl.png]]"
Dominio:
  - Forja
  - Conocimiento
Sequito:
  - Magos, Alquimistas, Artificieros e ingenieros sobretodo gnomos y enanos
RangoDeidad: Deidad Menor
Alineamiento: NB
Estado: Vivo
Prohibido: No
Simbolo:
  - Cubo dorado extraño
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
![[Karl Brillabomba.png| left ]]
Karl Brillabomba es representado por un gnomo de de pelo cano y rasgos afilados. Suele ser representado con muchos de sus inventos en la mano o junto a ellos.
>La creacion es la clave de la existancia
# 🎯Objetivos

#TBD
# 📜 Historia

#TBD
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
