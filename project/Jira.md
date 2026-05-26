
# 1. what's issue or work item in Jira?

In Jira, an **issue** is the basic unit of work—a record that tracks a task, bug, story, or epic.

A **work item** is essentially the same thing. The term is often used in team-managed projects to refer to actionable issues like stories, tasks, bugs and epics

# 2. what's board in Jira ?

A **board** in Jira is a visual tool that displays a set of issues (work items) and tracks their progress through a workflow.

There are two main types:

- **Scrum board** – organizes work into sprints; used for teams working in time-boxed iterations.
- **Kanban board** – focuses on continuous flow; limits work in progress without sprints.

Boards help teams see what’s *to do*, *in progress*, and *done* at a glance.

# 3. what's workflow in jira?

A **workflow** in Jira is the set of statuses and transitions that an issue moves through from start to finish.

- **Statuses** represent where an issue is in the process (e.g., *To Do*, *In Progress*, *Done*).
- **Transitions** are the actions that move an issue between statuses (e.g., *Start Progress*, *Resolve*, *Close*).

Workflows ensure issues follow a consistent process and can include rules like approvals or required fields.

# 4. what's projects in jira?

A **project** in Jira is a container that groups related issues (work items) together.

Key points:
- It acts as a **central hub** for a team, product, or initiative.
- Each project has its own **issues**, **board**, **workflow**, and **permissions**.
- Projects can be **company-managed** (more configurable) or **team-managed** (simpler, team-controlled).

In short, a project is where all the work for a specific effort lives.

# 5. what are differences between company managed and team managed projects?

Here are the key differences:

| Aspect          | **Company-Managed**                                    | **Team-Managed**                            |
| --------------- | ------------------------------------------------------ | ------------------------------------------- |
| **Control**     | Managed by Jira admins; centralized configuration      | Managed by the team; no admin required      |
| **Workflow**    | Fully customizable; can be complex with global sharing | Simplified; team edits their own workflow   |
| **Issue types** | Shared across projects; can add custom types           | Simplified set; team controls their own     |
| **Permissions** | Granular, permission scheme-based                      | Simpler; role-based (Admin, Member, Viewer) |
| **Board**       | Separate from project settings; highly configurable    | Built-in; tied directly to the project      |
| **Best for**    | Large organizations, standardized processes            | Small teams, autonomy, simplicity           |

**Summary:** Company-managed offers more power and control but requires admin oversight. Team-managed is simpler and gives teams independence.

# 6. Creating issues in Excel

we should create our epics, stories and tasks with each story impact, effort, points and then prioritize them with function and RICE formula, this is because we are not able to prioritize our stories with Jira that properly and we have more access in Excel while we can create epics, stories and tasks in Jira and share it so other team members can see it but prioritization is not possible in the way I want so I think Excel is a better option for doing such tasks and we just share stories and epics and tasks in Jira so other team member can see it.

we should have a bug list and worksheet in Excel to prioritize them or I think it's better to consider bugs as an epic and each bug is like a story and then we define tasks for each bug but I think bug should be in the separate spreadsheet since it doesn't get refined at end of each quarter and w have it as a list which everything gets added to it.

we can have a excel sheet for each quarter which has a spread sheet for bugs and one for resolved bugs, then one for epics and stories and one for done stories and a spreadsheet for sprints.

# 7. creating custom issue or work item

choose your space, click ellipses or three dot next to space name (more action), navigate to 
space setting -> work types -> Add work type

we can create custom issues like front-end task or back-end task but it's kind of fancy thing to do, stick to default issue types.  

# 8. Key in jira

key are a prefix in our work items to show which space they belong to, so choose them as descriptive as it should be.

# 9. how to add work item?

navigate to backlog->backlog-> select create or
select the global create button next to search bar

# 10. team managed projects superiority over company-managed projects

always use team managed project while creating your projects because it's more straight forward and has less bullshit things comparing to company based projects

# 11. how to check which project type, team managed or company managed

from the left pane and three dots next to spaces section, select manage spaces and you can see each space or project is either team managed or company managed.

# 12.difference between scrum and kanban backlog
in Kanban backlog there is no epic, which is no worries and we just add our stories but in our excel backlog we will have epic for our kanban framework.

# 13. epic in kanban
there is no feature like scrum backlog to create epics in kanban, I can create a custom issue or work item as epic and then sort its correspondent stories beneath it and then its tasks but you can skip adding epics and just add stories, if you add epics it helps for clarification but also it may make confusion, so you have epics in Excel, and sort stories and tasks based on them and just add stories in kanban and tasks in the backlog of it and we have everything sorted in my Excel sheet.

