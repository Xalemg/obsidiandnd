---
<%*

const dv = app.plugins.plugins.dataview.api;
let pages = dv.pages("#sesion");
const campaña = await tp.system.suggester(["El desencadenamiento", "El desencadenamiento, El legado de plata (Kiera)"], ["El desencadenamiento","El desencadenamiento, El legado de plata (Kiera)"]);
let sesionNumber =0;
const filterSessions = (session, campaña)=>{
    if( session.Campaña==campaña){ 
	        return true;
    }
}
let sesionesCampaña = pages.file.frontmatter.where(t => filterSessions(t, campaña)).values;
console.log(sesionesCampaña);
sesionNumber =sesionesCampaña.reduce((sesionNumber, sesion)=> {
console.log(sesion);
if(sesionNumber>sesion.Numero){
return "" + sesionNumber;
}
else{
return  parseInt(sesion.Numero)+1
}
},0);
//Math.max.apply(null, sesionNumber);
sesionNumber = await tp.system.prompt("Numero de la sesión","" + sesionNumber, "");
console.log(sesionNumber);
const date = await tp.system.prompt("Fecha proxima sesion", tp.date.now("YYYY-MM-DD"), "");
const title = "Sesión " + sesionNumber+ " " + campaña + "( " + date + ")";
await tp.file.rename(title);


_%>
Tipo: Sesion
Tags: Sesion
Campaña: <% campaña %>
fecha: <% date %>
Numero: <% sesionNumber %>
banner: "![[lazy_dm_workbook_banner.jpg]]"
banner_y: 0
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
>WHERE contains(En_curso, "si") AND contains(Campaña, <% campaña %>)
>```




>[!aside | right clean no-t nmg ]
># 🏘️[[3.Lugares]] importantes
> *Añadir lugares de importancia para la sesión*
># ⚔️ Encuentros
>*Un encuentro puede ser mortal si la suma total de los valores de desafío de los monstruos es superior a la mitad de la suma total de los niveles de los personajes o a un cuarto de los niveles de los personajes si estos son de 4º nivel o inferior.*
>`encounter: 1: goblin`
># 💰Tesoro
>ejemplo
># ⏯️Grabación


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