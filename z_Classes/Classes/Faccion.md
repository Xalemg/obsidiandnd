---
limit: 20
mapWithTag: false
icon: users
tagNames: 
filesPaths: 
bookmarksGroups: 
excludes: 
extends: Global
savedViews: []
favoriteView: 
version: "2.23"
fields:
  - name: aliases
    type: Input
    options: {}
    path: ""
    id: lIxh9f
  - name: icon
    type: Media
    options:
      folders:
        - 
        - z_Assets/Arte
        - 
        - z_Assets/Emblemas
      embed: true
    path: ""
    id: ddztZn
  - name: Mundo
    type: Input
    options: {}
    path: ""
    id: t1r309
  - name: Influencia
    type: Select
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Influencia.md
      valuesFromDVQuery: ""
    path: ""
    id: 65vnyr
  - name: Alineamiento
    type: Select
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Alineamiento.md
      valuesFromDVQuery: ""
    path: ""
    id: AhAqkH
  - name: Tipo
    type: Select
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Tipo de Gobierno.md
      valuesFromDVQuery: ""
    path: ""
    id: R9hlrd
  - name: Ubicacion
    type: File
    options:
      dvQueryString: dv.pages("#Lugar")
    path: ""
    id: gFsL0G
  - name: Rangos
    type: Multi
    options:
      "1": Rey (Lider)
      "2": Caballeros
      "3": Reina
      "4": Lider
      "5": Padre
      "6": Padre
      "7": Padre(Lider)
      "8": Hija menor
    path: ""
    id: s7c817
  - name: Lider
    type: File
    options:
      dvQueryString: dv.pages('#NPC').where(n=>!n.file.path.contains("z_"))
    path: ""
    id: 5B8076
fieldsOrder:
  - 5B8076
  - s7c817
  - gFsL0G
  - R9hlrd
  - AhAqkH
  - 65vnyr
  - t1r309
  - ddztZn
  - lIxh9f
---
