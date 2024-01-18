```dataviewjs
const {fieldModifier: f} = this.app.plugins.plugins["metadata-menu"].api;

dv.table(["Asentamiento", "Localizacion", "Lideres"],
await Promise.all(dv.pages('"7.Asentamientos"').map(async p => [
	p.file.link,
	await f(dv,p, "location"),
	await f(dv,p, "leaders")])
))
```