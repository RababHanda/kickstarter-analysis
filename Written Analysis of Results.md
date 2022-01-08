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
1. A new column to extract years from the entire launch date was created in the KickStarter sheet. The dates were already in **short date** format, so it was simple to use the **Year()** function by just adding the cell reference between the parantheses. This additiona column was added to make the filtering in the pivot table easy.

2. Next, a Pivot Table was created to filter all campaigns according the the *Parent Category* and the *Year* of the launch date. The *Outcomes* were added to the columns so the number of failed, canceled and successful could be easily reflected next to the date it launched on, therefore "Launch Dates" were input in the rows tab. Lastly the "Count of Outcomes" was added to the values tab to consolidate each outcome. Note that only months were kept in rows to classify launch dates into larger groups and see a higher level trend. The parent category was set to Theater to only analyze the trends for that media category.

3. Lastly, a line pivot chart with markers was created to represent the three different outcomes of the campaigns visually. Lines charts are best to represent a trendline over a span of time. The following chart shows how many of eahc outcomes were from January to December across all years. 

![Theater Outcomes by Launch Dates ](/Resources/Theater_Outcomes_vs_Launch.png)
### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
