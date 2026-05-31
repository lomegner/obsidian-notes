
confluence is good to write PRD to know what each story scope is and writing retro report to know what's wrong and right and if stakeholders ask why we're following an approach, we can provide evidence based on our retro report results.

use confluence to write PRD and retro report for each sprint as you supply each sprint issues and their info based on your excel file and add PRD of each story and then write retro report for each sprint, you can have pages for each epic to add new ideas in it to refine them after but this one is optional since you can have it also in obsidian or any other app or even on the paper. 

you create each sprint a page for their PRD and retro report with the date of the sprint in the title and inside of the page, after you finished the sprint and you wanted to start the new sprint, you can archive the previous page for reducing clutter, for archiving a page, click the three dots next to page name and select archive and for viewing archived contents, click the space name and click archive space to see archived content.

# 1.what's confluence and its application and what's its difference with jira?

Here’s a clear breakdown of **Confluence**, its applications, and how it differs from **Jira**.

## What is Confluence?

**Confluence** is a team collaboration and documentation tool (a wiki-style platform) made by the Australian company **Atlassian**. Unlike traditional file shares or local documents, Confluence lives in the cloud (or on a server) and is designed for real-time, persistent, organized knowledge sharing.

### Core Applications of Confluence

1.  **Internal Knowledge Base (Wiki)**
    - Store company policies, onboarding guides, FAQs, and best practices.
    - Centralized source of truth to replace scattered Word docs/PDFs.

2.  **Project Collaboration Hub**
    - Create a single page for a project with goals, meeting notes, decisions, and status updates.
    - Link to related Jira issues, design files, or roadmaps.

3.  **Meeting Notes & Agendas**
    - Collaborative meeting notes where teams add agenda items beforehand and capture action items afterward.
    - Action items can be converted into Jira tasks.

4.  **Product Requirements & Design Docs**
    - Draft, review, and iterate on product specs with inline comments and version history.

5.  **Team & HR Documentation**
    - Org charts, team roles, vacation schedules, expense policies, etc.

6.  **Process & Runbooks**
    - Step-by-step guides for incident response, deployment, hiring, or customer support.

---

## What is Jira? (Brief recap)

**Jira** (also from Atlassian) is an **issue tracking and project management** tool. It is built for:
- Tracking tasks, bugs, and user stories.
- Managing agile workflows (Scrum/Kanban boards).
- Assigning work, setting priorities, and monitoring progress.

---

## Key Differences: Confluence vs Jira

| Feature              | Confluence                                                         | Jira                                                                  |
| -------------------- | ------------------------------------------------------------------ | --------------------------------------------------------------------- |
| **Purpose**          | Create, share, and organize *knowledge* and *documentation*.       | Track and manage *work* – tasks, bugs, stories.                       |
| **Core Unit**        | **Page** (content, text, tables, images, macros).                  | **Issue** (task, bug, epic, story with status, assignee, due date).   |
| **Structure**        | Hierarchical (Space → Parent Page → Child Pages).                  | Hierarchical (Project → Epic → Story/Task → Subtask).                 |
| **Workflow**         | No fixed workflow; pages are edited/published freely.              | Strict workflows (e.g., To Do → In Progress → Done).                  |
| **Primary Use**      | “How do we do X?”, “What decisions did we make?”, “Meeting notes”. | “Who is doing what?”, “Is the bug fixed?”, “When will this be done?”. |
| **Owners/Assignees** | Can mention people, but no required owner for each page.           | Every issue has a **reporter** and **assignee**.                      |
| **Reporting**        | No burndowns or velocity; basic page views/edits.                  | Dashboards, sprint reports, control charts, velocity tracking.        |
| **Integration**      | Links to Jira issues; can embed Jira filters on a page.            | Links to Confluence pages; can create Confluence pages from Jira.     |

---

## How They Work Together (Not Either/Or)

Most teams use **both** together:
- **Jira** tracks *what* needs to be done and *who* is doing it.
- **Confluence** explains *why*, *how*, and *what was decided*.

**Example flow:**
1. Product manager writes a **Product Requirements Doc (PRD)** in Confluence.
2. From that PRD, they create **Jira issues** (stories/tasks) linked back to the Confluence page.
3. Developers update Jira as they work.
4. After the sprint, the team adds **retrospective notes** to Confluence, linking to the completed Jira issues.

---

## Quick Summary

