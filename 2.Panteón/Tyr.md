---
fileClass: Deidad
tags: Deidad
icon: "![[tyr simbolo.png]]"
Dominio:
  - Orden
  - Guerra
Alineamiento: LB
Prohibido: No
Estado: Deidad Principal
Simbolo:
  - Balanza sobre un martillo
Sequito:
  - Magistrados y jueces, especialmente humanos
RangoDeidad: Deidad Principal
---

> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
> **Dominio** | `VIEW[{Dominio}][text(renderMarkdown)]` |
> **Rango Deidad** | `VIEW[{RangoDeidad}][text(renderMarkdown)]` |
> **Alineamiento** | `VIEW[{Alineamiento}][text(renderMarkdown)]` |
> **Prohibido** | `VIEW[{Prohibido}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Simbolo Sagrado** | `VIEW[{Simbolo}][text(renderMarkdown)]` |
> **Sequito** | `VIEW[{Sequito}][text(renderMarkdown)]` |
# 🔍 A simple vista
![[Tyr.jpg | left portrait]]
Se ocupaba principalmente del castigo de los malhechores y de la promoción general de la ley y el bien en el mundo. Tyr odiaba la duplicidad, el engaño, el incumplimiento de las normas y la destrucción gratuita. Asimismo, odiaba las mentiras y la ruptura de los juramentos, y le repugnaban las personas que ganaban dinero con tales cosas. Por su parte, nunca rompería una promesa.
> Un buen hombre es un martillo en la mano de Tyr.

---
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
