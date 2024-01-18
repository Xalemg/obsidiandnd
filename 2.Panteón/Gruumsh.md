---
fileClass: Deidad
tags:
  - Deidad
icon: "![[gruumsh.png]]"
Dominio:
  - Tempestad
  - Naturaleza
Sequito:
  - Orcos guerreros y cazadores que le adoran por su fuerza. Shamanes y marineros que buscan su permiso en la navegación
RangoDeidad: Deidad Menor
Alineamiento: CN
Estado: Vivo
Prohibido: Si
Simbolo:
  - Ojo
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

Gruumsh normalmente aparece como un orco corpulento de 3 metros de altura cubierto de cicatrices de batalla y vestido con una armadura de malla de placas negra y reluciente. Tiene solo el ojo derecho con una cuenca vacia en el izquierdo.
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
