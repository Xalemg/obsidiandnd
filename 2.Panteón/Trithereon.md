---
fileClass: Deidad
tags:
  - Deidad
icon: "![[trithereon.png]]"
Dominio:
  - Guerra
Sequito:
  - Gente desesperada por la libertado o idealistas extremos
RangoDeidad: Semidios
Alineamiento: CB
Estado: Vivo
Prohibido: No
Simbolo:
  - Trisquel
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
# 🔍 A simple vista

Trithereon es el dios de la libertad y la rebeldía. Se caracteriza por las 3 almas que le representan y que siempre lleva consigo, su espada la Lengua de la Libertad, su lanza, Krelestro y el Bastón de la Retribución, su cetro.
>Todos merecen la vida y la capacidad de elegir su propio lugar en el mundo, y aquellos que encadenen a otros o los controlen con leyes opresivas deben ser derribados. Entrena a la gente común para que se defienda a sí misma y a sus bienes en caso de que otro quiera arrebatarles sus libertades. Si te hacen daño, tienes derecho a vengarte, sobre todo si nadie te ayuda.
# 🎯Objetivos

#TBD
# 📜 Historia

La fe en Trithereon surge de la llegada de los humanos a Altalos tras la [1700 AM La gran migración Elfica](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckk8hntpw4lu40702dazgm006) que dejo la Isla de Altalos a merced de las criaturas salvajes. En el dificultad de la dificultad de imponerse sobre las bestias salvajes surge la figura de [Trithereon](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckj7rifd8vt5c0726nvxjrs0w). Su origen exacto es desconocido pero muchos aseguran que se trataba de un hero cuya admiración por parte de los colonos de la [Isla de Altalos](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckiywq50rj0uh07268z8ioyws) elevo al estatus de dios.

Durante este periodo se unio a la [La divina alianza del orden](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckk8h683m4kwc0702okrgb8lt). Aunque cuando la victoria se hizo evidente fue el primero en abandonarla debido a grandes diferencias con el resto, en especial con [Tyr](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckjigh2xl9i6807251gfmj73h). Esto provoc que gran parte de la población cambiara su devocion por [Tyr](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckjigh2xl9i6807251gfmj73h).

Durante [2400 -1200 AM Los ultimos dias de los dioses (Los dias antiguos)](notion://www.notion.so/a/worlds/ckiypptepbkbs0725834icu5e/ckjd241fdzcpa07255nj46z4y)
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