|                       | Confluence                            | Jira                                             |
| --------------------- | ------------------------------------- | ------------------------------------------------ |
| **Type**              | Collaboration + documentation         | Issue tracking + project management              |
| **Question answered** | "What do we know?"                    | "What do we need to do?"                         |
| **Best for**          | Wikis, meeting notes, specs, policies | Agile development, bug tracking, task assignment |
| **Structure**         | Pages + Spaces                        | Issues + Projects                                |

If you need a **single source of truth for documentation** → **Confluence**  
If you need to **track tasks and manage workflows** → **Jira**  
If you need both (most common) → **Integrate them**

# 2. what are space, page and macro in confluence?

Here’s a concise explanation of **Space**, **Page**, and **Macro** in Confluence:

- **Space** – A high-level container or folder for related content. Think of it as a project or team "area" (e.g., "Marketing Space" or "Engineering Space").

- **Page** – The actual document or content unit inside a space. Pages can have child pages to create hierarchies (like a website tree).

- **Macro** – A reusable add-on component you insert into a page to add dynamic features (e.g., a task list, Jira issue table, calendar, code block, or info panel).

spaces contain pages and pages contain content like image and text, spaces are like project in jira and pages are like issues in jira.

# 3. what are team space and personal space in confluence and what are their differences?

Here’s the difference between **Team Space** and **Personal Space** in Confluence:

## Team Space
- **Purpose** – Shared collaboration for a group (e.g., a department, project, or product team).
- **Ownership** – Owned by the team; multiple members can edit, view, and manage content.
- **Visibility** – Usually open to the whole team or company (permissions can be restricted).
- **Content** – Project plans, meeting notes, documentation, decisions, runbooks.

## Personal Space
- **Purpose** – Private workspace for an individual user.
- **Ownership** – Owned and controlled by one person.
- **Visibility** – By default, only the owner can see/edit (can share with others if desired).
- **Content** – Drafts, personal notes, to-do lists, work-in-progress documents not ready for the team.

## Key Differences

|                     | Team Space              | Personal Space         |
| ------------------- | ----------------------- | ---------------------- |
| **Who uses it**     | A group                 | One individual         |
| **Default access**  | Team members            | Only the owner         |
| **Typical content** | Shared knowledge        | Private drafts & notes |
| **Permissions**     | Managed by space admins | Controlled by owner    |

personal space is like team space and there is no difference, just each user can have a personal space for itself and set the access to a point that only that specific user can view it and not other team members for their own notes and drafts, for creating personal space click the profile icon in the right side of the screen and click personal space, you can restore your personal space after you delete this from the same options (for deleting a space, click the three dots next to space name and select delete space), for creation of a team space, click the spaces  in the left side of the screen and select `create a space`, application-wise there is no difference between personal and team space.
# 4. as a product manager, how can I use confluence and what are the applications of confluence for me?

As a product manager, Confluence becomes your **single source of truth** for product knowledge, decisions, and collaboration. Here’s how you can use it:

## Key Applications for a Product Manager

### 1. Product Strategy & Roadmaps
- **Vision & strategy docs** – Keep your product vision, mission, and OKRs in one place.
- **Roadmap pages** – Use timelines or Jira roadmap macros to share high-level plans with stakeholders.
- **Quarterly planning** – Document goals, initiatives, and success metrics.

### 2. Requirements & Specifications
- **PRDs (Product Requirements Documents)** – Write, iterate, and review specs with inline comments.
- **User stories & acceptance criteria** – Link directly to Jira issues for traceability.
- **Feature briefs** – Quick one-pagers for early alignment before detailed specs.

### 3. Discovery & Research
- **Customer interview notes** – Share synthesized insights from user research.
- **Competitive analysis** – Maintain living documents on market landscape.
- **Feedback repository** – Collect and categorize customer requests (linked to Jira tickets).

### 4. Prioritization & Planning
- **Prioritization frameworks** – Show RICE, Kano, or WSJF scoring in tables.
- **Sprint planning pages** – Embed Jira filters to review backlog before planning.
- **Release notes drafts** – Collaborate with marketing and support on upcoming releases.

### 5. Decision Logs & Alignment
- **Decision records** – Document *why* you chose one direction over another (saves future arguments).
- **Meeting notes** – Run stakeholder meetings with shared agendas and action items.
- **RFCs (Request for Comments)** – Propose changes and gather feedback asynchronously.

### 6. Go-to-Market (GTM) Coordination
- **Launch checklists** – Use task list macros to track launch activities.
- **Messaging & positioning** – Share with sales, marketing, and customer success.
- **Sales enablement** – Store FAQs, demos, and battle cards.

