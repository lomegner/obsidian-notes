
# 1. what's Microsoft Visio?
it's an application for drawing charts and diagram, it's good for s when we want to display epics and stories for each sprint along side our KPI in the meeting or to demonstrate our WBS in the meeting or as a BI analyst it may be useful when we're analyzing solution and outcome out of our Power bi reports and now we're creating a flowchart or diagram for step-step plan for our solution to improve e.g. sales, profit or a specific KPI or maybe it's not that useful as BI analyst because I think solution is what managers decide what to do and BI analyst only prepares reports but this application is quite useful as a product manager or project manager.

# 2. adding shapes to the page
for adding shapes to page just drag and drop them from left side of the application. for adding different type of shapes, select more shapes from shapes section in the left side and add your desired shape type.

for instance we can add flowchart, in flowcharts the oval is for start or end of our project and represents the title for beginning and finish like opening a restaurant (start of project) and the actual opening or grand opening ( end of project), the rectangle represents what we're going to do and represents action like buying meat, buying chairs, the rhombus represent the if statements and the result will be in the rectangle and for documents like hiring staff and signing contract we use document shape.

# 3. connectors
for connecting two shapes together, we use connectors, connectors are two types: dynamic and static. for dynamic connector we select connector from home -> tools -> connector and select the shape center we want arrow to be from it to another shape and hold left side of the mouse and drag it to the center of our destination shape center, in dynamic connectors wherever we take the shape, always the origin shape chooses the shortest path to the destination shape based on the  
points are available on the shapes (some points are available on the shapes that connector line, connects based on those lines) and always the arrow direction is from the first shape we select to second shape we select.

for static connectors, select from home->tools->connectors, drag the connector from the available point of origin shape to destination shape. the difference if we move our shapes, the connector line will be connected between two available points we selected on our shapes and the app doesn't pick the shortest path of available points to connect shapes.

in fact there is no difference between these two type of connectors but I prefer static due to stability.

# 4. visualization of shapes
for changing color of the shapes navigate to home->shape-> fill, and click on our specific shape and change its color, for removing borders of our shape or visualizing our borders navigate to home -> shapes -> line ( select no line for removing borders), we have format painter option we had in power bi, you can use it from home-> clipboard-> format painter

for changing color of connector lines select one of them or hold ctrl and select multiple or all of them and then select home-> shape ->line section and change their color.

for adding text to our lines like for our if statement to see what happens in each true and false  scenario and to specify true and false for each by writing down `YES` or `NO`, we can use texts, navigate to home -> tools -> text and click on wherever of your connector which you want a text and type down your text, you can do this by double clicking on the lines also.

you can add text via this text option on anywhere or blank area of our page also and it's not limited to lines only.

# 5. `ctrl+d` shortcut
by holding `ctrl+d` while a shape is selected, you can duplicate it and there is no need to `ctrl+c` and `ctrl+v` it.

# 6. callout
we use callout to give extra information about each shape or step in our diagram, like if our step or shape text is opening a restaurant, the callout can be the possible name of restaurant like   `Lome gourmet`, this callout can be a name, location or number and etc.

# 7. grouping
for example we want to move some part of our diagram together, we can group some parts or all of them to move together, for grouping shapes, click on any shape you want to group, then hold `ctrl` and click other shapes, then navigate to home -> arrange -> group -> group and for ungrouping them, navigate to same path and this time choose ungroup, for grouping all of the shapes together, just click on page and hold `ctrl+a` and then navigate to home -> arrange -> group and group them.

# 8. templates
we have templates in the Microsoft Visio which allows us to use the most used shape type as a category, some of the template provides some extra feature like wizard that you can't access while accessing them normally instead of templates like in organizational chart template and they may have some drag and drop auto connection features.

for using template navigate to file -> new.

# 9. organizational chart wizard
in the template section we have a wizard template for organizational chart, you can import a specific excel file with special header and cell format to be used as data of your organizational chart members or you can allow the application to create a sample for you and modify it, it depends on the situation, you can enable this wizard if you have used the organizational chart template by navigating to org chart -> organizational data ->import.

for using an already existing excel or text file, select `information that's already stored in a file or database` and for using the auto generated sample from Microsoft Visio, select `information that I enter using wizard`.

use template if you need wizard or ease of use is important to you in organizational chart, otherwise just create it manually.

you can fine organizational chart wizard template in template path which we addressed in the previous point.

organizational chart is basically a chart full of members and their relation to each other showing who works in which department and who is the manger of other people and who is employee

for using wizard it's better to use wizard template instead of regular organizational chart template and enable template manually.

always mention `name` and `reports_to` field in the excel, otherwise no connection and shape will be created for that specific employee in our organizational chart.

use template for ease of use and wizard for ease of use and inserting data automatically from a file.

you can create an organizational chart via organizational chart shape type or other shapes like basic shapes, only the hierarchy matters, the shapes and names are not important.

