---
fileClass: Punto de interes
tags:
  - PuntoDeInteres
  - "#Lugar"
aliases: 
icon: "![[Catedral de Tyr.png]]"
Tematica: [Religiosa, Reflexion, Deber]
Tipo: Templo
Prosperidad: Medio
Defensas: Paladines y clerigos de Tyr
Ubicacion: "[[Crestafria]]"
Mundo:
  - Aretries
---


> [!infobox| background-black ]+
`VIEW[{icon}][text(renderMarkdown)]`
> ###### Información basica
>  |
> ---|---|
>  **Ubicación** | `VIEW[{Ubicacion}][link]` |
> **Alias** |`=this.aliases` |
> **Tipo** | `=this.Tipo` |
> **Temática** | `=this.Tematica` |

# 🔍 A simple vista
Gignatesca Catedral con forma de martillo. Hace a los vio andantes sentirse pequeños. Parece tener varias plantas y esta decorado con distintas vidrieras con escenas de la [[Corona de Altalos| ]] de un martillo gigante se encuentra incrustado en el centro de la catedral. Catedral del Martillo
El mayor edificio de rezo de Tyr. Aquí se producen los juicios mas importantes del Reino
# 📜 Historia
#TBD

# ✏️ Notas
 El martillo pertenece a la caballera Filda, Una de las mayores caballeras del primer Rey de Altalos, [[Julio Altalos]]

# Ubicaciones



> [!metadata|characters]+ NPCs
> ```dataview
table without ID file.link AS Nombre, join(aliases, ", ") AS Aliases, join(Oficios, ", ") AS "Oficios", Alienamiento
FROM #NPC
WHERE  contains(Ubicacion, [[]]) AND !contains(Estado, "Muerto" )
SORT file.name ASC