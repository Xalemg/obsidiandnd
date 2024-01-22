---
fields:
  - name: NPCs Relevantres
    type: Lookup
    options:
      autoUpdate: false
      outputType: LinksList
      builtinSummarizingFunction: Count
      customListFunction: page.file.name
      customSummarizingFunction: return pages.length
      dvQueryString: dv.pages('#NPC' && '#Relevante')
    path: ""
    id: U8n5UG
version: "2.5"
limit: 20
mapWithTag: true
icon: scroll
tagNames:
  - Sesion
filesPaths: 
bookmarksGroups: 
excludes: 
extends: Global
savedViews: []
favoriteView: 
fieldsOrder:
  - U8n5UG
---
