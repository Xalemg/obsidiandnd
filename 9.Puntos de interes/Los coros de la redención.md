---
fileClass: Punto de interes
tags:
  - "#PuntoDeInteres"
  - "#Lugar"
aliases: 
icon: "![[coros de la redención.png]]"
Tematica:
  - Descanso
  - Religiosa
Tipo: Taberna
Prosperidad: Medio
Defensas:
  - Paladines y clerigos de Tyr
Ubicacion: "[[Crestafria]]"
Mundo:
  - Aretries
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Temática** | `VIEW[{Rangos}][text(renderMarkdown)]` |
>   ## NPCs
>   ```dataview
table without ID  file.link AS Nombre, Raza
FROM #NPC
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC
>```
> ## Localizaciones
>   ```dataview
table rows.file.link AS Nombre
FROM #Lugar
WHERE  contains(Ubicacion, [[]])
GROUP BY Tipo
SORT file.name ASC
>```
>   ## Facciones
> ```dataview
table without ID  file.link AS Nombre
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.Tipo ASC
# 🔍 A simple vista
Multiples sacerdotes novicios reparten comida entre las mesas.

[[Juanlu]], un paladin con lazos con la iglesia de [[Tyr]] regenta la taberna los clérigos cantan en tramontes todos los días dando 2d6+2 puntos de golpe temporales a los parroquia que escuchan.

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Otros