### 7. Team Collaboration
- **Team space** – Share weekly updates, metrics dashboards, and best practices.
- **Onboarding** – Create a "New PM" guide with links to tools, processes, and key docs.
- **Retrospectives** – Capture what went well and what to improve after each release.

## Example Workflow for a PM

1. **Discover** → Write interview notes in your **personal space**.
2. **Synthesize** → Move key insights to **team space** under "Research & Insights."
3. **Define** → Create a **PRD** page with linked Jira epics/stories.
4. **Plan** → Build a **roadmap** page with embedded Jira filters.
5. **Align** → Share with stakeholders via page comments and @mentions.
6. **Launch** → Use a **launch checklist macro** and draft release notes.
7. **Retro** → Document learnings and link back to the original PRD.

## Bottom Line

Confluence helps you **stop repeating yourself** (answers to "Why did we decide that?") and keeps everyone aligned without endless email threads or outdated Word docs. It's your memory and communication hub as a PM.

# 5. is it a good idea to check on the previous product manager of the company confluence notes to see what it wrote so we can do the same thing with same structure?

It’s a **good starting point, but don’t blindly copy it**. Here’s a balanced view:

## ✅ When it’s a good idea

- **Learn the company’s vocabulary** – What they call epics, initiatives, or customer segments.
- **Understand past decisions** – Why certain features were built (or killed), what research was done.
- **Follow existing conventions** – If stakeholders are used to a certain structure (e.g., where release notes live), changing it causes friction.
- **Avoid reinventing the wheel** – Meeting note templates, PRD formats, or launch checklists that worked well.

## ❌ When to be careful

- **The previous PM wasn’t effective** – Their structure might be messy, incomplete, or the reason the team struggled.
- **Context changed** – New tools, processes, or team culture may require a different approach.
- **You’re just copying without understanding** – You might inherit bad habits (e.g., over-documenting, never updating pages).
- **The team hated it** – Ask your engineers, designers, or QA if that structure actually helped them.

## ✅ A better approach

1. **Read everything** – Absorb the content and logic.
2. **Ask the team** – “What worked? What was painful about the old PM’s docs?”
3. **Keep what works** – Templates, key decision logs, useful macros.
4. **Improve what doesn’t** – Simplify, reorganize, or retire outdated pages.
5. **Document your changes** – Add a “Structure update” page explaining what you changed and why.

## Bottom line

Use the old PM’s notes as **reference and archaeology**, not as a blueprint. Your job is to evolve the process, not just maintain it.

# 6. do I need to have a retorrespective report in my confluence as a product manager and  what does it look like?

## Do you need a retrospective report in Confluence?

**Not strictly required, but highly recommended.** As a product manager, you don't own the agile retro (that's typically the Scrum Master or team lead). However, having a **product-focused retrospective report** in Confluence is valuable for capturing learnings that affect roadmap decisions, prioritization, and stakeholder alignment.

## What a Product Retrospective Report looks like

Here's a simple, practical template:

---

### 📄 Title: [Product/Release Name] Retrospective – [Date]

**1. Quick Summary**
- What shipped: [list key features]
- Timeline: [start date] → [launch date]
- Goal met? ✅ / 🟡 / ❌

**2. What Went Well**
- Shipped on time
- Adoption metrics hit target
- Cross-team collaboration was smooth

**3. What Didn't Go Well**
- Missed scope (X feature cut)
- Delayed due to late requirements
- Stakeholder alignment issues

**4. Key Learnings (Product-specific)**
- Users didn't use feature Y as expected → validate earlier next time
- Technical debt blocked velocity → allocate 20% to debt next quarter
- Competitor launched similar feature → adjust messaging

**5. Action Items (Owned by PM)**
| Action | Owner | Due |
|--------|-------|-----|
| Update PRD template to include risk section | You | MM/DD |
| Schedule customer beta for next release | You | MM/DD |
| Share learnings with leadership | You | MM/DD |

**6. Links**
- Link to team's agile retro notes (if separate)
- Link to Jira epic/release
- Link to metrics dashboard

---

## When to create this report

- After each **major release** (not every sprint)
- After a **failed or delayed launch**
- **Quarterly** for ongoing products

## Bottom line

You don't need a retro after every sprint (let the team run theirs). But a **product retro report** in Confluence helps you:
- **Justify roadmap changes** with real learnings
- **Avoid repeating mistakes** across releases
- **Show leadership** you're data-driven and reflective

# 7. do we need a report for our daily meeting in conflunece or for sprint refinement meeting?

Short answer: **No, you don't need a full "report" for either.** But lightweight documentation helps.

## Daily Standup (Daily Scrum)

**Do you need a report?** ❌ No.

