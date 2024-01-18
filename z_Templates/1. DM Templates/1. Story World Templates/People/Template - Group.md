---
fileClass: Facciones
---
> [!infobox| background-black ]+
> # `=this.file.name`
> ![[PlaceholderImage.png]]
> ###### Información basica
>  |
> ---|---|
> **Alias** | `=this.alias` |
> **Localizaciones** | `=link(this.localizaciones)` |
> **Religión asociada** | `=link(this.associatedreligion)` |
> **Alineamiento** | `=this.alineamiento` |
> **Influencia** | `=this.influencia` |
> **Tipo** | `=this.tipo` |

> >Cita
# **`=this.file.name`**
> [!metadata|overview]+ A simple vista
TBD

> [!metadata|characters]+ Miembros
> [[👨‍👩‍👧‍👦 NPC Database| 📝Add New NPC]]
> ```dataview
table join(link(Rango), ", ")  AS Rango, join(Occupation, ", ") AS "Occupation(s)", join(link(AssociatedGroup), ", ") AS "Group(s)", join(link(AssociatedReligion), ", ") AS "Religion(es)"
WHERE contains(AssociatedGroup, this.file.name) AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT file.name ASC


### 🎯 Objetivo

## 📜Historia

## 🗒️Notas

