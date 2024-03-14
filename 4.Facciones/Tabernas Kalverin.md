---
fileClass: Faccion
tags:
  - Faccion
aliases: 
icon: "![[tabernas kalverin.png]]"
Mundo: Aretries
Influencia: Media
Alineamiento: LN
Tipo: Franquicia
Ubicacion: "[[Islas Shamal]]"
Rangos: 
Lider: 
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicaciones** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Alineamiento** | `VIEW[{Alineamiento}][text(renderMarkdown)]` |
> **Lideres** | `VIEW[{Lideres}][text(renderMarkdown)]` |
> **Rangos** | `VIEW[{Rangos}][text(renderMarkdown)]` |
> **Influencia** | `VIEW[{Influencia}][text(renderMarkdown)]` |




# 🔍 A simple vista

Una cadena de Tabernas establecidas a lo largo de todas las [[Islas Shamal]]. Están todas dirigidas por Warforged llamados Kevin. Cada taberna intenta adaptarse a las costumbres y tópicos locales.
# 🎯Objetivos

Ganar money.

# 📜 Historia

#TBD

# ✏️ Notas

> [!characters|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
