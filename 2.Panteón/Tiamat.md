---
fileClass: Deidad
tags:
  - Deidad
icon: "![[Tiamat.png]]"
Dominio:
  - Engaño
Sequito:
  - Dragones cromáticos, draconidos malvados y cultistas
RangoDeidad: Deidad Principal
Alineamiento: CM
Estado: Vivo
Prohibido: Si
Simbolo:
  - 5 cabezas de dragones cromáticos en circulo
---

> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
> **Dominio** | `VIEW[{Dominio}][text(renderMarkdown)]` |
> **Rango Deidad** | `VIEW[{RangoDeidad}][text(renderMarkdown)]` |
> **Alineamiento** | `VIEW[{Alineamiento}][text(renderMarkdown)]` |
> **Estado** | `VIEW[{Estado}][text(renderMarkdown)]` |
> **Prohibido** | `VIEW[{Prohibido}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `VIEW[{Simbolo}][text(renderMarkdown)]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |

![[tiamat.jpg | tiny left ]]
# 🔍 A simple vista
Tiamat era un dragón cromático único, que tenía una cabeza para cada color primario de las especies cromáticas más comunes (negro, azul, verde, rojo, blanco). Cada cabeza podía operar de forma completamente independiente entre sí y tenía los poderes de un miembro de la raza respectiva de los dragones. Su cuerpo también tenía rasgos en común con un wyvern, incluida una cola larga con un aguijón venenoso en la punta.
> Muchas bocas hablan de tu hambre en este mundo, ama. Déjame ser la más ruidosa.
# 🎯Objetivos

Acabar con Bahamut
# 📜 Historia

Durante la guerra de los dioses Tiamat tuvo feroces encuentros contra Bahamut. Creo la La asamblea de los cinco colores para asegurarse que tras la guerra los grandes dragones acabaran con los hijos de Gath e Igeo ya que en ellos [[Bahamut]]  invuyo su alma para de esta forma poder regresar tras su muerte
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
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
