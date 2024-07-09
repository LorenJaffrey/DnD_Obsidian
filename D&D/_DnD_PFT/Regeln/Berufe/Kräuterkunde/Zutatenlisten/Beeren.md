# `=this.file.name`
```dataview
TABLE WITHOUT ID
file.link AS "Kräuterkundezutat",
join(file.frontmatter.Umgebungen) AS "Umgebungen"
FROM #Beruf/Kräuterkunde/Zutat
WHERE Art = this.file.link
SORT file.name
```