I just realized you can add epic in kanban also, by hovering over issue in backlog, an `+ Epic` sign appears, if you have created an epic and doesn't allow you to create another one, just click one of the already created epics and then select add parent and add the epic.

you can also create epic from the global create button next to search bar.

# 14. description of a issue

we have a summary for our issues and a description, summay is the title, in story description, we can add its acceptance criteria and the summary is like `as a guest I want to have these to resolve this` and for tasks summary we have `add gateway API` and description can be more info about how to implement API.

# 15. what's the difference between status and workflow in jira?

Here's the difference:

---

| Aspect         | **Status**                                                       | **Workflow**                                           |
| -------------- | ---------------------------------------------------------------- | ------------------------------------------------------ |
| **Definition** | A single state that indicates where an issue is in its lifecycle | A set of statuses and the transitions between them     |
| **Purpose**    | Shows current progress (e.g., "In Progress")                     | Defines the path an issue follows from start to finish |
| **Examples**   | To Do, In Review, Done, Waiting for Approval                     | To Do → In Progress → In Review → Done                 |
| **Scope**      | Individual issue attribute                                       | Project-level configuration                            |

---

### Simple Analogy
- **Status** is a **snapshot** – where you are right now.
- **Workflow** is the **map** – all possible paths and how to move between them.

---

### Example
An issue with status *"In Review"* is part of a workflow that allows it to move:
- *Back to In Progress* (if changes are needed)
- *Forward to Done* (if approved)

The **workflow defines those options**; the **status shows the current location**.

# 16. what's the application of Jira?

Jira is a project management and issue tracking tool developed by Atlassian. Its main applications include:

---

### 1. Software Development
- **Agile project management** (Scrum and Kanban)
- **Bug tracking** – log, prioritize, and fix bugs
- **Release management** – plan and track software versions
- **CI/CD integration** – connect with development tools like Bitbucket, GitHub, or Jenkins

---

### 2. IT Service Management (ITSM)
- **Service desk** – manage customer support tickets
- **Incident management** – track and resolve IT issues
- **Change management** – control and approve infrastructure changes
- **Asset management** – track hardware and software assets

---

### 3. Business Operations
- **Task management** – assign and track work across teams
- **Process automation** – streamline approvals and workflows
- **Reporting** – generate dashboards and insights on team performance

---

### 4. Cross-Team Collaboration
- **Marketing** – manage campaigns and content calendars
- **HR** – track onboarding requests and employee processes
- **Finance/legal** – manage contract reviews and approvals

---

### Summary
Jira is versatile—it helps teams **plan, track, and manage work** across software, IT, and business functions.

# 17. inviting other people to our project

for adding new people to our project, we can add them at the first moment we're creating our project or the other approach is we click on three dots next to project or space name and navigate to space settings -> access -> add people.

# 18. what's list in jira?

In Jira, a **list** (often called an **issue list** or **filtered list**) is a way to view issues as a table or list, rather than on a board.

---

### Key Points

| Aspect               | Description                                                                                        |
| -------------------- | -------------------------------------------------------------------------------------------------- |
| **What it is**       | A structured, tabular view of issues showing fields like summary, status, assignee, priority, etc. |
| **Where to find it** | **Issues** → **Search for issues**; or use **filters** to save custom lists                        |
| **Purpose**          | Bulk editing, sorting, exporting, or analyzing issues without the visual layout of a board         |

---

### Common Uses

- **Bulk operations** – edit, transition, or delete multiple issues at once
- **Exporting** – export issues to CSV or Excel for reporting
- **Filtering** – save a filtered list as a **filter** for reuse or dashboards
- **Tracking** – see all issues across multiple projects in one place

---

### List vs. Board

| View      | Format             | Best For                                         |
| --------- | ------------------ | ------------------------------------------------ |
| **Board** | Kanban/Scrum cards | Visual workflow, daily standups, sprint tracking |
| **List**  | Table rows/columns | Bulk editing, searching, reporting, analysis     |

---

In short, a **list** is the spreadsheet-style view for managing and searching issues efficiently.

in list we have all our issues without any categorization unlike boards and backlogs and it contains boards/sprint and backlog issues together.
# 19. what's filter section in jira?

In Jira, the **filter section** (or simply **filters**) is where you create, save, and manage custom searches for issues.

---

### What is a Filter?

A **filter** is a saved set of search criteria that returns a specific list of issues.

---

### Key Points

