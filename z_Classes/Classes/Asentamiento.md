---
limit: 20
mapWithTag: false
icon: tent
tagNames: 
filesPaths: 
bookmarksGroups: 
excludes: 
extends: Lugar
savedViews: []
favoriteView: 
fieldsOrder:
  - gvGjWJ
  - MqSamn
  - 5Jch3p
version: "2.10"
fields:
  - name: Gobierno
    type: Select
    options:
      valuesList: {}
      sourceType: ValuesListNotePath
      valuesListNotePath: z_Classes/Options/Tipo de Gobierno.md
      valuesFromDVQuery: ""
    path: ""
    id: 5Jch3p
  - name: Defensas
    type: Input
    options: {}
    path: ""
    id: MqSamn
  - name: Religion
    type: File
    options:
      dvQueryString: dv.pages('#Deidad')
    path: ""
    id: gvGjWJ
---
