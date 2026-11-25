---
categories:
---
## Notes
```dataview
table dateformat(file.ctime, "dd/MM/yy") as "Created", dateformat(file.mtime, "dd/MM/yy") as "Last Modified"
where contains(categories, this.file.link)
sort file.mtime DESC
```