| Aspect               | Description                                                                             |
| -------------------- | --------------------------------------------------------------------------------------- |
| **Purpose**          | Quickly find and reuse a specific set of issues without rebuilding the search each time |
| **Where to find it** | **Issues** → **Search for issues** → enter criteria → click **Save as**                 |
| **Access**           | Can be private, shared with a team, or made public within the organization              |

---

### Common Uses

- **Personal** – save filters for "My open tasks" or "Issues I'm watching"
- **Team** – share filters like "All bugs in current release" or "Unresolved high-priority issues"
- **Dashboards** – use saved filters as **gadgets** to display charts and reports
- **Boards** – create boards based on a filter to show specific issues

---

### Filter vs. List

| Term       | Meaning                                           |
| ---------- | ------------------------------------------------- |
| **List**   | The actual results displayed (the issues)         |
| **Filter** | The saved search criteria that generates the list |

---

### Example
- **Filter name:** "My Open Tasks"
- **Criteria:** Assignee = current user, Status not in (Done, Closed)
- **Result:** A list showing only your active issues

---

In short, **filters** are reusable search definitions that help you organize, share, and report on issues efficiently.

when filtering in each project doesn't seem enough, we can navigate to filters section to add more filters and sort our issues and even save them or we can use JQL (a query language like SQL) for sorting and filtering.

in filter we can see all of our issues from all of our projects and then filter them based on the project name.

o navigate to filters, select `Filters` from the pane in the left side.

filtering in board and backlog is useful because filters section and list contain backlog issues as to do and it gives us an inaccurate vision of our filtered issues because we know that backlog issues are not done, we usually want to see which issues are in our sprint or board and not started yet, I changed my mind they can be useful but you should consider backlog issues are part of that filtering also and these filtering are not specific to sprint/board.
# 20. adding to backlog

when adding an issue to backlog, always set the status to `to do` because when you add that to board or sprint it goes in `to do` section and not other sections then from there we can manage that issue and it seems irrational to set the status in the backlog to something else than `to do`, because we haven't done anything to that issue and it should go to sprint or board, so it can go to another stage. 

# 21. what are dashboard in jira and what is its application?

A **dashboard** in Jira is a customizable page that displays key information about your projects, issues, and team activity using visual components called **gadgets**.

---

### What is a Dashboard?

Think of it as a **personal or shared home screen** where you can see an overview of what matters most—without digging through menus or running searches manually.

---

### Key Points

| Aspect         | Description                                                                          |
| -------------- | ------------------------------------------------------------------------------------ |
| **Purpose**    | Provide at-a-glance visibility into project health, progress, and individual work    |
| **Components** | Built using **gadgets** (charts, lists, reports, metrics)                            |
| **Access**     | Can be private (only you) or shared with teams, projects, or the entire organization |
| **Location**   | Access via **Dashboards** in the top navigation bar                                  |

---

### Common Applications

| Use Case                   | Gadgets Used                                                            |
| -------------------------- | ----------------------------------------------------------------------- |
| **Personal task tracking** | "Assigned to Me" filter, "Issues in Progress" list                      |
| **Team progress**          | Sprint burndown chart, Kanban board gadget, created vs. resolved chart  |
| **Project health**         | Two-dimensional filter statistics (e.g., issues by status and priority) |
| **Performance metrics**    | Average age report, resolution time, velocity chart                     |
| **Executive oversight**    | Multiple project trackers, high-level pie charts, workload distribution |

---

### Dashboard vs. Board vs. Filter

| Feature         | Dashboard                  | Board                 | Filter              |
| --------------- | -------------------------- | --------------------- | ------------------- |
| **Purpose**     | Overview and reporting     | Visual workflow       | Saved search        |
| **Interaction** | View-only (mostly)         | Drag-and-drop updates | Returns a list      |
| **Best for**    | Metrics, charts, summaries | Daily work execution  | Reusable issue sets |

---

### Example
A Scrum team dashboard might include:
- **Burndown chart** – track sprint progress
- **Filter gadget** – list of unassigned bugs
- **Pie chart** – distribution of issues by priority
- **Heatmap** – workload by team member

---

In short, **dashboards** turn raw issue data into visual insights, helping individuals, teams, and leaders stay informed without manually searching for updates.

# 22. sharing filters
you can select who can see your filter while you can create them but if you didn't you can navigate to left pane-> filters -> view all filters -> click three dots for filter you want to share and choose who can see the filter or edit it.

# 23. resolution meaning in jira
**Resolution** in Jira indicates if an issue was resolved(done) or unresolved(anything except done e.g. to do, in progress)

# 24. when to use filters section
if you want to filter all of your issues across all of your projects or filters in each project doesn't seem enough, you check on the filters section otherwise you use the filters in each project.

