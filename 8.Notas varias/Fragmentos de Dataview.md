## Seleccionar opciones de las properties de otra notas (NPCs Rangos de Facciones)
[...new Set(dv.pages('#Faccion')
.where(p=>{
    if(!p.file.path.contains("z_Templates")&& p && p.Rangos){
        if(Array.isArray(current.Facciones.path)){
            return p && current.Facciones.map(link => link.path).includes(p.file.path) 
        }else{
            if(current.Facciones.path === p.file.path){
                console.log(p)
                return p
            } 
        }
    }   
})
.map(p=> p.Rangos).values)
].flat()


```dataviewjs
dv.paragraph([...new Set(dv.pages("#Lugar").where(q =>!q.file.path.contains("z_") && q.Religion && Array.isArray(q.Religion)).values.flatMap(q =>" [[" + q.file.name+"]] "))])

```

 dv.paragraph([...new Set(dv.pages("#Lugar").where(q =>!q.file.path.contains("z_") && q.Religion && Array.isArray(q.Religion)&& q.Religion.map(x=>x.path).contains(p.file.path)).values.flatMap(z =>z.file.link))])