---
Tipo: Sesion
tags:
  - Sesion
Campaña: 
fecha: 
Numero: <% sesionNumber %>
banner: "![[lazy_dm_workbook_banner.jpg]]"
banner_y: 0
fileClass: Sesion
---
# [[Personajes de <% campaña %>]]
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




>[!aside | right clean no-t nmg ]
># 🏘️[[3.Lugares]] importantes
> *Añadir lugares de importancia para la sesión*
> ## [[4.Facciones]] 
>```dataview
>list 
>FROM #NPC AND #relevante 
>```
> [[5.NPCs]]

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

# ⚔️ Encuentros
*Un encuentro puede ser mortal si la suma total de los valores de desafío de los monstruos es superior a la mitad de la suma total de los niveles de los personajes o a un cuarto de os niveles de los personajes si estos son de 4º nivel o inferior.*
`encounter: 1: goblin`
# 💰Tesoro
Ejemplo
# ⏯️Grabación

# 🎥Situaciones probables
*Situaciones probables que vayan a darse durante la sesión.*
## Situacion 1

>[!column | 3 nmg clean txt-c no-i ttl-c] [[4.Facciones]] y [[5.NPCs]]
>>[!note|no-i no-t clean nmg]
>>## ⚔️ Enemigos
>>Enemigo 1
>
>>[!note|no-i no-t clean nmg]
>> ## ✌️Neutrales
>>Neutral 1
>
>>[!note|no-i no-t clean nmg]
>> ## 🛡️Aliados
>>Aliado 1
___
# 📝 Notas