
# 1.are cards considered as tasks in trello?

In Trello, **cards are not considered "tasks" in a strict, built-in sense**, but they are commonly **used as task representations**.

Here’s the breakdown:

- **Trello’s official terminology**: Cards are items that represent *anything* you want to track — tasks, ideas, bugs, contacts, leads, etc. Trello does not label them as “tasks” natively.
- **Common usage**: Most people do use cards **as tasks** (e.g., “Write report”, “Call client”, “Fix login bug”).
- **Difference from dedicated task managers**: Unlike apps like Todoist or Asana, Trello has no native “task complete” checkbox on a card (though you can add a checklist inside a card to track subtasks).

**Summary**:  
If you want to treat cards as tasks → yes, that’s fine and very common.  
If you’re asking whether Trello formally defines cards as tasks → no, they are generic “cards.”

trello is like kanban board and you can add tasks, stories and bugs to it but they won't be labeled as any of them and they are just plain text and we don't have such a thing as epic and we have to supply a name next to our title to consider it as epic.

# 2. is trello for kanban framework and not scrum?

That's a great follow-up question. Here's the precise answer:

**Trello is not limited to Kanban** — but it is *best suited* for Kanban and lightweight Scrum. It can support Scrum, but with limitations.

### Breakdown:

| Framework  | Is Trello good for it?                    | Notes                                                                                                               |
| ---------- | ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Kanban** | ✅ Excellent                               | Trello was built around Kanban principles: visual workflow, WIP limits (via lists or plugins), continuous delivery. |
| **Scrum**  | ⚠️ Possible, but not ideal out-of-the-box | Missing native: sprint burndown charts, sprint reports, velocity tracking, defined roles, time tracking.            |

### To use Trello for Scrum, you typically need:

- **Power-Ups** (e.g., Scrum for Trello, Burndown, Reports)
- **Manual tracking** (e.g., due dates for sprint end, labels for story points)
- **Workarounds** (e.g., a list for "Sprint Backlog", another for "Done this sprint")

### Official stance:
- Trello's parent company (Atlassian) positions Trello for **Kanban and general task management**.
- They offer **Jira** for full Scrum (sprints, backlogs, reports, velocity).

### Summary:
- **Kanban** → Trello is perfect.
- **Scrum** → Possible with add-ons, but not native; Jira is better.
- **General rule**: If you need Scrum ceremonies, metrics, and backlog management out-of-the-box, choose Jira or another Scrum-focused tool.

# 3. **Yes, exactly.** In Trello, what most people think of as "columns" are officially called **Lists**.

### Key details:

- **Official name:** Lists
- **Visual layout:** Displayed as vertical columns on your board
- **Purpose:** Organize cards by status, stage, priority, category, etc.

### Common examples of Lists:

- "To Do" → "In Progress" → "Done"
- "Backlog" → "Sprint" → "Review" → "Completed"
- "Idea" → "Working On" → "Test" → "Launched"

### Why "Lists" instead of "Columns"?

Trello was inspired by physical kanban boards (sticky notes on whiteboards) and digital "list" interfaces. The term "list" also works well for:
- **Boards viewed on mobile** (where they may stack vertically rather than show as side-by-side columns)
- **Filtering/focus modes** (e.g., "Show only cards in this list")

### Summary:
| Common term | Trello's official term   |
| ----------- | ------------------------ |
| Column      | **List**                 |
| Row         | *(No direct equivalent)* |
| Card        | **Card**                 |
| Board       | **Board**                |

So if someone says "move this card to the next column," a Trello user would say "move this card to the next **list**."

we can create scrum and sprints in trello by creating a backlog list and `to do`, `in progress` and `done` list to represent our sprint but since we can't specify our issues type and we don't have epics beside there is no automation between backlog and sprint and we don't have access, jira is better option for both scrum and kanban but if you wanted you can use trello for kanban.

# 4. what's board in trello?
A **board** in Trello is the main container that holds **lists** and **cards**. It represents a project or a workflow.

# 5. what's workflow in trello?
In Trello, a **workflow** is the path a card follows from start to finish as it moves across **lists** (e.g., "To Do" → "Doing" → "Done").

It represents your process or set of steps for getting work completed.

