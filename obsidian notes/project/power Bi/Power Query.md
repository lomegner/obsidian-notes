
# 1. Using power query in excel
we have power query and power pivot (data model) in excel and I don't see any reason to use it because for large dataset, excel will crash and visualization and normalization doesn't make sense because if excel worked properly with large dataset with excel, so why they created power bi and for small amount of dataset (until excel crashes) we can visualize without need to normalize and using power query and power bi, the only case is our data is in range of excel dataset but when we want to visualize, it gets slow, so since we want to have access to data entry feature, we normalize our table to have a fast visualization alongside to our data entry feature but I think in practice, it's something rare and visualization will work fine as long as data size is as large as excel working range.
I earlier mention power query can be used for merging two worksheets but for merging we should have a common column which we usually don't have for two random worksheets, so power query and power pivot are actually useless in excel.

# 2. transferring Excel data to power query
for transferring data to power query, we navigate to data tab, get and transform data section, from table/range for importing from excel table or range and we have other options too.

# 3. column profiling
color bar below headers of the each column indicating how much of columns values are valid, how many errors and empty cells we have, it gets calculated based on the first 1000 rows.

# 4. removing rows
we can remove rows from top or bottom for a specified number of rows, for doing this in the home tab, in reduce rows section, select remove rows, by clicking top rows, we can remove rows from the top for a number of rows.

# 5. removing null or blank values from columns
click on chevron next to each header and click remove empty, to remove empty columns.

# 6. uppercasing and formatting each data
for uppercasing each data or capitalizing each word, we navigate to transform tab, text column section, select format and you can capitalize each word, uppercase and lowercase each letter of the selected column.

# 7. loading data into excel from power query
home -> close -> close load
after navigating to specific address, you have two options: 1. close and load which loads data into a new worksheet and 2. close and load to... which you can select a worksheet and load into that.

# 8. how to open power query in excel
there are 2 approaches to open power query in excel: 1. data -> get and transform data -> get data -> launch power query editor
 2.data -> queries and connection -> a section opens up in the right side of the excel, select and right click an existing table and click edit.

# 9. changing names of applied steps and gear icon next to them 
you can change name of the applied steps by right clicking on them in power query, also there re some gear icon, next to some of the steps which allows us to edit that step.

# 10. another name of fact table
transactional table is other name of fact table.

# 11. using first row as header
we can set our first rows a s our header of each column, for doing this, you only need to navigate to home -> transform -> use first row as headers

by clicking this feature, we have two options: 1.use first row as headers which is also known as promoting headers that makes our first row as headers of each column and 2, use headers as first row which is also know as demoting headers that adds our headers as first row to each column and each column header name changes to column1, column2 and so on.

# 12. unpivoting columns
unpivoting columns are for when we want to use our headers as values of a cell, like when the column headers names are locations and their values are price for that location for that specific product, when we unpivot the locations, each product gets all of the location headers and their prices in aa new column, for unpivoting and in case we add new columns e.g. new locations and keep our data refreshed and updated and include the recently added column as part of unpivoting process, we select the columns we don't want to be unpivot and in unpivot setting, we select, unpivot other columns.

path to unpivoting:
transform -> any column -> unpivot columns

that's one of the features that power query enables for us which is not possible to do in the excel and power bi, it's good for cleaning data and having neat data to work with.

# 13. selecting a folder and combining multiple excel worksheets
this action is bullshit and always import a single excel file instead of a folder.

# 14. another type of merging
what we had as merging so far was left outer which was basically  A U B which was plus of two queries called A and B, we have another merge called left anti which A-B which the difference between A and B which are our queries ( U and - are algebra symbols), so in left anti, power query checks the common column between the top query and bottom query, and deletes whatever is  mutual between them from the top query and adds noting to fist query (if you expand imported column from bottom table to top table, it's null, so it's just better to remove that column), the left outer application was when we wanted to add a column from another table to another one like when we add index in normalization, the left anti is for when we want to compare two table and remove whatever mutual from the first one like we have two products list and the second one is expired products list, we use the left-anti to remove mutual products from the first query which are total product list, in the left outer new columns gets added to the first query and in the        left-anti, rows get deleted from the first table.

# 15. append queries
when we merge (based on our current knowledge), we either add a column or remove a row, for adding new e.g. products to our column i.e. new rows, we use appending queries.