**What to do instead:**
- **No Confluence page** – Daily standup is for coordination, not documentation.
- **Use Jira** – Team updates happen around the board (moving tasks, updating statuses).
- **Only document** if there's a recurring blocker or decision worth capturing – add a quick bullet to an existing "Decisions" page.

**Over-documenting daily meetings** creates busywork nobody reads.

---

## Sprint Refinement (Grooming)

**Do you need a report?** 🟡 Yes, but keep it lightweight.

**Why it helps:**
- Refinement often spans multiple sessions over the sprint.
- You need a record of what was discussed, estimated, or deferred.

**What it looks like (not a formal report, just a running page):**

> 📄 **Sprint Refinement Notes – [Sprint Name/Date]**
>
> **Backlog items refined:**
> - TICKET-123 – Added acceptance criteria, estimate: 5 points
> - TICKET-456 – Split into two smaller tickets (TICKET-457, TICKET-458)
> - TICKET-789 – Deferred to next release (needs more discovery)
>
> **Open questions:**
> - TICKET-123 – Confirm API rate limits with backend team
>
> **Decisions:**
> - We'll prioritize tech debt ticket TICKET-999 in next sprint

**Format:** One shared page that gets updated each refinement session (not a separate page per session).

---

## Summary

| Meeting               | Report needed? | What to use                              |
| --------------------- | -------------- | ---------------------------------------- |
| Daily Standup         | No             | Jira board only                          |
| Sprint Refinement     | Light notes    | One running Confluence page per sprint   |
| Sprint Review         | Yes            | Confluence page with demo notes, metrics |
| Sprint Retrospective  | Yes (team)     | Confluence page (team owns it)           |
| Product/Release Retro | Yes (PM)       | Confluence report per release            |

**Rule of thumb:** If nobody will read it next month, don't write it.

# 8. what's the point of this documentation for prd and retro, why we do this ?

Excellent question. It gets to the **"why"** behind the work, not just the "how."

The point of PRDs, retrospectives, and similar documentation isn't to create paperwork. It's to solve five fundamental problems that kill products and frustrate teams.

Here’s why you do each one:

---

## Why a PRD (Product Requirements Document)?

**The core problem:** Everyone has a different picture in their head of what you're building.

**The point of the PRD is to:**

1.  **Force clarity on *you*** – Writing something down reveals the gaps in your own thinking. An idea that sounds perfect in your head often falls apart on paper.

2.  **Create a shared contract** – Not a legal contract, but a mutual understanding between PM, designers, engineers, and QA. "We all agreed this is the scope, these are the success metrics, and this is out of scope."

3.  **Stop "telephone game" decay** – You tell designer → designer tells engineer → engineer tells QA. Each hop loses detail. The PRD is the single source of truth everyone refers back to.

4.  **Provide a decision anchor** – When someone asks later, "Why didn't we support X?" you can point to the PRD's "Out of Scope" section. Without it, you rely on memory (which fails).

5.  **Enable async work** – Engineers in different time zones or teams can read the PRD and start asking informed questions without you repeating yourself 10 times.

**Without a PRD:** Endless meetings, rework, scope creep, "I thought you meant Y," and finger-pointing at launch.

---

## Why a Retrospective Report (Product-focused)

**The core problem:** Teams repeat the same mistakes because no one writes down the lessons.

**The point of the retro report is to:**

1.  **Turn experience into institutional memory** – When you leave or get promoted, your hard-won lessons shouldn't leave with you. The next PM inherits your wisdom, not just your mess.

2.  **Stop repeating the same failures** – "We underestimated API work again" → If you document it, you can spot the pattern and fix the root cause (e.g., always add 30% buffer for integration work).

3.  **Justify roadmap changes with data** – When leadership asks, "Why are we slowing down feature work to pay down tech debt?" you point to the retro: "Three consecutive releases delayed due to brittle code. Here's the evidence."

4.  **Celebrate what worked** – Teams need to know what they're doing right. Documenting wins helps replicate good behaviors across the org.

5.  **Build a learning culture** – When you publicly share "we messed up X and here's what we learned," it gives permission for everyone else to be honest about failures instead of hiding them.

**Without a retro report:** The same arguments happen every quarter. No one remembers why you stopped using a certain process. Lessons die with the people who learned them.

---

## The One-Sentence Summary

| Document  | Why you write it                                                              |
| --------- | ----------------------------------------------------------------------------- |
| **PRD**   | So everyone builds the *same* thing, and you remember *why* later.            |
| **Retro** | So you stop making the *same* mistakes, and keep making the *good* decisions. |

