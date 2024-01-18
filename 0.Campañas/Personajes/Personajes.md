---
tags: favoritos
cssClasses: card-images
---
>[!cards| dataview 6]
>```dataview
>table without id embed(link(icon)) as Icono,
>"**"+file.link +"**",
>"**P.Pasiva: "+P_per+"**",
>"**AC: "+ac+"**",
>"**Max HP: "+hp+"**"
>FROM #personaje
>WHERE contains(En_curso, "si")
>```

```dataview
table without id embed(link(icon)) as Icono, file.link as PJ, P_per, ac as AC, Competencias, level
FROM #personaje
WHERE contains(En_curso, "si")
```
