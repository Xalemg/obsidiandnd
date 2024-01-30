---
Tipo: Sesion
tags:
  - Sesion
fecha: 2024-01-25
Numero: "0"
fileClass: Sesion
Mundo:
  - Aretries
Campaña: El legado de plata
cssclasses:
  - card-images
  - t-w
numero: 1
---
# [[Personajes]]
>[!cards| dataview 7]
```dataview
table without id embed(link(icon)) as Icono, file.link as PJ, P_per as "P.Per", ac as AC, Competencias, level
FROM #personaje
WHERE contains(En_curso, "si") and contains(Campaña, this.Campaña)
```

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
- [ ]  Gath Igeo se encuentra en Hismal
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
## Recap de lo ocurrido
- [ ] Lo ocurrido al final de la ultima aventura
- [ ] [[Elentari]] se desmaya, necesita días para recuperarse.
- [ ] [[Anvil Carrillo]] os contacta, esta interesado en saber como estáis y que ha pasado
- [ ] Al poco tiempo un mago llamado [[Hansel]] se presentan en [[Kalithir]] y les dice que [[Anvil Carrillo]] les espera. Les llevara a [[Puerto Kalabor]] donde os presentaran frente a la asamblea de [[La Mancomunidad del Viento]] donde os preguntan que sabéis sobre la desaparición del sol de [[Amaunator]] y sobre vuestras peripecias en [[Ust Natha]].
- [ ] Viaje a [[Puerto Kalabor]] para comparecer frente al consejo [[La Mancomunidad del Viento]] y todos los dirigentes de las naciones que las componen. Os cuestionaran sobe lo sucedido en [[Ust Natha]] y sobre el sol desaparecido.
- [ ] [[Hansel]] te separara del resto de la party y te dirá que alguien tiene algo información importante que hablar contigo acerca de su futuro
## Comienzo en [[Crestafria]]

# ⚔️ Encuentros
*Un encuentro puede ser mortal si la suma total de los valores de desafío de los monstruos es superior a la mitad de la suma total de los niveles de los personajes o a un cuarto de os niveles de los personajes si estos son de 4º nivel o inferior.*

`encounter: 1: goblin`
# 💰Tesoro
Ejemplo
# ⏯️Grabación


# 📝 Notas