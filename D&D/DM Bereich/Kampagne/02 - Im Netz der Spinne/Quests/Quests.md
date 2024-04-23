# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Quest", Belohnung, Questgeber

FROM "DM Bereich/Kampagne/02 - Im Netz der Spinne/Quests" AND #Quest

WHERE Erledigt = false

SORT file.name
```