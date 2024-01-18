---
fileClass: Deidad
tags:
  - Deidad
icon: "![[lolth.png]]"
Dominio:
  - Engaño
Sequito:
  - Drows malvados
Simbolo:
  - estrella de 8 puntas con gema roja en el centro
Prohibido: Si
Estado: Encadenado
RangoDeidad: Deidad Menor
Alineamiento: CM
aliases:
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
![[Lolthwebp.webp | wsmall left]]
Lolth era una diosa de cruel frialdad, no fuera de lugar en las profundidades más oscuras del interminable Abismo, disfrutando de la traición y el derramamiento de sangre, y burlándose tanto de sus secuaces como de sus víctimas. No solo disfrutaba, sino que prosperaba en la tortura, destrucción y muerte, ya sea ejecutándolas personalmente o causándolas. Cada interacción se realizaba en última instancia con malicia, con malevolencia brotando de cada movimiento suyo, e incluso aquellos que la conocían bien podían sorprenderse por la profundidad de su ferocidad. Su malicia podía compararse con la ira del brutal dios orco Gruumsh, pero mientras que su furia era tan violentamente ciega como una fuerza de la naturaleza, la malicia de Lolth era complicada y deliberada. Además, se podría decir que Gruumsh al menos era constante en su odio, mientras que el de Lolth era completamente caprichoso.

>La espera es el camino de Lolth, la ambición que ella otorga para fomentar el caos, para mantener a sus "hijos" drow en su curso designado de auto-prisión.
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