# 6. kanban style lists
we may not have the exact same columns or lists in our trello board which we have in kanaban i.e. `to do`, `in progress`, `done` and we may columns like `recipe idea`, `test and refine`, `photo` and `done`, these are same as the lists we have in kanban except different procedures and layers and we may have only task as our issue in our lists but in the kanban bord we have for  website or a product, we use kanban lists i.e. `to do`, `in progress` and `done` and we use story and task combination (I know trello can't specify the type of issue but we can specify ourselves by typing down their type in front of their title, supplying epic name after the name is something optional)

# 7. creating boards in trello
in the bottom bar, select switch boards and create new boards and switch between them and boards are like projects in Jira.

# 8. what's workspace in trello?
In Trello, a **workspace** is a container that holds **boards** and members. It’s used to organize related projects and control team access at a higher level than individual boards.

# 9. do boards represent projects in trello?
**Generally, yes** — but it depends on how you use Trello.

- **Common usage:** Most people use one board per project (e.g., "Website Redesign," "Marketing Q2").
- **Alternative uses:** A board can also represent a **continuous workflow** (e.g., "Customer Support," "Personal To-Dos") or a **department** (e.g., "HR Requests").

So while boards *often* represent projects, Trello doesn't enforce that — you define what a board means for your team.

# 10. should someone use our username when they want to invite us to a board?
**Yes.** To invite you to a board, someone needs your **email address** or your **Trello username**.

- **Email address** – Most common method. Trello sends an invitation email.
- **Trello username** – Can be used if searching for you within Trello's invite system.

They cannot invite you with just your display name (e.g., "John Doe") — they need the unique username (e.g., "@johndoe123") or email.

# 11. attachments in trello
you can add additional info to your cards under attachments, it can be a image or link, even i you add a image in the comments, it will be included in the attachments, for attaching a file or link, click a card and select `attachment`, if you don't see `attachment`, click `+Add` and add `attachment`. 

# 12. flagging a card as finished
you can check the circle next to each card title when you hover over it and it will be labeled as done, it's trello system to display a task is done wherever or any list it's located in it but we can drag and drop our cards into our done list to show it's done and beside that, we can also check that as done.

# 13. what's the application of cover in trello?
In Trello, the **application cover** (or simply **cover**) is an image or color displayed at the top of a **card** to help it stand out visually.

Covers can be:
- A solid **color**
- An uploaded **image** or photo
- An **emoji** (small icon)
- An **attachment** preview (like a Google Drive file or image link)

They are purely visual — they don't affect functionality, just make cards easier to recognize at a glance.

when you add a image as attachment or a comment with image, you can set those images as cover, sometimes after adding them, they get automatically added as cover and sometimes you have to set them manually, for setting a cover select the three dots next to attachment to add at it as cover or click the pencil icon next to card title when you hover over it to change icon.

# 14. sharing the board and workspace
for sharing a board, click the share button in the right side of the screen and add people via their trello username or email address, if they don't have trello account, you can invite them to trello via their email address.

for giving access to the workspace to another people, click the trello icon in the left side of the screen and from the left pane, click members and add them via username or email address.

# 15. what's the application of labels in trello?
In Trello, **labels** are color-coded tags used to **categorize, prioritize, or classify cards** visually.

**Common applications:**

- **Priority** – Red = High, Yellow = Medium, Green = Low
- **Status** – Blue = Blocked, Purple = In Review
- **Type of work** – Bug, Feature, Task, Meeting
- **Department/Team** – Marketing, Dev, Design
- **Custom text** – You can add names to each color (e.g., "Urgent," "Client A")

**Key benefit:** You can **filter boards** to show only cards with specific labels, making it easy to focus on what matters.

for creating labels, click the three dots in the top right of the screen and select labels, for using labels click the card and click labels or hover on the card and click pencil icon and select edit labels. 

# 16. what's the application of checklist in trello?
In Trello, a **checklist** is a list of subtasks inside a card, used to **break down a task into smaller, trackable steps**.

**Common applications:**

- **Task decomposition** – e.g., "Write report" → steps: Research, Draft, Edit, Submit
- **Progress tracking** – Shows a completion percentage bar
- **Quality control** – Ensure all steps are done before closing a card
- **Recurring processes** – e.g., "Daily standup" checklist: Update board, Review blockers, Assign tasks
- **Accountability** – Assign individual checklist items to different members

**Key benefit:** You can see at a glance how much of a card is complete without opening it (percentage shown on the card cover).

checklist is like subtasks in jira, therefore they aren't that useful, for adding checklist 
click the card and select checklist.

# 17. copying a card
for copying a card, just click the card and click three dots in the top right and select copy or hover on the card and click the pencil icon and select copy card.

# 18. for deleting a card, should we first archive it in trello?
**Yes.** In Trello, to permanently delete a card, you must **first archive it**, then delete it from the archive.

**Steps:**
1. Archive the card (moves it out of the board view)
2. Go to the board's menu → **Archived Items** → find the card → select **Delete permanently**

**Why?** This two-step process prevents accidental permanent deletion. Archiving alone is reversible (you can send the card back to any list).

when we are done with a task or card for removing clutter, we archive it and then the cards get removed from the board and then we can delete them, we only delete them when cards were added mistakenly or they contained wrong information.  

for archiving a card click the card and click the three dots in the top right of the screen and select archive or hover on the card and click the pencil icon and select archive.

for checking the arched items, click the three dots in the right side of the page and select archived items, from there you can restore the item back to board or delete it.

In Trello, **archiving** removes cards or lists from your board's main view without deleting them permanently.

**Common applications:**

- **Cleaning up completed work** – Hide finished cards without losing the record
- **Removing clutter** – Keep only active tasks visible
- **Preserving history** – Archived items remain searchable and restorable
- **Ending sprints or projects** – Archive old lists after a project closes
- **Temporary hiding** – Remove something you might need later

**Key benefit:** You can restore archived items at any time. Permanent deletion requires archiving first, then deleting from the archive.

# 19. is watching for changes other people make or it also monitor changes made by myself also? 
In Trello, **watching** (or "subscribing" to a card/board) monitors **changes made by any member** — including yourself.

**What triggers notifications:**
- Other people add, move, edit, or comment
- **You** make changes to that card or board (though you typically won't notify yourself unless your settings allow it)

**Default behavior:**  
Trello usually **does not** send you notifications for changes you make yourself (to avoid clutter). It focuses on activity from **other members**.

**Bottom line:** Watching watches all activity, but you generally only hear about *others'* changes — not your own.

we watch a card when another member except than us made a change or modification in the card, we get notified like making a comment or changing the due date and we get notified by them in notification section which is the bell icon located in the top right of the screen.

for watching a card, select a card and click the eye icon in the top right of the screen and for stopping watching a card, again click the same eye icon.

# 20. what's application of join when we can make changes to a card even we're not a member of it?
Great observation. You're right — in Trello, **you can sometimes make changes to a card even if you're not a member of that specific card**. However, being a **member of the board** is what usually gives you that access.

Here's where **"Join"** (adding yourself as a card member) becomes useful:

### What "Join" does:
It adds you as a **member of that specific card**, not the whole board.

### Why use "Join" if you already can edit the card?
Even if you can edit the card as a board member, joining gives you:

1. **Notifications** – You'll be alerted to changes on that card (without joining, you may not be)
2. **Assignment visibility** – Others can see you're responsible for or following that card
3. **Filtering** – You can filter boards to show only cards where you're a member
4. **Personal organization** – Marks the card as relevant to you

### Key distinction:

| Access level                   | Can edit card?  | Gets notifications? | Shows as assigned? |
| ------------------------------ | --------------- | ------------------- | ------------------ |
| Board member (not card member) | ✅ Yes (usually) | ❌ No                | ❌ No               |
| Card member ("Joined")         | ✅ Yes           | ✅ Yes               | ✅ Yes              |

### Bottom line:
You don't need to "Join" to edit — but you **join to track, get notified, and show ownership** of that specific card.

# 21. you say joining allows us to get notified if any change occurs in the card, so what's the difference of that with watching?
**Joining** = You are a **member** of the card. Notifications are automatic for changes (by anyone).

**Watching** = You are **not necessarily a member**. You manually choose to follow the card's activity.

**Key difference:** Joining implies responsibility/assignment. Watching is just following without being assigned.

joining is useless.

for joining a card click a card and click the three dots and select `join` and for leaving the card, select the same three dots in a card and select `leave`.

# 22. changing background and adding stickers
for changing background, select the three dots in the screen and click `change background`, for adding a sticker to a card, click the same three dots and select `stickers` and drag the sticker you want to the specific card and drop it there, you can also add custom images as stickers and backgrounds.

# 23. what's the difference between any match and exact match in filtering?
In Trello's **filtering** (search or card filter):

- **Any match** – Shows cards that contain **at least one** of your search terms (OR logic).
- **Exact match** – Shows cards that contain **the exact phrase** you typed, in that order (AND logic for the sequence).

**Example** – Searching `bug fix`:
- **Any match** → Cards with "bug" **or** "fix" (or both)
- **Exact match** → Cards with the phrase `"bug fix"` exactly (not "fix bug" or just "bug")

for filtering your cards, you click the funnel icon (3 horizontal lines beneath each other) in the right side of the screen , any match will check for situation that any of the conditions may happens not all conditions with each other, for situation that all condition that we want to check for all selected conditions at once, we select exact match, in reality any match is like exact match but for more safety always set on the exact match when you're filtering because when we select multiple conditions, we want them all together.

# 24. comments section option
we have markdown options in the comment section, after creating bullets and numeric list, if we press `tab`, we create a subset and if we press `enter`, we create a superset.

we can even tag other people to notify them about comment, for using it press the `+` sign and click `mention`.

# 25. leaving a board
for leaving a board, click three dot in the screen and select leave.

# 26. public and private workspace and how to make public boards via public workspace
for toggling between private and public workspace, click the trello logo in the top left, click the `setting` from workspace section and from workspace visibility section, you can change your workspace to private or public, public workspace can be indexed by google and search engines but people need permission to change in the boards, for making a board public, you need premium subscription of trello but there is a workaround to have public boards in free version of trello and that's to make a workspace public, subsequently the boards get public also. 

# 27. highlighting a board
in the top right of the screen, there is a star icon, by clicking that you make your board highlighted, if you want to make other boards highlighted also, click the trello icon and in the screen, you see your boards, on the top right of the boards you see a star icon, by clicking that, you make your board highlighted.

# 28. finding which cards are assigned to me
you can use filters to see what tasks are assigned to you, you can click the your name icon in the top right and click cards to see what cards are assigned to you.

# 29. copying a checklist
you can select a card and drag all of the checklist items and press `ctrl+c` it and paste it wherever you like it by pressing `ctrl+v`.

another approach is to when we want to make a checklist, to choose a card from 
`copy items from` section and select a card to copy its checklist.

another approach is to copy a card and select to only copy its checklist.
# 30. another approach of copying a card
you can click a card and press `ctrl+c` and hover over a list and press `ctrl+v`.

# 31. relating two cards to each other
we copy URL of a card and copy it in a comment for mentioning that card, another approach is to click attachment and paste link of that card or search for name of that card to look for it and and attach that card, a relation can be bi-directional, after attaching a card in another card, click the three dots below it and select `relate both cards` and the card we are in it right now will appear in the card we had related to our current card attachment.

# 32. what's power ups in trello?
In Trello, **Power-Ups** are integrations or add-ons that extend a board's functionality beyond the basic features.

**Common applications:**

- **Calendar view** – See cards with due dates on a timeline (like Google Calendar)
- **Slack integration** – Receive Trello notifications or create cards from Slack
- **Jira integration** – Link Trello cards to Jira issues
- **Custom fields** – Add dropdowns, numbers, dates, or text fields to cards
- **Automation (Butler)** – Create rules, buttons, and scheduled commands (e.g., "move card after 7 days")
- **Voting, time tracking, reports** – Depending on the Power-Up

**Key details:**

- Free boards get **1 Power-Up** per board
- Paid plans unlock **unlimited Power-Ups** per board

**Bottom line:** Power-Ups let you turn Trello into a calendar, CRM, support desk, or custom workflow tool.

we have a power-up for calendar which its name is calendar power-up and a calendar icon appears in the top right of the screen and it's like calendar in jira which changing due date and start date in the calendar causes the start date and due date of that card changes and if you change the due date and start date in the card, the calendar interface will change also.

# 33. linking two boards
we copy a board URL and attach it as attachment or use the link in the comment and we don't have bi directional relation for boards relation in a card like card relations.

# 34. shortcuts for trello
for applying shortcuts just click the key and there is no need to press `ctrl` or any key simultaneously.

b -> boards
f --> filter
`ctrl+c` a card and clicking on a card makes the copied card related to clicked card
x-> removing filter
q -> filter cards to cards that are assigned to you

shortcuts when a card is clicked:
space -> add yourself to a card i.e. join a card
d -> due date
l -> opens label section
numbers -> adding labels

# 35. some other useful power-ups
**1.pin card**
pins a cards and can't be moved in a list and can't be moved to another list and it's always placed at the top of its list.

**2.voting**
enables voting options for a card, it's useful when we have lots of cards and we want to see what other members think about completion of cards and which one is more popular to be completed.

# 36. useful google chrome extensions for trello

**trello card numbers plus**
it gives card a unique number that when we want to refer to a card, we can use that number, beside that it displays number of existing cards in a list.



