---
banner: "![[lazy_dm_workbook_banner.jpg]]"
banner_y: 0.38692
fileClass: Sesion
Mundo:
  - Aretries
cssclasses:
  - card-images
  - t-w
  - wide
Campaña: 
Numero: 
tags:
  - Sesion
---
> [!Info]-
> - [ ] Reflexionar sobre los PJs y en cosas que les involucren con la sesión 
> - [ ] Elegir un comienzo de sesión impresionante
> - [ ] Describir la información básica
> - [ ] Pensar en las escenas probables 
> - [ ] Preparar Lugares fantasticos 
> - [ ] Revisar Facciones importantes 
> - [ ] Preparar NPCs memorables
> - [ ] Preparar Encuentros
> 	- [ ] Statblocks de los enemigos 
> 	- [ ] Mapa
> - [ ] 
# [[Personajes]]
>[!cards| dataview 7]
>```dataview
>table without id embed(link(icon)) as Icono,
>"**"+file.link +"**",
>"**P.Pasiva: "+P_per+"**",
>"**AC: "+ac+"**",
>"**Max HP: "+hp+"**"
>FROM #personaje 
>WHERE contains(En_curso, "si") and contains(Campañas, string(this.Campaña))
>```

>[!aside  | right clean no-t nmg ]
># 🔐Revelaciones claves
>*Información clave que deba ser revelada o que puede alterar la trama dramaticamente*
>- [!] 
>- [s] 
># [[3.Lugares| Lugares fantasticos]]
>```dataview
>list 
>FROM #Lugar AND #Relevante
>```
># [[4.Facciones]] 
>```dataview
>list 
>FROM #Faccion AND #Relevante
>```
># [[5.NPCs]]
>```dataview
>list 
>FROM #NPC AND #Relevante
>```




# 🎥Encuentros importantes

> [!Info]-
>*Situaciones probables que vayan a darse durante la sesión. Pensar en cuenta localización, NPCs/monstrups, comportamientos, importancia y posibles eventos*
## Encuentro fuerte 1
*Empezar fuerte la sesión con algo que enganche*
## Encuentro 2

## Encuentro 3

# 💰Tesoro
Ejemplo
# ⏯️Grabación


# 📝 Notas