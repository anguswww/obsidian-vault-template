---
categories:
---
Daily notes live in the `Daily Notes` folder and link here automatically. Open today's note with the calendar icon in the left ribbon, or `Cmd/Ctrl`+`P` → "Open today's daily note".

## Notes
```dataview
table dateformat(file.ctime, "dd/MM/yy") as "Created", dateformat(file.mtime, "dd/MM/yy") as "Last Modified"
where contains(categories, this.file.link)
sort file.name DESC
```