the way it works is, it checks the second query headers with every single headers of first query if they match, it adds the data of that column from second query to the specific column from first query, it we have headers from second query that doesn't exist in first query, they get added to the first query as a new column while the value for the first column data in the new column is null and for the recently added data from second query can be anything because they do exist in the second query. 

and for columns that exist in the first query and not in the second query, the value for second query appended value will be null.

path to appending queries option:

home -> combine -> append queries.
# 16. different date regions and issues with type changing
if our power bi or excel regional setting set in UK, our date format will be MMM/DDD/YYY, and for example if we have a date in us format which is DDD/MMM/YYY like 24/1/2020 and if the type of this data is text or any at first and then we want to change it to date, we will confront an error because this date has no meaning in UK format version and we have to tell them that these date are in US version, so if we want to tell this is a date, when we want to change type, we select locale data type and we select date as type and united states as our locale to say that's our date in united states format unlike the application system setting which is united kingdom. 

# 17. fill

if we have empty cells (null) in our column, we can use fill to give them same value of their top cell or bottom cell which has a non-empty value.

fill down: takes the top cell non-empty value and give it to bottom empty cells.

fill up: takes the bottom cell non-empty value and give it to top empty cells.

path to fill:
transform -> any column -> fill

# 18. grouping column in power query

we can group our columns in power query, I couldn't find any specific application for it in power bi but it's quite useful in excel for visualization.

