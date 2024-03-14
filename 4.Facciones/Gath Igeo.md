---
fileClass: Faccion
tags:
  - Faccion
aliases:
  - Jinetes de dragon
  - Vinculados a los dragones
icon: "![[gath igeo.png]]"
Mundo:
  - Aretries
Influencia: Muy Baja
Alineamiento: LB
Tipo: Guerreros justos
Rangos: 
Lider: 
Ubicacion: ["[[Islas Shamal]]", "[[Cueva del regalo]]"]
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
> 




# 🔍 A simple vista

[[Gath Igeo]] fue una sociedad de humanoides vinculados con dragones. Estos combatían en dragones. Debido a la persecución por [[Tiamat]] y la [[Asamblea de las 5 caras]]. La ciudadela alada. Existen 5 ordenes dentro de [[Gath Igeo]] cada una destacando las excelencias de cada tipo de dragón metalico:
- [[La ala dorada]] Lideres y dirigentes. Vivian aislados del resto.
- [[La escama plateada]] Guardias, protectores y espías encargados de la defensa de la [[Ciudadela alada]]  
- [[El ojo de bronce]] Jueces y legisladores. Gobernaban y buscaban mejorar [[Gath Igeo]]
- [[La voz de cobre]] Emisarios y reclutadores, se encargaban de la diplomacia y la búsqueda de personas bendecidas por [[Bahamut]]
- [[La mente de bronce]] Investigadores cientificos y teologos. La mente de Bronce se encargaba 


# 🎯Objetivos

Enfrentarse al mal, en especial a [[Tiamat]] y los agentes de la [[Asamblea de las 5 caras]]

# 📜 Historia
[[Gath Igeo]] nació cuando [[Bahamut]] dio su bendición a una familia de nobles elfos guerreros con los que colaboro durante los [[Dias de los dioses]]. Abrió las almas de sus descendientes para que pudieran ser vinculadas a las almas élficas. De esta forma lograron detener a [[Tiamat]]. Cuando los humanos llegaron a la [[Isla de Altalos]] Gath Igeo compartió su bendición con el resto de humanoides. Sin embargo la [[Asamblea de las 5 caras]] ataco la [[Ciudadela alada]] acabando con el vinculo entre humanoides y dragones, destruyendo la ciudadela y dispersando al pueblo de Gath Igeo. Tras esto la [[Gran Dragon Mandrasath]] se quedo como custodia de la ciudadela, mientras que los drows cazaban a los restos del pueblo y las perlas del alma los grandes dragones cromaticos acababan con los dragones metalicos restantes.


# ✏️ Notas

#TBD

> [!characters|characters]+ Miembros
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Rango, join(Oficios, ", ") AS "Oficios"
FROM #NPC
WHERE  contains(Facciones, [[]])
SORT file.name ASC
