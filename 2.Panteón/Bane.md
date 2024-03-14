---
fileClass: Deidad
tags:
  - Deidad
icon: "![[hand bane.webp]]"
Dominio:
  - Guerra
  - Orden
Sequito:
  - Hombre avariciosos de baja moral y mercaderes con pretensiones de progresar y pocos escrúpulos
RangoDeidad: Deidad Menor
Alineamiento: LM
Estado: Vivo
Prohibido: Si
Simbolo:
  - Mano Negra
---

> [!infobox| background-black ]+
`VIEW[[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
> **Dominio** | `VIEW[{Dominio}][text(renderMarkdown)]` |
> **Rango Deidad** | `VIEW[{RangoDeidad}][text(renderMarkdown)]` |
> **Alineamiento** | `INPUT[alineamiento][:Alineamiento]` |
> **Estado** | `VIEW[{Estado}][text(renderMarkdown)]` |
> **Prohibido** | `VIEW[{Prohibido}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `VIEW[{Simbolo}][text(renderMarkdown)]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |
# 🔍 A simple vista

Musculado y enorme individuo de piel oscura, pequeños cuernos asoman por su cabeza y barbilla.
>Elijo gobernar por toda la eternidad como el tirano supremo. Puedo inducir el odio y la lucha a mi antojo, y todos se inclinarán ante mí mientras estén en mi reino.
# 🎯Objetivos

#TBD
# 📜 Historia

Antes de El ultimo dia de los dioses mato a Haduuz el campeon de Mielikki y lo convirtio en su capitan, logrando asi que acabara con su antuga deida
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
