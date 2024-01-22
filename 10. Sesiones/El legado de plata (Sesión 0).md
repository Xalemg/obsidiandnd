---
Tipo: Sesion
tags:
  - Sesion
fecha: 
Numero: "0"
fileClass: Sesion
Mundo:
  - Aretries
Campañas: El legado de plata
cssclasses:
  - card-images
---
# [[Personajes]]
>[!cards| dataview 7]
```dataview
table without id embed(link(icon)) as Icono, file.link as PJ, P_per as "P.Per", ac as AC, Competencias, level
FROM #personaje
WHERE contains(En_curso, "si") and contains(Campaña, this.Campañas)
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