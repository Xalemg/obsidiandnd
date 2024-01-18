---
limit: 20
mapWithTag: false
icon: mountain
tagNames: 
filesPaths: 
bookmarksGroups: 
excludes: 
extends: Global
savedViews: []
favoriteView: 
version: "2.66"
fields:
  - name: Poblacion
    type: Input
    options: {}
    path: ""
    id: YiQNh3
  - name: Tipo
    type: Select
    options:
      valuesList:
        "1": Plano
        "2": Continente
        "3": Subcontinente
        "4": Reino
        "5": Region
        "6": Ciudad
        "7": Pueblo
        "8": Mazmorra
        "9": Punto de Interes
        "10": Servicio
      sourceType: ValuesList
      valuesListNotePath: ""
      valuesFromDVQuery: ""
    path: ""
    id: rjXphZ
  - name: Prosperidad
    type: Select
    options:
      valuesList:
        "1": Muy Alto
        "2": Alto
        "3": Medio
        "4": Bajo
        "5": Muy Bajo
        "6": Pauperrimo
      sourceType: ValuesList
      valuesListNotePath: ""
      valuesFromDVQuery: ""
    path: ""
    id: tn42Wf
  - name: Ubicacion
    type: File
    options:
      dvQueryString: dv.pages("#Lugar")
    path: ""
    id: dtB3td
    command:
      id: insert__Asentamiento__Ubicacion
      icon: list-plus
      label: Insert Ubicacion field
  - name: icon
    type: Media
    options:
      folders: []
      embed: true
      display: list
    path: ""
    id: 20MWhN
  - name: Tematica
    type: Multi
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Tematica.md
      valuesFromDVQuery: ""
    path: ""
    id: Jik8kn
  - name: Terreno
    type: Multi
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Terrenos.md
      valuesFromDVQuery: ""
    path: ""
    id: dhMgdN
fieldsOrder:
  - dhMgdN
  - Jik8kn
  - 20MWhN
  - dtB3td
  - tn42Wf
  - rjXphZ
  - YiQNh3
---
