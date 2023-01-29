*Command + T for today's note*
**Quick Lists:** [[Next Actions]] | [[Waiting For]] | [[Someday Maybe]]
**Tasks & Reminders:** [[Personal Reminders]] | [[Home Chef Tasks]] | [[Digital Gardening Tasks]] | [[Context Lists]]
   
## Home Chef Projects
```button
name New Project
type note(New Project, split) template
action Project Template
```
``` dataview
	TABLE type, owner
	FROM "Projects"
	WHERE area="Home Chef"
	SORT type descending
```
## Personal Projects
```dataview
	LIST
	FROM "Projects"
	WHERE type="Project" AND area="Personal"
```

## SJCS Projects
```dataview
	LIST
	FROM "Projects"
	WHERE type="Project" AND area="SJCS"
```

## Legend
- **People** are notes that begin with a `@` and are stored in /Reference/People
