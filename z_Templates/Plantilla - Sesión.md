---
banner: "![[lazy_dm_workbook_banner.jpg]]"
banner_y: 0.36
fileClass: Sesion
Mundo: 
cssclasses:
  - card-images
  - t-w
---
# [[Personajes]]
>[!cards| dataview 7]
>```dataview
>table without id embed(link(icon)) as Icono,
>"**"+file.link +"**",
>"**P.Pasiva: "+P_per+"**",
>"**AC: "+ac+"**",
>"**Max HP: "+hp+"**"
>FROM #personaje
>WHERE contains(En_curso, "si") AND contains(Campaña,this.Campaña)
>```


>[!dataview  | right clean no-t nmg ]
># [[3.Lugares]]
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
# 🔐Secretos y pistas
*Secretos sobre el villano/enemigos, objetivo de los PJs, aliados, lugares que visitan, eventos relevantes, objetos mágicos o la misión.*
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 

# 🎥Situaciones probables
*Situaciones probables que vayan a darse durante la sesión.*
## Situación 1


# ⚔️ Encuentros
*Un encuentro puede ser mortal si la suma total de los valores de desafío de los monstruos es superior a la mitad de la suma total de los niveles de los personajes o a un cuarto de os niveles de los personajes si estos son de 4º nivel o inferior.*
`encounter: 1: goblin`
# 💰Tesoro
Ejemplo
# ⏯️Grabación


# 📝 Notas