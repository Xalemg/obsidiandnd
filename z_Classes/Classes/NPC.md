---
limit: 20
mapWithTag: true
icon: user
tagNames:
  - NPC
filesPaths: 
bookmarksGroups: 
excludes: 
extends: Global
savedViews: []
favoriteView: 
version: "2.84"
fieldsOrder:
  - zaqQrh
  - rhDWuR
  - ymM71F
  - C1P73m
  - OdTSrV
  - LjKzzu
  - STWFSD
  - 2wfaS0
  - rWLO7B
  - u26Wpx
  - 61Cg3p
  - OzE059
  - 0iEJpI
  - gbYp8V
  - drBJhI
fields:
  - name: icon
    type: Media
    options:
      folders:
        - z_Assets/NPCs
      embed: true
    path: ""
    id: drBJhI
  - name: Ubicacion
    type: File
    options:
      dvQueryString: dv.pages("#Lugar")
    path: ""
    id: gbYp8V
  - name: Religiones
    type: File
    options:
      dvQueryString: dv.pages("#Deidad")
    path: ""
    id: 0iEJpI
  - name: Estado
    type: Select
    options:
      valuesList:
        "1": Vivo
        "2": Muerto
        "3": Otro
      sourceType: ValuesList
      valuesListNotePath: ""
      valuesFromDVQuery: ""
    path: ""
    id: OzE059
  - name: Alineamiento
    type: Select
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Alineamiento.md
      valuesFromDVQuery: ""
    path: ""
    id: 61Cg3p
  - name: Sexo
    type: Select
    options:
      valuesList:
        "1": Hombre
        "2": Mujer
        "3": Otro
      sourceType: ValuesList
      valuesListNotePath: ""
      valuesFromDVQuery: ""
    path: ""
    id: u26Wpx
  - name: Raza
    type: Select
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Razas.md
      valuesFromDVQuery: ""
    path: ""
    id: rWLO7B
  - name: Facciones
    type: File
    options:
      dvQueryString: dv.pages("#Faccion")
    path: ""
    id: 2wfaS0
  - name: Edad
    type: Input
    options: {}
    path: ""
    id: STWFSD
  - name: Oficios
    type: Multi
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Oficios.md
      valuesFromDVQuery: ""
    path: ""
    id: LjKzzu
  - name: Ideal
    type: Input
    options: {}
    path: ""
    id: OdTSrV
  - name: Vinculo
    type: Input
    options: {}
    path: ""
    id: C1P73m
  - name: Defecto
    type: Input
    options: {}
    path: ""
    id: ymM71F
  - name: Interpretacion
    type: Input
    options: {}
    path: ""
    id: rhDWuR
  - name: Rango
    type: Multi
    options:
      valuesList: {}
      sourceType: ValuesFromDVQuery
      valuesListNotePath: ""
      valuesFromDVQuery: |-
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
    path: ""
    id: zaqQrh
---
