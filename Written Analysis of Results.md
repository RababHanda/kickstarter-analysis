# Kickstarting with Excel

## Overview of Project
The project looks at over 4000 campaigns and how each has fared. It utilizes the raw data, ranging from launch dates, funding goals, to countries, years etc, in order to analyse trends between different aspects of the campaigns. 
### Purpose
The purpose of this project is to exercise the different Excel tasks and strategies learned during the class for analyzing the outcomes of each campaign based on its launch date and the funding goals set for it. 

The project visualizes these relations to give an intrinsic understanding to the viewer. The visualizations designed to communicate a quick summary of trends in the outcomes of campaigns with respect to different aspects of its launch. 
## Analysis and Challenges
This sections breaks provides a detailed summary of the analysis performed in Excel comparing the outcomes of different campaigns to their launch dates or funding goals

Most commands needed to condense the data into a straightforward table were covered in class along with tasks to create different charts.
### Analysis of Outcomes Based on Launch Date

**This analysis examines the campaigns for Theater**

1. A new column to extract years from the entire launch date was created in the KickStarter sheet. The dates were already in **short date** format, so it was simple to use the **Year()** function by just adding the cell reference between the parantheses. This additiona column was added to make the filtering in the pivot table easy.

2. Next, a Pivot Table was created to filter all campaigns according the the *Parent Category* and the *Year* of the launch date. The *Outcomes* were added to the columns so the number of failed, canceled and successful could be easily reflected next to the date it launched on, therefore "Launch Dates" were input in the rows tab. Lastly the "Count of Outcomes" was added to the values tab to consolidate each outcome. Note that only months were kept in rows to classify launch dates into larger groups and see a higher level trend. The parent category was set to Theater to only analyze the trends for that media category.

3. Lastly, a line pivot chart with markers was created to represent the three different outcomes of the campaigns visually. Lines charts are best to represent a trendline over a span of time. The following chart shows how many of each outcomes occured from January to December across all years. 

![Theater Outcomes by Launch Dates ](/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

**This analysis examines the campaigns for Plays**

1. A new column was created in a new sheet within the same workbook with the fundraising goals grouped in increments of $5000 to combine extrememly varying sums of money into like categories. The outcomes were also regrouped as *Number Successful*, *Number Failed* and *Number Canceled*. The following function was used, with changes made to the criteria depending on what was being input into the columns: 
`=COUNTIFS(KickStarter!$F:$F, "SUCCESSFUL", KickStarter!$D:$D, "<1000",KickStarter!$R:$R,"PLAYS")`

2. Next, a *Total Projects* columns was populated for each fundraising goal category to eventually calculate the percentage of each of the aforementioned outcomes. The percentages were rounded off to 0 decimal places and were calculated using the formula: 
`=(B2/E2)*100`
Calculating the percentage of eacg outcome gives an overall picture of how the **Plays** campaigns fared overall, whether most were successes or failures or canceled. 

3. Lastly, a line chart was created to show the percentage of the outcomes changing as different fundraising goals were set. The following chart depicts the percentage trendline of the outcomes for different goal levels:

![Outcomes Based on Fundraising Goals](/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
As I have been using Excel extensively at my work for over 3 years, I faced no apparent technical issues since I am decently familiar with different functions in Excel. However, determining which column to assign to which of the categories of the pivot table took some practice. I needed to first develop an inherent understanding of what my pivot will summarize and somewhat mentally visualize how different aspects in rows/columns would change the summary of the table. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    - Highest number of successful Theater campaigns occur in the month of May across all years
    - The number of successful campaigns start reducing as the year ends, while the number of failed starts to increase during that time

- What can you conclude about the Outcomes based on Goals?
    - The percentage of successful outcomes reduces as the fundraising goal increases, while the reverse is true for failed campaigns (percentage increases as the goals increases)
    - 

- What are some limitations of this dataset?
    - 

- What are some other possible tables and/or graphs that we could create?
    - Tables and graphs could be created to study the outcome trends in different countries for different subcategories (perhaps theatres fare better in some countries over others, whereas movies fare better in some and not in others)
    - Another analysis can be performed on the outcomes based on how many backers each campaign had