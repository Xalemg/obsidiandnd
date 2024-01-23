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
>  **Ubicaciones** | `=this.Ubicacion` |
> **Alias** |`=this.aliases` |
> **Tipo** | `=this.Tipo` |
> **Alineamiento** | `=this.Alineamiento` |
> **Lideres** | `=this.Lideres` |
> **Rangos** | ``=this.Rangos`` |
> **Influencia** | `=this.Influencia` |




# 🔍 A simple vista

Una cadena de Tabernas establecidas a lo largo de todas las [[Islas Shamal]]. Están todas dirigidas por Warforged llamados Kevin. Cada taberna intenta adaptarse a las costumbres y tópicos locales.
# 🎯Objetivos

Ganar money.

# 📜 Historia

#TBD

# ✏️ Notas

> [!metadata|characters]+ Miembros
> ```dataview
table without ID file.name AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