always look for your shapes from template first and then check on shapes because template offer more features.

sometimes template contains multiple shape type together when we click them like floor plan template and if we want to create a floor plan we have to import lots of shapes on our own without knowing their name but by searching in template since they're less of them we can find the shapes for the idea we have in our mind.

you can create an excel file on your own with columns even with headers rather than `name` and `reports_to` (but it's better to name `name` and `reports_to` because of convention) for your wizard.

wizard is useful when you have a list of employees and their managers and you want to create an organizational chart out of it, instead of typing down everyone, wizard makes it automatically for you and their relation (after creation of organizational chart by wizard, you can change name, positions and their connection easily if you didn't like it) or when you're comfortable to type employees and mangers in an excel and their connection and let the wizard, create the chart for you.

 in the wizard section there is a part where it has a toggle option which in the left side we have `data file column` and on the right we have `displayed fields`, for data file columns, we should add columns we know which will be our connectors which is our `reports_to` and on the right side put whatever you want to display in the shapes.

but if you can create the organizational chart manually since you have more control over it and you can choose type of shapes.
# 10. search option in shape
if you can't find a shape, you can easily search for it, if the search option was unavailable, simply right click on the shape text on the left side and select search options, a menu opens in advanced section of it, in shape search section, check show shape search pane box.

# 11. home floor plan
in the home floor plan we need a room and space at first and then we can add appliances, for room and space, check wall, shell and structure shapes and after adding space, you can right click it and select properties to change its default name from office to kitchen.

# 12. flowchart quick access
in flowchart, when we hover over available points on the shapes, there are arrows below/above them, by hovering over them, we have option to add commonly used flowchart shaped, dynamically connected to our existing shape.

# 13. containers
containers are good to group and contain multiple shape to say they related to a specific time period or phase or department or people, for adding container, navigate to insert -> diagram parts -> container, before adding container, select all shapes and their related connectors that you want to be in a container by holding ctrl and then adding container.

container can be used for illustration of each phase and timing of each section of a project, department of each task or tasks related to each team.

# 14. connectors
connectors are lines, we can even change their direction and turn them from arrow to straight line (by clicking the connector and navigating to home -> shape -> line), we have shapes in Visio and can show their relation to each other ( from which shape to which one or even if it's bi-directional or they just are connected to each other with any direction like in organizational chart) by using connectors, so that's the application of the connectors.

we have shapes and connectors in the Visio, we can use shapes only to demonstrate a concept or present in a meeting or we can use combination of shapes and connectors to show relationships between them like what we do in flowchart, we have shapes and lines, lines demonstrate each step and what happens when a step finishes and what step we have after each step and what task starts after a task finishes. 

# 15. cross-functional flowchart
in cross-functional flowcharts we have flowchart which we can specify the phase like what we have in containers and each team working on each tasks but team specification is a little bad unorganized and ruins the concept of illustrating tasks below each other to show that tasks are related to each other and each task should finish so another task starts, instead of 
cross- functional flowchart, if you want to specify phases and teams, use basic flowchart shapes and then use container for phases and callout for team specification of each task, in this case, tasks remain under each other and show the concept of flowchart which is to show how tasks relate to each other and each task is dependent of another task by putting task in each phase under the previous task but in cross functional flowchart for making the team specification correct we may have to put one task which is dependent to another task finish above of it for correct team specification which this violates the rule of flowcharts that each task is dependent of previous task and should be under the previous task for each phase, so for fixing this we have to remove team specification by using callouts and everything works fine and therefore we don't need cross functional flowchart and use basic flowchart.

# 16. double clicking a text to edit
if we double click a text, we are able to edit like change it's color or its font-size.

# 17. putting a shape in front or behind of another shape when 2 shapes are overlapping
when two shapes are overlapping we can put one of them in front of another one or behind, by selecting our target shape and navigating to home -> arrange -> bring forward (for bringing forward) / send backward (for sending backward), for using these options it's better our shapes to be overlapped (in the normal situation they take effect also but it's better to be done in overlapped situation for avoiding any confusion).

# 18. text box
text box in insert -> text -> text box is the same tool we have in home -> tools ->text and works exactly the same.

# 19. creating custom shape type
for creating a custom shape type, click on more shapes, new stencil, then drag and drop shapes from other shape type to your custom shape type (the shapes should be on page and then you drag and drop it in your custom shape pane), when you drag and drop it, if they are filled with any color or any visualization applied on them, you can see them in your custom shape and those visualization are part of your shape from now on even a text.

you can change the name of your shape by right clicking on them and selecting rename master, then you save your shape by clicking the save icon in the shape pane and choose your custom shape container name and from n ow on you can use it from more shapes -> my shapes.

you can add new shapes to your custom shapes ( you can do it only to custom shape container and not built-in shape container) any time you want by opening your custom shapes and drag and drop your desired shapes to your custom shapes.

you can create a custom shape type for commonly used shapes or specific shape you use for a specific scenario.
# 20. hyperlinks
we can link to multiple locations in Microsoft Visio, first to another site, second to another file on our machine and last one is to another page in our Visio file.

for giving a hyperlink to a shape you should select the shape and then right click on it and choose hyperlink or navigate to insert -> links ->hyperlink

you can add multiple hyperlink to a single shape, for adding a second hyperlink after navigating to hyperlink path, in the popped up modal, select `new` and click browse and add your link to the shape, when browsing local file, please notice to toggle file type to all files and not just Visio files.

for editing your hyperlinks, select your shape and right click on them and click edit hyperlinks.

for adding websites, you should type it in the first blank and using browse option won't help you.

process -> subprocess -> create new is like what we have as sub-address in hyperlink section and there is no difference in it and it just enables to link to another page in Microsoft Visio, the only difference it has that process option creates a new page on fly but for linking to another page in hyperlink we should make the new page.

for navigating to specific link, linked to a shape just click the shape and hold `ctrl+click`.

linking a page to another page is useful when you want to elaborate the structure of a step in another page, like a step of a specific flowchart, itself can be a separate flowchart so we link that step to another page to elaborate it.

# 21. pivot diagram
we have pivot diagram in Microsoft Visio that you give an excel worksheet to it and it creates a pivot table out of it but represented as hierarchical chart and it works exact same as pivot tables in excel.

for removing a category, select the category from the pane in the left by clicking the chevron next to it, then click `select All` and press delete button and they will be removed.

after deleting a specific category, for better visualization and having neater structure, we should 
re-align and re-space our items to put them along side each other with even space between them, for doing this select unorganized category by clicking `select All` option from the pane in the left and then clicking the home->arrange->auto align and space.

# 22. general application of Microsoft Visio
Microsoft Visio get used for convenience in understanding of topics and presentation of subjects and topics in meetings for displaying relationship between tasks, people and tasks and people together, flowcharts get used for understanding how an application flow goes or for starting a project like opening a cafe or WBS, organizational chart can be used for key influencers or stakeholders of a company, basic shapes can be used for WBS or a project overview, floor plan is not that useful since there are lots are more better application for that purpose and pivot diagram is not that useful also since it's same as pivot table in excel.

for presenting these topics in a meeting, the application is the best option because you have access to features like hyperlinks and etc. but if you want to send a file or present in a way that you want to show relationship between diagram and dashboard across 2 or more apps like 
power bi and Visio and explain about that relationship, you better use application like 
power point. 

# 23. Microsoft Visio application as a product manager and BI analyst and project manager
Microsoft Visio, I think doesn't have any specific application as a BI  analyst, as a product manager it doesn't have any prominent application also but it may be used as a visualization between our epics and stories or as a tool to illustrate tasks of a story (if Jira or other application don't do these actions) and we can present them in the meeting but its main application is as a project manager to create our WBS diagram with all of the resource allocation, risks, contingency management
and so on.

# 24. general application of Microsoft Visio
**Microsoft Visio** is a diagramming and visualization tool that helps users represent complex systems, workflows, and structures in a clear, visual format.  
Here’s how it’s generally applied across disciplines:

---

### **1. Process Visualization**
- Used to create **flowcharts**, **business process models**, and **workflow diagrams** that describe how tasks or operations move through a system.  
- Helps identify inefficiencies, duplication, or unnecessary steps in organizational processes.

---

### **2. Organizational & Structural Mapping**
- Commonly used for **organizational charts**, illustrating company hierarchies, teams, and reporting relationships.  
- Useful during restructuring or project planning to visualize roles and responsibilities.

---

### **3. Technical & Engineering Diagrams**
- Supports **network diagrams**, **IT architecture**, and **software system design**—showing servers, databases, and data flow connections visually.  
- Engineers and IT professionals use it to plan infrastructures or troubleshoot system dependencies.

---

### **4. Facilities & Spatial Planning**
- Enables creation of precise **floor plans**, **office layouts**, or **space utilization designs** using scalable shapes and dimensions.  
- Often integrated with architectural or facilities management workflows.

---

### **5. Data-Linked Visualization**
- Can link shapes and diagrams directly to **data sources** (Excel, SharePoint, SQL, Power BI) so visuals update dynamically with real data.  
- This is ideal for dashboards or monitoring visualizations.

---

### **In essence:**  
Visio is not just about drawing—it’s about turning **data, processes, and systems into clear, interactive diagrams** that make communication and analysis faster and more intuitive across business, IT, and operations.

# 25. what's the difference between us units and metric
 it's bullshit, choose the metric unit always, it doesn't make a difference if you choose any of them.
it's useful when you have a shape that requires measurement, if you choose us units, the measurement will be in us units and if you choose metric units, the measurement will be in metric units.
