---
cssClasses: card-images
---



> [!cards|5 ]
 **[[0.Campañas| Campañas]]**
> ![[SessionNotes.png]]
>
> **[[Grupos de aventureros]]**
> ![[Parties.png]]
> 
> **[[Personajes]]**
> ![[Players.png]]
> 
> **[[2.Panteón| Dioses]]**
> ![[Deities.png]]
> 
> **[[5.NPCs| NPCs]]**
> ![[NPCs.png]]
> 
> **[[4.Facciones| Facciones]]**
> ![[Groups.png]]
> 
> **[[3.Lugares| Lugares]]**
> ![[Landmarks.png]]
>
> **[[6.Literatura|Literatura]]**
> ![[Literature.png]]
> 
> **[[7.Pantalla del Master| Pantalla del Master]]**
> ![[Quests.png]]
> 
> **[[8.Notas varias]]**
> ![[RandomNotes.png]]

> [!tip |nmg txt-c ttl-c n-th] 
> `dice: [[Tabla de consejos#^randomTip]]|Tip` 

>[!column | 3 no-t nmg clean]
>>[!note|no-i no-t clean nmg]
>>### 📂Actualizado recientemente
>>`$=dv.span(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(10).file.link)`
>
>>[!note|  no-i no-t clean nmg] 
>>### 🔖Favoritos 
>>`$=dv.span(dv.pages('#favoritos').file.link.sort())` 
>
>>[!note|no-t no-i nmg clean] 
>>### 🗓️ Futuras y ultimas sesiones
>> `$=dv.span(dv.pages('#sesion').sort(f=>f.fecha,"desc").limit(10).file.link)`

## Para hacer
> [!column|2 no-title]
>> [!metadata] Short Term
>> - [x] Actualizar las notas de la [[Chumipower]] 
>> - [ ] Migrar las notas de la otra boveda
>> - [ ] 
>
>> [!metadata] Long Term
>
>

## Notas aleatorias
> [!cards|dataview 5 cover] **Party**
>```dataview
> TABLE WITHOUT ID
> embed(link( icon  )) as Art,
> "**"+ file.link + "**" AS "Column Name"
> WHERE (contains(Tipo, "jugador") OR contains(tags, "NPC") OR  contains(tags, "Lore") OR  contains(tags, "Deidad") OR contains(tags, "Faccion") OR contains(tags, "Lugar") ) AND !contains(file.folder, "z_Templates")
FLATTEN [ [(seed) => (seed * 1103515245 + 12345) % 2147483648]] AS random
FLATTEN [number(dateformat(date("now"), "x"))] AS seed
SORT random[0](seed + file.size)
LIMIT 10

