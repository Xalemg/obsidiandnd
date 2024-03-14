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

  **Facciones**:
  ```dataviewjs
  [... new Set(dv.pages('#Faccion').where(p =>{if(Array.isArray(p.Ubicacion)){ return p.file.link && p.Ubicacion.map(link => link.path).includes(this.currentFilePath)}else{if (p.Ubicacion!=null && this.currentFilePath.contains(p.Ubicacion.path)) {return p}}}).map(p =>p.file.link +"(Influencia "+p.Influencia+")<BR/>"))].join ('') 
  ```
```dataviewjs
dv.paragraph([...new Set(dv.pages("#Lugar").where(q =>!q.file.path.contains("z_") && q.Religion && Array.isArray(q.Religion)).values.flatMap(q =>" [[" + q.file.name+"]] "))])

```

 dv.paragraph([...new Set(dv.pages("#Lugar").where(q =>!q.file.path.contains("z_") && q.Religion && Array.isArray(q.Religion)&& q.Religion.map(x=>x.path).contains(p.file.path)).values.flatMap(z =>z.file.link))])