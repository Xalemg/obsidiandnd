---
fileClass: Deidad
tags:
  - Deidad
icon: "![[mystra.png]]"
Dominio:
  - Magia
Sequito:
  - Magos y estudiosos de la magía arcana
RangoDeidad: Deidad Principal
Alineamiento: LN
Estado: Vivo
Prohibido: No
Simbolo:
  - Un hilo vertical con tres lunas de fondo
---

> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
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

>Soy Mystra. Soy la Dama del Poder y la Señora de la Magia. Soy la encarnación del poder. Dondequiera que se haga magia, allí estoy yo: desde los fríos polos de Aretries hasta sus junglas más cálidas, ¡sea cual sea la mano, la garra o la voluntad que haga magia! ¡Contempladme y temedme! Pero mírame y ámame, como hacen todos los que me tratan con honestidad. Este mundo es mi dominio. Yo soy la magia, la más poderosa entre todas las que los hombres adoran. Soy el Único Hechizo Verdadero en el corazón de todos los hechizos. No hay otro.
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
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
