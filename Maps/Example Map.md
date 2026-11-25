---
categories:
---
This is a map: an ordinary note that acts as a home page for a topic. Any note with `[[Example Map]]` in its `categories` property shows up in the table below. Rename or duplicate this note to make your own maps — new notes created in `Maps/` get this layout automatically.

## Notes
```dataview
table dateformat(file.ctime, "dd/MM/yy") as "Created", dateformat(file.mtime, "dd/MM/yy") as "Last Modified"
where contains(categories, this.file.link)
sort file.mtime DESC
```