# 25. what are reports in Jira?

**Reports** in Jira are visual tools that analyze and display data about issues, team performance, and project progress.

---

### Common Reports

| Report                      | Purpose                                                             |
| --------------------------- | ------------------------------------------------------------------- |
| **Burndown Chart**          | Tracks remaining work vs. time in a sprint                          |
| **Burnup Chart**            | Shows completed work vs. total scope over time                      |
| **Velocity Chart**          | Measures how much work a team completes per sprint                  |
| **Cumulative Flow Diagram** | Visualizes work in progress across statuses to identify bottlenecks |
| **Control Chart**           | Shows cycle time and lead time for completed issues                 |
| **Sprint Report**           | Summarizes sprint scope, completed vs. incomplete work              |
| **Epic Report**             | Tracks progress of epics and their child issues                     |
| **Time Tracking Report**    | Shows logged time against issues (if time tracking enabled)         |

---

### Key Points

| Aspect           | Description                                                             |
| ---------------- | ----------------------------------------------------------------------- |
| **Purpose**      | Analyze progress, predict future performance, identify bottlenecks      |
| **Location**     | **Reports** section in project sidebar (or via dashboards with gadgets) |
| **Availability** | Depends on project type (Scrum vs. Kanban) and board settings           |

---

### Summary
Reports help teams **measure**, **forecast**, and **improve** their workflow by turning issue data into actionable insights.

# 26. how to identify bottleneck from cumulative flow diagram in jira?
A **Cumulative Flow Diagram (CFD)** in Jira helps identify bottlenecks by showing how issues accumulate across statuses over time.

---

### How to Spot Bottlenecks

| Pattern                                          | What It Means                                                                          |
| ------------------------------------------------ | -------------------------------------------------------------------------------------- |
| **Widening horizontal band**                     | Issues piling up in a status → **bottleneck** (e.g., "In Review" band keeps expanding) |
| **Flat or slow upward slope**                    | Low throughput → work isn't moving through that stage                                  |
| **Steep vertical gap between bands**             | Work waiting to enter the next stage → handoff delay                                   |
| **Growing total line (top) without flat bottom** | Work arriving faster than it's completed → overload                                    |

---

### Quick Steps to Read CFD

1. Look at the **colored bands** (each = a status)
2. Check if any band **widens consistently** over time
3. The **widest expanding band** = the bottleneck

---

### Example
- *To Do* band widens → not pulling work into progress fast enough
- *In Review* band widens → reviewers are overloaded
- *Done* line stays flat → nothing is completing

---

**Remedy:** Focus team effort on the status with the widening band to clear the bottleneck.

when a band remains fixed for a specific amount of issues over a long period, that's a bottleneck.

# 27. useful reports
except for velocity chart for understanding how many story points is good to pick for each sprint based on average story points, other charts are useless and we must check ourselves to see how good our stories and tasks are going, I can track the time either in my excel or on paper but I think excel is better, I think Jira doesn't have any option for it or maybe it has, it doesn't make any difference, if it had I can add it in both Jira and excel.

# 28. bottleneck
we don't have such a thing as bottleneck in scrum because bottleneck is when a story lasts that long that a column like review or in progress gets full and other columns can't add anything to that columns, in the scrum when a task lasts long, the amount of story points we accomplish in that sprint reduces and since there is no column in the structure of the scrum, no bottleneck occurs, we have n story points in scrum and we divide 2 weeks over n number of story points to see how long each story point should last and if the story took longer we have to check on it. 

# 29. from parent I mean the label and tag that allows us to choose an epic for an story or a bug which its options are epics?
Ah, I see what you mean now. Thank you for the clarification.

In that specific context (the **"Parent" field** on a Story or Bug form), **yes – the Parent field is used to link to an Epic.**

### Short Answer:
For standard Issue Types like **Story**, **Task**, or **Bug**, the **Parent field** is essentially an **"Epic Link"** field. Its only options are **Epics**.

### How it works:
1.  You open a **Story** or a **Bug**.
2.  You see a field labeled **"Parent"** (or sometimes "Epic Link" in older/company-managed projects).
3.  When you click into that field, the dropdown only shows **Epics** from your project.
4.  By selecting an Epic, you make that Epic the **Parent** of your Story/Bug.

### Important Distinction (Why it gets confusing):
- **For Stories/Tasks/Bugs:** "Parent" = "Epic Link" (you choose an Epic).
- **For Sub-tasks:** "Parent" = The specific Story or Task they belong to (not an Epic).

### Summary Table:

