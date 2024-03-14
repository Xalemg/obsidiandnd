---
fileClass: Asentamiento
tags:
  - Lugar
  - Relevante
aliases: 
icon: "![[Costa de Altalos 2.gif]]"
Poblacion: 
Nacion: "-"
Gobernantes:
  - "-"
Tematica:
  - Caballerosidad
  - Épica
  - Heroismo
Tipo: Subcontinente
Prosperidad: Medio
Importaciones: 
Mundo:
  - Aretries
Ubicacion: "[[3.Lugares/Islas Shamal.md|Islas Shamal]]"
Gobierno: 
Terreno: 
Defensas: 
Religion:
  - "[[Tyr]]"
  - "[[Trithereon]]"
  - "[[Bane]]"
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][text(renderMarkdown)]` |
> **Alias** |`VIEW[{aliases}][text(renderMarkdown)]` |
> **Tipo** | `VIEW[{Tipo}][text(renderMarkdown)]` |
> **Población** | `=this.Poblacion` |
> **Temática** | `VIEW[{Rangos}][text(renderMarkdown)]` |
> **Terreno** | `VIEW[{Terreno}][text(renderMarkdown)]`|

# 🔍 A simple vista

La Isla de Altalos en su mayoría pertenece al Reino de Altalos, sin embargo en el sur se encuentran las naciones independientes del Kanato de Garras y Leinas Duin, todos ellos miembros de la Mancomunidad. La isla se encuentra dividida por una Gigantesca Cordillera conocida como El Espinazo y su clima varía según la zona de tierra partida por el Espinazo. La mayoría de la gente se dedica a la agricultura y la Isla constituye uno de las principales fuentes de alimentos

- **Crestafria** es la mayor ciudad de la Isla con dos millones de habitantes, debido a encontrarse en el paso que conecta el Este, Oeste y Norte es el punto de mayor valor estratégico de la Isla.

### Reino de Altalos

El principal reino humano de todas las Islas, es el segundo mayor poder militar y político de la Mancomunidad. Gobernado por la familia Altalos, su historia se encuentra llena de revueltas Nobles, campesinas y opresión por la corona. Tras la muerte de su hermano mayor, el actual Rey Kemdal parece haber roto con las anteriores aspiraciones totalitarias de su padre, lo que ha provocado que muchos de sus antiguos aliados le retiren su apoyo y se encuentre en una posición delicada en la que necesita ganar el apoyo de aquellos Nobles que hace apenas unas décadas su padre pretendía eliminar.

### Kanato de Garras

El Kanato de Garras es la principal población tabaxi de las Islas. El totalitario Kan Kurai dirige a todos los que se dedican a vagar sobre las dunas.

### Leinas Duin

Escondidas tras la cordillera del Bajo Espinazo se encuentran las hermosas tierras de Leinas Duin, los pacíficos elfos de los bosques que aquí habitan se dedican a proteger sus dominios del creciente desierto que amenaza con devorarlos.

- **Los dominios salvaje**s son el hogar de aquellos monstruos y humanoides que rechazan cualquier tipo de gobierno o ley. El último punto de salvajismo descontrolado de las Islas.
- **Bajo Volcán** En algún lugar del intransitable Bajo Espinazo una colonia Drow causa problemas con los habitantes del Sur del Reino de Altalos.

# 📜 Historia

#TBD

# ✏️ Notas

#TBD

# Otros



> [!metadata|pois]+ Localizaciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Tematica
FROM #Lugar
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!facciones|facciones]+ Facciones
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, Tipo, Influencia
FROM #Faccion
WHERE  contains(Ubicacion, [[]])
SORT file.name ASC

> [!characters|characters]+ NPCs
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, join(Oficios, ", ") AS "Oficios", Alienamiento
FROM #NPC
WHERE  contains(Ubicacion, [[]]) AND !contains(Estado, "Muerto" )
SORT file.name ASC