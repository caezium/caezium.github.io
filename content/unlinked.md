```dataview
TABLE without id
out AS "Uncreated files", file.link as "Origin"
FLATTEN file.outlinks as out
WHERE !(out.file) AND !contains(meta(out).path, "/")
SORT out ASC
```