---

## The Real Test

Before you write any document, ask yourself:

> *"If this page disappeared tomorrow, would anyone notice or care in six months?"*

If the answer is **no**, don't write it. If **yes**, that's the point.

# 9. adding member in confluence
in adding members, if you're not admin, the admin will be notified and it should allow you to add new members.

# 10. what are templates in confluence?
Here's a concise explanation of **templates** in Confluence:

## What are Templates?

**Templates** are pre-built page structures that save you from starting from scratch. They include placeholder text, sample sections, macros, and formatting.

## Analogy

Think of templates like **document blueprints**:
- Blank page = empty Word doc
- Template = letterhead + "Dear [Name]," + signature block already there

## Common Examples

| Template                  | What it gives you                                                     |
| ------------------------- | --------------------------------------------------------------------- |
| **Meeting notes**         | Agenda, attendees, discussion, action items (with task macro)         |
| **Product requirements**  | Problem statement, goals, user stories, success metrics, out of scope |
| **Project retrospective** | What went well, what didn't, action items, metrics                    |
| **Decision log**          | Decision, rationale, alternatives considered, date, deciders          |
| **How-to guide**          | Goal, prerequisites, numbered steps, tips, related links              |

## Why Use Them

- **Save time** – No rebuilding the same structure every time
- **Consistency** – Every PRD looks the same (easier to read)
- **Reduce mistakes** – Don't forget sections (e.g., "Out of scope")
- **Onboard faster** – New PMs know exactly what to include

## Where Templates Live

| Type                                       | Who can use it        | Where to find it               |
| ------------------------------------------ | --------------------- | ------------------------------ |
| **Global templates** (Atlassian defaults)  | Everyone              | Create → "Browse templates"    |
| **Space templates** (custom for your team) | Members of that space | Space Settings → Templates     |
| **Your personal templates**                | Only you              | Save any page as "My template" |

## How to Use One

1. Click **Create** in Confluence
2. Pick a template (e.g., "Meeting notes")
3. Fill in the placeholders
4. Publish

## Bottom Line

**Templates = Don't reinvent the wheel.** If you find yourself building the same type of page over and over, save it as a template. Your future self (and your team) will thank you.

for using template, click a page and click the three dots in the right side, choose `template and import`, just bear in mind as long as you haven't published your page, you can add template, as soon as you publish it, you can't change template or add a new template.

# 11. how to add new page
click the global `create` button next to search bar or in each space setting, under content, click the `create` button.

# 12. how to promote a template and disable it
promote is like a filter in template that let your specified templates sit aside.
to promote a template, there is a three dot next to each space name, click that, navigate to 
`look and feel`, `templates` and from there, you can promote any template you want or even disable it (remove it from template list), notice that each person that creates a space has access to space setting and subsequently the template setting, other people can't. 

# 13.editing of a page
while writing content or editing the page, is like jira comment or description and it supports markdown.

# 14. drafting and publishing
when you write a new page, and you hit close button instead of publish, that page or content gets drafted and is only visible to the person and user who has written it, after that you can publish it, from now on, any time you make a change to a published page and content, you should update the page otherwise the new non-updated changes won't be displayed and anyone can see non-updated changes when they click content regardless of who has made the change.
for seeing the non-updated changes, click the page, click the edit button, click the three dots in the right of the screen and click view changes.

# 15. how to write page for each sprint
you create each sprint a page for their PRD and retro report with the date of the sprint in the title and inside of the page, after you finished the sprint and you wanted to start the new sprint, you can archive the previous page for reducing clutter, for archiving a page, click the three dots next to page name and select archive and for viewing archived contents, click the space name and click archive space to see archived content.

# 16. users and accounts 
first of all the integration between Atlassian products is useless because they don't have enough access and info, for example using work items of jira in confluence is useless because when I import issues of a specific project, it shows all of the issues ( sprint + backlog ) not the one related to a sprint and there is no way to filter it, in a PRD, I just want the issues related to a sprint, so its better to use my own excel sheet to import issues.

you can invite people to your confluence spaces via invite people in the bottom left of the screen, if you get invited to multiple confluence accounts and you accept them, you have only access the one which is accepted the latest not the others.

for giving access to spaces and removing people, click the three dots next to space setting and click `users`.

don't use multiple accounts for Atlassian products, just use one Gmail or email for all of the three (Jira, Trello, Confluence)

based on works we do in each of them as a product manager, other team members should be viewer in Jira and confluence (just to see tasks in Jira and check the PRD in the confluence) but they should be able to have editing role in Trello to add bugs. 

