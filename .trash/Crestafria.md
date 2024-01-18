---
fileClass: Asentamiento
tags:
  - settlement
prosperity: Muy Bajo
Kingdom: "[[Template - Player]]"
defenses: 
leaders:
  - "[[Template - ShopService]]"
theme: 
population: 122
type: Ciudad
aliases: []
location: "[[The Wandering Bard Tavern]]"
overview: |
  asdadadas das asd **asdads** asdas
icon: ![[z_Assets/Amaunator.jpg
emblem: 
ruler: 
Terain: 
---

> [!infobox| background-black ]+
> `VIEW[{icon}][text(renderMarkdown)]`
> ###### Info
>  |
> ---|---|
>  **Ubicación** | `=link(this.location)` |
> **Alias** |`=this.aliases` |
> **Tipo** | `=this.type` |
> **Población** | `=this.population` |
> **Temática** | `=this.theme` |
> **Nación** | `=link(this.Kingdom)` |
> **Terreno** | `=this.terrain` |
> ###### Política
>  |
> ---|---|
> **Gobernantes** | `=this.rulers` |
> **Lideres** | `INPUT[inlineListSuggester(optionQuery("7.Asentamientos"))]` |
> **Tipo de gobierno** | `=this.GovtType` |
> **Defensas** | `=this.defences` |
> **Religiones** | `=link(this.religions)` |
> ###### Comercio
>  |
> ---|---|
> **Prosperidad** | `=this.prosperity` |
> **Importacioness** | `=this.imports` |
> **Exportaciones** | `=this.exports` |
# **`=this.file.name`**
> [!metadata|overview]+ A simple vista 
> ```meta-bind
INPUT[editor:overview]
>```


> [!metadata|map]+ Mapa
> ```leaflet
> id: TBD
> image: [[PlaceholderImage.png]]
> height: 600px
> width: 640px
> lat: 50
> long: 50
> minZoom: 1
> maxZoom: 5
> defaultZoom: 1
> unit: meters
> scale: 1
> darkMode: false
> ```

> [!metadata|districts]+ Distritos
> [[🪧 District Database|🪧Add New District]]
> ```dataview
table join(aliases, ", ") AS Aliases, join(type, ", ") AS Types
WHERE Settlement = this.file.name AND contains(NoteIcon, "District")
SORT file.name ASC

> [!metadata|shops]+ Tiendas y Servicios
> [[💲 Shop & Service Database|📝Add New Shop/Service]]
> ```dataview
table join(aliases, ", ") AS Aliases, join(type, ", ") AS Types
WHERE Location = this.file.name AND contains(NoteIcon, "Shop")
SORT file.name ASC

> [!metadata|pois]+ Puntos de interes
> [[❓ POI Database|📝Add New Point of Interest]]
> ```dataview
table join(aliases, ", ") AS Aliases, join(type, ", ") AS Types
WHERE Location = this.file.name AND contains(NoteIcon, "POI")
SORT file.name ASC

> [!metadata|groups]+ Grupos
> [[🔰 Group Database| 🔰 Add New Group]]
> ```dataview
table join(aliases, ", ") AS Aliases, join(type, ", ") AS Types
WHERE econtains(Location, this.file.name) AND contains(NoteIcon, "Group")
SORT file.name ASC

> [!metadata|characters]+ NPCs
> [[👨‍👩‍👧‍👦 NPC Database| 📝Add New NPC]]
> ```dataview
table join(aliases, ", ") AS Aliases, join(occupation, ", ") AS "Occupations", join(link(associatedgroup), ", ") AS "Groups"
WHERE Location = this.file.name AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT file.name ASC

### 🎯 Objetivo

## 📜Historia

## 🗒️Notas

