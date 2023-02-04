# {{DATE:dddd}}
[[Home]] | [[Next Actions]] | [[Waiting For]] | [[Someday Maybe]]
## Journal

## Tasks Planned Today
Note: This query utilizes the Templater plugin to create the date parameters based on the note title. This assumes the Daily Note title format is set to `YYY-MM-DD`. The benefit of this method is to allow you to create a particular day's note on any other day and still generate a valid query for that note's day.
```tasks
(due before <% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>) OR (scheduled before <% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>)
not done
path does not include Reminders
group by priority
```
***
## Today's Reminders
```tasks
(due before <% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>) OR (scheduled before <% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>)
not done
path includes Reminders
```
***
## Daily Review
Do this at the end of the day 
- [ ] Empty inboxes
	- [ ] Work email
	- [ ] Personal Email
	- [ ] Obsidian Inbox folder
- [ ] Review tomorrow's calendar
	- [ ] Personal
	- [ ] Work
- [ ] Review open projects
- [ ] Review next actions
- [ ] Review tomorrow's daily note and prioritize tasks

***
## Tasks Completed Today
```tasks
done <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD") %>
hide due date
hide recurrence rule
hide done date
heading does not include Daily Routine
heading does not include Daily Review
```