so what's grouping? imagine we have a name column and income column, some names appear multiple time, when we want to create a visualization for it in excel, unlike power bi, it relates each name to each number and it doesn't calculate same name income aggregation, so we have to either use complex formulas to create such a list for better visualization ( I think it's not even possible with excel functions) or we can use power query grouping feature, after we loaded our data, we navigate to home -> transform -> group by, after that a modal pops up, in that modal 
the single top blank is for grouping and it's like x-axis concept we had in power bi (the sorting and categorization is same) and by clicking the advanced option, we can have multiple x-axis and the column below is like creating a new column as y-axis based on categorization of our x-axis.

then we can import our newly created table to excel to use it for a better visualization with some of income of each person like what we had in power bi.

the issue that excel charts have is it doesn't have sum of y-axis and x-axis single appearance system and it just considers everything as a data and display it even the duplicate categories, that's why we use grouping and therefore their legends system is a bit different than power bi, same output but different approaches. 

so even for small range of data it's better to use power bi for visualization because of it's better system but if you wanted to have data entry feature along side of a accurate visualization, use power query to group your data and then visualize because any approach except this, ends up in non-sense charts.

all the benefits I said for grouping and visualization in excel can be done with power pivot charts and legend and chart style is exactly like power bi, so if your problem is visualization just use power pivot but if you need that type of data that grouping provides for data entry use, grouping, since power pivot table is not suitable for data entry.

use power pivot table charts for visualization and we know for some charts, we can't use power pivot data, we copy power pivot data and create chart for them and we know some charts features are limited in excel like drill down option we have in funnels in power bi, we don't have in excel and sometimes we can't have our desired table with excel pivot table charts or other charts, so we have to use power bi.

therefore, for small range of data use excel and power pivot table charts, if power pivot doesn't support your chart, copy the data and create a chart based on the data and if you have problem with excel data in any o cases, you have to use power bi even if you care about data entry option, and for small range of data don't worry about normalization in power bi, no normalization won't make a problem in small range of data.

count rows option gets calculated based on the occurrences of the group column value.
# 19. refreshing after data modification in power query

after we applied changes on our data in power query, we need to click close and load in power query, normally it should load our changes to our excel worksheet but it seems it's not like this always, so we have to press data -> queries and connections -> refresh all, so whenever you make a modification in power query and you want to load that into excel, press refresh all in excel for assurance.

when you want to make a change in data of an existing table in power query, you should make a change in the worksheet that was imported to power query and created that table and making any change on the output of that existing table worksheet in excel doesn't make any difference in power query.

# 20. conditional columns

you can create conditional columns based on other columns values, for using it navigate to 

add column -> general -> conditional column  

at the end, features like merging, appending and unpivoting and some other features like grouping can be useful in excel which we can't do with excel itself and in power bi.

actions like conditional columns and removing rows is something we can do in excel and may not be that practical and may be they are useful in power bi ( even conditional columns is possible with DAX)

# 21. what's application of unpivoting in power query?

Unpivoting in Power Query transforms data from a "wide" format (where categories are columns) to a "long" format (where categories become rows).

**Key Applications:**

*   **Easier Analysis:** Makes data suitable for PivotTables, charts, and aggregations (like summing values per category).
*   **Data Modeling:** Prepares data for BI tools (like Power BI) and machine learning models that prefer row-based data.
*   **Consolidation:** Standardizes data when combining sources with varying column structures.

Essentially, it makes your data more flexible and easier to work with for reporting and analysis.

# 22. what's application of left-anti merging in power query?

In Power Query, **Left Anti Merge** is a type of merge operation used to find and keep only the rows from the **left** table that **do not have a match** in the **right** table, based on specified join columns.

Here are its main applications:

---

### **1. Finding Unique or Missing Records**

*   **Scenario:** You have two lists of items (e.g., customers, products, orders) and you want to identify items that are present in the first list but missing from the second.
*   **Application:** A Left Anti Merge will return only those rows from your primary (left) table that have no corresponding entry in your secondary (right) table. This is perfect for identifying:
    *   Customers who haven't placed an order.
    *   Products that exist in your inventory but haven't been sold.
    *   Records in a new data extract that are not yet present in your master database.

---

### **2. Data Validation and Auditing**

*   **Scenario:** You need to ensure consistency between two datasets, perhaps a source system and a target system, or a staging table and a final table.
*   **Application:** By performing a Left Anti Merge, you can pinpoint discrepancies. If the merge operation returns any rows, it means those rows from the left table are not accounted for in the right table, indicating a potential data integrity issue or a record that needs attention.

---

### **3. Identifying Gaps or Exclusions**

*   **Scenario:** You might have a list of all possible items and another list of items that have been processed or approved. You want to know which ones are still pending.
*   **Application:** Merge the "all items" table (left) with the "processed items" table (right) using a Left Anti Join. The result will be the list of items that are still pending processing.

---

### **How it works in Power Query:**

1.  **Select Tables:** You choose your primary (left) table and the secondary (right) table.
2.  **Select Join Columns:** You specify the column(s) that contain matching values between the two tables (e.g., `CustomerID`, `ProductID`).
3.  **Choose Merge Kind:** Select "Left Anti" as the merge kind.
4.  **Result:** Power Query outputs a new table containing only those rows from the left table for which no match was found in the right table based on the selected join columns.

---

**In essence:** A Left Anti Merge is your go-to tool in Power Query when you need to answer the question: "What data exists in Table A that is *not* in Table B?"

# 23. what's the application of fill in power query?

In Power Query, the "Fill" operation is primarily used to handle **"sticky" or "waterfall" data** within a table, often seen in financial reports, multi-level groupings, or hierarchical data. It propagates the last non-null value downwards or upwards to fill in blank cells.

Here are the main applications:

---

### **1. Restoring Hierarchical or Grouped Data**

*   **Scenario:** Imagine a sales report where region names (e.g., "North", "South") are listed only once at the top of a group, and subsequent rows under that region have blank cells in the region column until a new region is introduced.
*   **Application:** Using "Fill Down" on the region column will copy the region name to all the blank rows beneath it, effectively associating each sales record with its correct region. This makes the data "flat" and suitable for analysis, filtering, and aggregation. The same logic applies to other hierarchical identifiers like departments, product categories, or project names.

---

### **2. Handling Missing Values in Sequential Data**

*   **Scenario:** You might have data where a certain attribute (like a status, a date, or a code) is only updated when it changes. Intermediate records might have blank values for that attribute.
*   **Application:** "Fill Down" can populate these blanks with the most recent known value, ensuring each row has a complete set of attributes based on the last known state. This is useful for tracking changes over time or filling in information that remains constant for a period.

---

### **3. Preparing Data for Analysis and Reporting**

*   **Scenario:** Many analytical tools and functions (like PivotTables, SQL queries, or some charting libraries) require complete data. Blank cells can cause errors or misinterpretations.
*   **Application:** By filling down (or sometimes "Fill Up", though less common for this use case), you ensure that every row has a value for the critical columns, making the dataset ready for further processing, summarization, and visualization without data gaps.

---

### **How it works in Power Query:**

1.  **Select Column:** You select the column containing the blank cells you want to fill.
2.  **Choose Direction:**
    *   **Fill Down:** Propagates the last non-blank value from above into the blank cells below it. This is the most common usage.
    *   **Fill Up:** Propagates the first non-blank value from below into the blank cells above it.
3.  **Apply:** Power Query applies the fill operation, creating a new step in your query.

---

In summary, the "Fill" operation in Power Query is essential for transforming messy, grouped, or sequentially reported data into a clean, structured format where each record is fully defined by the relevant attributes.

the first reason is the most useful application.

# 24. for combining files from a folder in power query, should header names be same? I think we combine sheets when we know they share similar columns like sales report of a product through different years or sales report from different products?

That's a great question, and you've hit on a key point about combining files in Power Query!

**Yes, for the most straightforward and reliable "Combine Files" operation in Power Query, the header names (column names) should ideally be the same across all the files you want to combine.**

Here's why and how it works:

### Why Identical Headers Matter

When you use the "Combine Files" feature (often found under "Get Data" > "From File" > "From Folder"), Power Query essentially does the following:

1.  **Connects to the Folder:** It lists all the files within the specified folder.
2.  **Previews a Sample File:** It takes one file as a template (usually the first one).
3.  **Transforms the Sample File:** It applies a set of transformation steps (defined in a "Sample Query" or "Transform Sample File" function) to this one file. These steps typically include extracting the content, promoting headers, and any other cleaning you do.
4.  **Applies Transformations to All Files:** It then applies these *exact same* transformations to *every other file* in the folder.
5.  **Appends Results:** Finally, it combines the transformed content of all files into a single table.

If the header names differ:

*   **Mismatched Columns:** Power Query will try to append columns based on their names. If File A has a column named "Sales Amount" and File B has "Revenue", Power Query will treat these as two separate columns during the append step, leading to incomplete data in each.
*   **Errors:** In some cases, significant header differences can lead to errors during the transformation of individual files.

### Your Examples are Perfect!

You're absolutely right with your examples:

*   **Sales Report by Year:** If you have "Sales_2021.xlsx", "Sales_2022.xlsx", and "Sales_2023.xlsx", and each has columns like `ProductID`, `ProductName`, `Quantity`, `Revenue`, Power Query will easily combine them.
*   **Sales Report by Product:** Similarly, if you have reports for "ProductA_Sales.csv", "ProductB_Sales.csv", etc., and they all share the same column structure (`Date`, `Region`, `UnitsSold`, `Price`), combining them is seamless.

### What if Headers Differ?

If your files have different headers but represent the *same kind of data*, you have a few options, but they require more manual work *before* or *during* the "Combine Files" process:

1.  **Clean Headers First:** Open each file individually (or use Power Query's advanced features) to rename the columns so they are consistent *before* combining.
2.  **Custom Transformation Function:** When Power Query prompts you to transform the sample file, you can build a more robust transformation function. This function can include steps to:
    *   Identify potential header variations.
    *   Rename columns to a standard set (e.g., mapping "Revenue" and "Sales Amount" both to "Total Sales").
    *   Handle missing columns gracefully.
    This is more advanced and requires careful M code writing.
3.  **Append Queries (Manual):** Instead of "Combine Files," you can import each file individually as a separate query, clean/standardize the columns in each query, and then use "Append Queries" to stack them together. This gives you maximum control but is more time-consuming for many files.

**In summary: For the automated "Combine Files" feature to work smoothly, aim for identical header names in all source files. If they differ, you'll need to standardize them first or use more advanced techniques.**

combining files of a folder are some sort of appending (not exactly appending but similar to it)

# 25. what's difference between excel ordinary charts and pivot table charts in application since pivot table chart give better and accurate results since it aggregate same name, values but in the ordinary charts, same name appears in the chart each time, like we want to check each person sales in each month and we have Kevin as a salesman, he will appear once in pivot table chart but it will appear multiple times in ordinary chart?

You've hit on a crucial distinction in how different chart types handle data aggregation, and your observation about PivotTable charts versus ordinary charts is spot on! Let's break down the differences in their application and why PivotTable charts often provide "better and accurate results" for certain types of analysis.

### Ordinary Charts (e.g., Excel Standard Charts)

*   **How they work:** Ordinary charts in Excel (like bar, line, pie, scatter plots) typically plot data directly from a source data range. Each row or data point in your source range is usually represented individually or as part of a series.
*   **Aggregation:** They **do not inherently aggregate data**. If you have multiple rows with the same value (like "Kevin" appearing multiple times for sales), the chart will plot *each instance* as a separate data point or bar, unless you manually aggregate the source data *before* creating the chart.
*   **Application:**
    *   **Detailed View:** Excellent for showing the raw data, individual transactions, or specific occurrences. If you need to see *every single sale* made by Kevin, including its specific date and amount, an ordinary chart plotting each transaction would be appropriate.
    *   **Trend over Time (Individual Events):** If you're tracking events over time and want to see the pattern of each event, even if they have the same label.
    *   **When Source Data is Already Aggregated:** If you've already performed a `SUMIFS` or `AVERAGEIFS` in your Excel sheet to aggregate sales per person per month, then an ordinary chart based on *that aggregated data* would work fine.

*   **Your Example:** If your source data looks like this:

    | Salesperson | Month | Sales |
    | :---------- | :---- | :---- |
    | Kevin       | Jan   | 100   |
    | Kevin       | Jan   | 150   |
    | Sarah       | Jan   | 200   |
    | Kevin       | Feb   | 120   |

    An ordinary chart plotting "Salesperson" on the category axis and "Sales" on the value axis would show "Kevin" multiple times (potentially as separate bars if plotted row-by-row, or it might average/sum them depending on how you set it up, but it won't automatically group identical salesperson entries). If you wanted to see *total* sales per person, you'd first need to create a summary table (perhaps using `SUMIFS`) before charting.

### PivotTable Charts

*   **How they work:** A PivotChart is intrinsically linked to a PivotTable. A PivotTable is a powerful data summarization tool that aggregates data from a source range or external data source. The PivotChart visualizes the aggregated data from its associated PivotTable.
*   **Aggregation:** This is their primary strength! PivotTables **automatically aggregate data** based on the fields you place in the Rows, Columns, Values, and Filters areas. When you place "Salesperson" in the Rows area and "Sales" in the Values area, the PivotTable automatically sums (or counts, averages, etc.) all sales for each unique salesperson.
*   **Application:**
    *   **Summarized Insights:** Ideal for quickly understanding high-level trends, totals, averages, and distributions across different categories.
    *   **Interactive Analysis:** PivotTables and PivotCharts are dynamic. You can easily rearrange fields (drag and drop), filter data, drill down into details, and change the aggregation method (e.g., from Sum to Average) to explore your data from multiple angles.
    *   **"Better and Accurate Results" for Aggregation:** As you noted, for questions like "What is the total sales for each person?" or "What is the average sale amount per product category?", PivotTable charts provide the accurate, aggregated view directly because that's what the PivotTable does by design.

*   **Your Example:** Using the same source data:

    | Salesperson | Month | Sales |
    | :---------- | :---- | :---- |
    | Kevin       | Jan   | 100   |
    | Kevin       | Jan   | 150   |
    | Sarah       | Jan   | 200   |
    | Kevin       | Feb   | 120   |

    If you create a PivotTable with "Salesperson" in Rows and "Sum of Sales" in Values, it will automatically produce:

    | Salesperson | Sum of Sales |
    | :---------- | :----------- |
    | Kevin       | 370          |
    | Sarah       | 200          |

    A PivotChart based on this PivotTable will then show "Kevin" once with a value of 370 and "Sarah" once with a value of 200. This is why you perceive it as giving "better and accurate results" for summary-type questions – because it's designed specifically for that.

### Key Differences Summarized

| Feature           | Ordinary Charts                                                            | PivotTable Charts                                       |
| :---------------- | :------------------------------------------------------------------------- | :------------------------------------------------------ |
| **Data Handling** | Plots raw or pre-aggregated data                                           | Aggregates data dynamically from a PivotTable           |
| **Aggregation**   | None by default; requires pre-aggregation                                  | Automatic and core functionality                        |
| **Data Points**   | Can show individual records; repeats labels                                | Shows aggregated summaries; unique labels per category  |
| **Interactivity** | Limited; based on source data changes                                      | High; can filter, sort, rearrange fields                |
| **Best For**      | Detailed views, specific event tracking, when source is already summarized | Summarized trends, comparisons, interactive exploration |
| **Accuracy**      | Accurate for raw data; requires manual summary for aggregated views        | Accurate for aggregated views (totals, averages, etc.)  |

**In essence:**

*   Use **ordinary charts** when you want to visualize the **individual data points** or when your source data is already summarized to the level you need.
*   Use **PivotTable charts** when you need to quickly explore, summarize, and visualize **aggregated data** across different categories, and benefit from interactive analysis.

Your intuition is correct: for the task of seeing *total* sales per person without repetition, the PivotTable chart is the superior and more direct tool because its underlying PivotTable handles the aggregation automatically.

we usually want to see the total values for analysis and if we want to check raw data we use data table itself for analysis, so we use ordinary table for charts when it has sum of data in itself otherwise we prefer the pivot table charts.


