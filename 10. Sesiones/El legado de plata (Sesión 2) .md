---
banner: 
banner_y: 0.304
fileClass: Sesion
Mundo:
  - Aretries
cssclasses: 
Campaña:
  - El legado de plata
Numero: 2
tags:
  - Sesion
fc-date: 0783-01-10
---
# [[Personajes]]
>[!cards | dataview 7]
>```dataview
>table without id embed(link(icon)) as Icono,
>"**"+file.link +"**",
>"**P.Pasiva: "+P_per+"**",
>"**AC: "+ac+"**",
>"**Max HP: "+hp+"**"
>FROM #personaje 
>WHERE contains(En_curso, "si") and contains(Campañas, string(this.Campaña))
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
- [ ] La [[Familia de Norias]] es la principal aliada de la [[Corona de Altalos]] 
- [x] [[Lisa]] es una dragona 
- [ ] [[Gath Igeo]] esta en [[Hismal]]
- [x] [[Gath Igeo]] proviene del tramontes, es el nombre que los humanos pusieron a la familia élfica se ha traducido como jinetes de dragón aunque vinculados a los dragones seria un nombre más apropiado.
- [x] [[La escama plateada]] era una de las ordenes de Gath Igeo encargadas de la recopilación de información
- [ ] La tribu de [[Gath Igeo]] esta compuesta por cinco ordenes, cada una encargada de distintas 
- [ ] La mayoria de los miembros de [[La escama plateada]] no conocen a [[Lisa|Lysandryth (Nombre de Dragon)]] 
- [ ] Lisa Recibió un mensaje de su padre que si queria abandonar a los humanos al norte de las [[Islas Shamal]] se encontraba el ombligo elemental
- [ ] [[Cueva del regalo#📜 Historia| Historia de la cueva del regalo]]
- [ ] 
- [ ] 
- [ ] 

# 🎥Situaciones probables
*Situaciones probables que vayan a darse durante la sesión.*
## Charlita con [[Lisa]]
- [ ] ¿Solo sabes luchar corriendo? Esperaba poder ver una demostración mas impresionante de tus habilidades.
- [ ] ¿Sabes quien soy?
- [ ] Mañana tienes otra prueba, una prueba para demostrar que estas preparada. Iras acompañada. Debes acabar el trabajo de otro. Un hace su nido en la cuna de la montaña. Un dia los elfos de [[Gath Igeo]] habitaron una vez. Busca la historia de tu pueblo alli. Demuestra que eres capaz de acabar con nuestros enemigos. Entonces sabre que estas lista.
- [ ] [[Hansel]] te dejara en los pies de la montaña y te recogerá en el mismo lugar. Encuentra la cueva y acaba con el dragón blanco que allí mora. Buena suerte.
- [ ] Te dejara una nueva piedra mensajera 100 po
## Preparativos pre aventura
¿Qué necesitas? ¿Necesitas comprar algo?
## La llegada al campamento abandonado
Tiendas abandonadas.
# ⚔️ Encuentros
*Un encuentro puede ser mortal si la suma total de los valores de desafío de los monstruos es superior a la mitad de la suma total de los niveles de los personajes o a un cuarto de os niveles de los personajes si estos son de 4º nivel o inferior.*
`encounter: 1: goblin`
# 💰Tesoro
Ejemplo
# ⏯️Grabación


# 📝 Notas
Lagrima del invierno margarita violeta de grandes alturas