| Issue Type   | What does the "Parent" field do? | What are the options?                   |
| :----------- | :------------------------------- | :-------------------------------------- |
| **Story**    | Links to an Epic                 | **Epics** only                          |
| **Task**     | Links to an Epic                 | **Epics** only                          |
| **Bug**      | Links to an Epic                 | **Epics** only                          |
| **Sub-task** | Links to its main issue          | **Stories, Tasks, or Bugs** (not Epics) |

So, **yes – in your case, you are correct:** The Parent field on a Story acts as a tag to select an Epic.

# 30. what's timeline application in jira?
In Jira, the **Timeline** (formerly called the *Roadmap*) is a **strategic, Gantt-chart-like view** that shows how work items (Epics, Stories, Tasks) are scheduled over a period of time.

Here is the breakdown of its application:

### 1. Long-Term Planning (The Main Use)
Unlike a Sprint board (which focuses on 1-2 weeks) or a Kanban backlog (which focuses on priority order), the Timeline is designed for **months** ahead. It helps you visualize when a large feature (Epic) will start and finish.

### 2. Visualizing Dependencies
You can draw lines linking issues that cannot be started until another is finished.
- **Application:** If "Design Logo" must finish before "Build Website," you link them on the Timeline. If "Design Logo" slips, the Timeline automatically shows "Build Website" at risk.

### 3. Resource Allocation (Team Planning)
The Timeline shows you every issue assigned to each team member across the week/month.
- **Application:** You can see if one developer is assigned to five overlapping tasks (overloaded) while another has nothing to do (idle).

### 4. Managing Parallel Workstreams
You can group issues by Project, Assignee, or Epic.
- **Application:** You can visually track that "Mobile App work" is on schedule while "Web work" is falling behind, all on the same screen.

### 5. Communicating with Stakeholders
- **Application:** Instead of showing a technical Scrum board full of statuses (In Progress, Code Review, QA), you show a simplified Timeline to executives or clients to answer: *"When will we be done?"*

---

### Summary Table: Where to use it

| Feature                | Best Application                                                                  |
| :--------------------- | :-------------------------------------------------------------------------------- |
| **Sprint Board**       | "What are we doing *today/tomorrow*?"                                             |
| **Backlog**            | "What is the *priority order*?"                                                   |
| **Timeline (Roadmap)** | "Does the *date* of March 15th conflict with the *date* of the Marketing launch?" |

**One important note:** In **Team-Managed** projects, this is called **Timeline**. In **Company-Managed** projects, it is often called **Roadmap** (requires Jira Premium/Cloud).

timeline is useless for me because I use Epics for grouping and as a container and not as a issue that tracks time, for me each Epic will have a share in each sprint and it will last as long as the sprint lasts and my Epic aren't going to finish, they are stable.

# 31. All Work in course
we have a part called as All work in navigation in the course which we don't have it in the Jira, that section is the filters section we have, for using this section navigate to Filters -> search work items

# 32. inserting tasks and stories from Excel
we can insert tasks and stories from excel but the way I've structured tasks and stories in excel cannot be useful in jira and adds again a lots of confusion while sorting them, so you should add them on your own or just copy paste from your own excel file.

# 33. bulk changing in jira
for bulk changes in jira, navigate to filters section, search work items and filter the issues you want to bulk change or at least narrow the list of issues you want to make a change on it, then click three dots in the top right of the page and select bulk change work items.

# 34. importing work items from CSV
you can import work Item from a csv file when you have bulk work items, for doing this you need a csv file with columns and their data, then navigate to filters section, click the three dot or more actions in the top right of the screen and select import work items from CSV, please notice if you use an excel file instead csv, it won't work. 

# 35. goals for each Epic
type down goals that each story follows and when we have sprint, type what goals that sprint follows based on the stories that are involved in that sprints and goals they have and, we have a goal status for each story to see has each story met its goal or not.

# 36. multiple sprints
when we have multiple sprint, all of their issues gets added to the board, it's logical to only start one sprint at once.

# 37. calendar
we have calendar in the jira which we can access it via navigation bar, we can set the due and start date of the stories, we can also set their start date and due date also by clicking each story and setting the due and start date which also get displayed in the calendar also.

# 38. teams
to specify each story and bug team and members, we don't use assignee option in jira because we can only assign each story, bug and task to one person and we have multiple team members for each story and bug, so we type each team name next to title of the story and bug and type team members in description of the story or bug.

# 39. forms
we have forms in the jira which is like a rough notes for our ideas and anything we try to add to our board including a story or bug, we can implement same thing in obsidian, Excel or even on paper so don't worry about this feature, it's something optional we can use but it's not that useful at the end.



