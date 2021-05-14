# Trade and Labor, Ch. 14
John, Janet and Data for Development

Welcome to the Chapter 14 Data Module! Let's get started: 

**1. Download Tableau and Tableau Prep.** 
Go to https://www.tableau.com/academic/students. 
Use your .edu email to sign up for a year-long free account. 
Download Tableau Desktop and Tableau Builder Prep. 

**2. From our OSF project page, download the following files:** 
"Data Module, V3_Manuscript Only_210420.DOCX or .PDF"
"CountryRegion_ILO_210419.csv"
"InfEmp_ILO_210419.csv"
“Decent Work Workbook_210420.twbx”

**3. Open the "Data Module" file and follow the instructions to complete the data module assignment.**

Good Luck! Keep reading to learn more about this project below. 

# Abstract

The primary purpose of this chapter’s data work has been to understand the landscape of data related to decent work through (1) describing concepts related to these topics and how they are operationalized, (2) exploring the indicators and datasets covered in the accompanying chapter, (3) understanding the detailed metadata, data coverage and index constructions behind the commonly-used indicators, (4) identifying and bringing to light patterns and relationships in the data as means of testing theories related to our chapter’s key questions, and (5) effectively visualizing this data for comparison among countries and indicators. The result of these research efforts will be to create a data module which illustrates how concepts in trade and labor are operationalized and translated into data and indicators. This will shed light on the ways these data may be used and misused as a result. Though mentioned explicitly in the Sustainable Development Goals (SDG 8), the concept of “decent work” is abstract anda lacks conceptual clarity in development theory and practice. This results in a myriad of definitions and ways to measure decent work in both academic and “gray” literature. It’s linked to child labor, gender equity in the workforce and employment rates in the SDGs. In fact, there is no universally agreed upon indicator that points to whether countries are progressing toward this goal. This data module builds on this empirical work by asking what data is available that indicates whether work is “decent.” Without indicators to show the effects on workers of removing trade barriers, what data exists to test the assumptions embedded in trade as development?


**Files in this Github Repository:** 

*ILO Dataset: Global Employment Data*
  This dataset (available in Github or on Open Science Framework) is in two spreadsheets titled: InfEmp_ILO_210419.csv and CountryRegion_ILO210419. 
  Instructions for how to merge and clean these datasets are within our Data Module Manuscript, available on OSF (Ch14_Data_Module.docx).
*Workbook: Tableau, Part II of Data MOdule*
  The Tableau workbook (Decent Work Workbook_210420.twbx) is available here and in OSF, too! Download this to complete Part 2 of the Data Module for Chapter 14. 

#Want more information? The entire Data Module is copied and pasted here to make your life easier (in case you already have too many things downloading to bother). Good luck!

# Chapter 14: Connecting Free Trade and Decent Work (Data Module)

**Introduction:** In Chapter 14 of the Global Development textbook, we introduced a diverse set of labor measures used in the global development community, from free trade negotiators to Aid for Trade benefactors. Many of these measures, including unemployment, wages, child labor rates, and measures of social protections, are codified as key indicators in the United Nations’ Sustainable Development Goal 8. However, in Chapter 14 we make the case that a newer and lesser-known measure, informal employment, is a central indicator of decent work for actors in the international community. Informal employment intersects directly with free trade policies, which are often given the explicit goal of formalizing a country’s enterprises and economy. Informal employment intersects with “decent work” based primarily on its association with jobs that lack basic legal protections (e.g. work contracts, governmental protections) associated with good working conditions.  In this data module, we will dive into the International Labour Organization (ILO) datasets on all of these indicators. As you will see, informal employment data has strong correlations with many measures of decent work.

By the end of the module, you will have a stronger understanding of the data available on global informal employment and the relationship between informal employment and other measures of decent work. You will be equipped with new data processing, analysis, and visualization skills using Tableau Prep and Tableau. You will also be equipped to create your own independent analysis of informal employment data, describe the limitations and characteristics of this dataset as a proxy measure for “decent work,” and continue digging into the international labor data landscape on your own.

## Data Preparation, Analysis and Exploration

**Getting Started:** In this module, you will spend considerable time making charts and choosing which ones to use in a dashboard that visualizes informal employment. Here are a few tips to get you started: First, manage your time well. Try to complete this module in around 4 hours. It’s easy to get caught up in formatting when you’re working with data, so one tip is to focus on the big stuff (the right variables and visualization types) and leave the details (which are still important) until the end. Secondly, stay focused on learning. In every step of this module, and there are many steps, you will get more out of the work if you reflect on why you made the choices you did and evaluate how well your approach worked. Also, don’t worry about making your dashboard visuals perfect the first time. You can always return to it for this or future projects--we hope you find Tableau as interesting to tinker with as we do! 

Now, navigate to the Global Development Chapter 14: International Labor and Trade project folder in Open Science Framework. Under Files, navigate to Data Module Manuscript > OSF Storage (United States) > Data Module Downloads. Download everything in the Downloads folder into a unique folder on your local drive. Open the README.md file in OSF and follow the instructions. To prepare for Parts 1 and 2 of this data module, you will also need to download the software applications Tableau Prep and Tableau. Students with “.edu” email accounts will be able to get free access to this software for up to one year.

**Part 1:** Descriptive Analysis of Informal Employment
What can we learn about the state of informal employment in the world and general trends in the data over time? Chapters 9 and 14 of Global Development explain the differences between the informal economy and informal employment. In this section, we’ll explore whether measures of these two indicators display similar global trends. We’ll start by preparing a raw dataset for analysis and then create basic data visualizations, using the Tableau suite of tools. The data visualization that you will create is inspired by researchers characterizing a very similar dataset: the informal economy. Researchers with the International Monetary Fund published a series of papers based on a dataset they created to measure the “shadow economy,” i.e. the informal economy. 

In Part 1 of this module, you’ll re-create this chart (visible in the download of this module) using ILO data on informal employment, to compare the findings in the Medina and Schneider report with what the data say is happening with jobs. In Part 2, you’ll use the ILO data to compare informal employment rates with other proxy measures of decent work to determine the best proxy measure for labor to judge whether trade creates jobs that are decent. 

**1.1** First, we’ll clean and tidy data in Tableau Prep, as well as connect two datasets that will give us both country and world region information in our final table.

Open Tableau Prep. At the top of the left hand panel, you will see the title “Connections” and a button with the ‘+’ plus sign. Selecting that sign will bring up a menu of file and server types. We want to connect “To a File”, so select the “Text file” option (our .CSV files are considered text files). Now you will be prompted to browse your computer for the .CSV files you downloaded. Select the “CountryRegion_ILO_210419.CSV” file and click “Open.” Then, repeat this process and open the “InfEmp_ILO_210419.CSV” file. You now have two CSV datasets open in Tableau Prep, which you should see visually in the main field of the application (look for a colorful circle with a paper symbol and the name of the file). Go to File > Save and save this file (known as a “flow”) as “InfEmp_ILO_flow_YYMMDD” with the current date.

Next we will clean and tidy these two datasets. In the main/center field of the application, where you see visual representations of the two datasets, click the plus arrow for the CountryRegion dataset and select “Clean Step.” In the bottom panel, columns will appear that represent the columns, or “fields” in this dataset. We are going to remove some of these fields because they are not necessary for our analysis and can be confusing and take up space. The “ISO3 Code” field can be removed by navigating over its box and finding the three dots in the top right corner. Selecting this will reveal a drop-down menu where you will select “Remove.” Do the same for the field “Included in ILO estimates?”; we are not done cleaning this data, but we will return to it.

Next, open up a “Clean Step” for the InfEmp dataset. A lot of cleaning and tidying is needed here. In the same three dot dropdown menu, note the “Rename Field” function. Change field title “ref_area.label” to “country”, “classif1.label” to “economic_activity”, “time” to “year”, and “obs_value” to “inf_emp_rate”. Next, remove “.label” from the remaining field titles. In the “sex” field, rename the actual values (“Sex: Female”, “Sex: Male”, etc.) by right-clicking them and selecting “Edit Value”. Change these values by removing “Sex:” so they read only as “Female”, “Male”, etc. Finally, change the data type for the “year” field from Number to Date by selecting the # pound sign above the “year” field title and selecting “Date”.

Now we want to connect these two datasets, so that our observations in the informal employment dataset are not only by country, but also by ILO region and subregion. This will allow us to group countries by region in our visualizations. Click and drag the InfEmp “Clean 2” icon over the to CountryRegion “Clean 1” icon. You should see “Join” and “Union” options appear. Drop your selected icon over the “Join” option. A new icon should appear with lines connected to both of your clean datasets, called “Join 1”. In the bottom panel for Join 1, we have many new options. On the left side, you will see the “Applied Join Clause”. Tableau Prep likely already knew you wanted to join the datasets by “country”. If not, select the “country” field for both sides. Then, look for “Join Type: inner” and the associated Venn Diagram. Select the right side of the Venn Diagram such that the title now reads “Join Type: right”.

We know that the informal employment dataset doesn’t contain observations for every country in the CountryRegion dataset. However, we want to make sure that every country in the informal employment dataset is matched to their region information from the other table. We can check this by looking at the “Join Clauses” field, by checking the white box next to “Show only mismatched values.” We see for “Clean 1” that there are many countries without any data, which we expected (these are countries without any informal employment data). For “Clean 2” however, we see that Côte d'Ivoire and North Macedonia are not matched. What is the problem? Find Côte d'Ivoire in the “Clean 1” column. You’ll notice that the CountryRegion dataset contains an error: Côte d'Ivoire is “C?te d’Ivoire”. Double click on the incorrect spelling to fix it (You can double click on “Côte d'Ivoire” and copy and paste the correct spelling if you don’t have easy access to a “ô” on your keyboard). For North Macedonia we have a similar problem, it is “Macedonia, the former Yugoslav Republic of” in the Clean 1 list. Change this to “North Macedonia” (the updated name). Your unmatched “Clean 2” countries are now matched!

The final step is to create an output for our cleaned, tidied, and joined dataset. Select the +plus button the right of the “Join 1” icon, and select “Output”. An Output icon will appear. In the bottom panel, change the Output type from “Tableau Data Extract (.hyper)” to “Comma Separated Values (.csv)”. Change the name of your output to “InfEmp_CountryRegion_join_YYMMDD”. Click the “Browse” button under “Save output to” and find your save folder for this assignment. Finally, click “Run Flow”. You have now created your CSV file! Be sure to save your Tableau Prep file and then exit.

**1.2** Using our cleaned .csv file, now we’ll explore ways to visualize this data in Tableau. You will create three visualizations of the informal employment dataset that will characterize recent trends in the data and visualize the availability of this data around the world. 

Open a new workbook in Tableau (opening the application will automatically bring you to a new workbook). Go to Data>New Data Source, and again select “Text file”. Navigate to your project folder and open the cleaned “InfEmp_CountryRegion_join_YYMMDD.csv” file you just created. The dataset will open in the “Data Source” view, which you can see as a tab in the bottom left corner of the window. Review the dataset in this tab to confirm that it is the clean data you created. In the top right area where you see “Connection”, change the connection from “Live” to “Extract”, which will save this version of your dataset in your workbook file. Finally, save your file as a .TWBX “packaged workbook” to allow others to open your workbook and view your data. Using our naming convention and save this file as Part1_Workbook_YYMMDD. You are now ready to create data visualizations!

The first visualization you will create is a global informal employment bar chart, organized by region and years. This visualization will parallel the chart from Figure 1 on the informal economy, published to the IMF blog in 2019. Notice that this bar chart does not show informal employment by year, but rather by groups of years (e.g. 1991-1999). You will need to do additional data work to create the same visualization.

Navigate to Sheet 1. In the left hand panel, you will see a column list of fields from your dataset. Click and drag the “ILO_Region” field into the “Columns” bar near the top center of the screen. Next click and drag the “Year” field into the same “Columns” bar. Finally, click and drag the “inf_emp_rate” field into the “Rows” bar. This “inf_emp_rate” field will appear in green, and automatically appear as “SUM(inf_emp_rate). We don’t want the sum, we want an average. Right click on the field in the “Rows” bar and navigate to Measure>Average. Next, we want to change our visualization to a Side by Side Bar Chart. In the top right of the window, click on “Show Me” and click on the vertical bar chart icon. You are starting to see progress!

Now we want our data to be colored by region, so click and drag the “ILO_Region” field from the left hand panel over to the next panel where you see the “Marks” box, and drop the field in the “Color” tile with 4 colorful circles inside. Each regional section of the chart should now be a unique color.

Next, we need to make sure we are visualizing the correct informal employment averages! For every year in our dataset, we know that we have informal employment rates delineated by the “sex” and “economic_activity” fields. All of these rows are being averaged together, skewing our measure. We can solve this by filtering out all rows except for “sex” = “total” and “economic_activity” = “total”. Click and drag the “sex” and “economic_activity” fields from the left hand panel into the “Filters” panel. Each time, a window will open asking you what you want to filter. Check only the boxes labeled “Total” and select OK. Almost done!

The remaining issue with your visualization is that it is too busy. We do not want a datapoint for every year. To create buckets of years, we will need to create a new field. In the left hand panel, right click the “year” field and select Create>Group. A window will pop up with all of the observations (years) in the “year” field. Using either the CTRL or Shift key, select the most recent four years (1/1/2020 through 1/1/2017) and click “Group”. Make the group title “2017-2020”. Create 5 total groups this way for the years 2001-2020. For the Field Name at the top of the window, call this field “year_buckets”. Finally, select “OK”. You have created a new field! Click and drag this new field from the left hand panel over the the “Columns” bar and replace the “year” field here with the “year_buckets” field. We want to filter out all of the years and buckets except for the 3 most recent buckets. Click and drag the “year_buckets” field into the filters window and select only 2009-2012, 2013-2016, and 2017-2020.

Give you visualization a title: “Global Informal Employment” and update the sheet name to be the same. If the year buckets at the bottom of your visualization are oriented horizontally, right click on the x-axis and select “Rotate label”. Does your chart look like this? Be sure you are saving!

Conduct some preliminary visual analysis of your bar chart, and keep the IMF blog chart on the informal economy for comparison. Answer the following questions:
  1. What’s the key takeaway or pattern/trend you notice in the IMF blog chart on the informal economy?
  2. Do we see similar trends in the informal employment data based on the visualization you created? What other trends do you identify that are unique to the informal employment chart? Note that the two charts cover very different time periods. How might they fit together?
  3. Does adding the 2 additional buckets you created change your analysis? What other changes can you imagine making that might alter the analysis and how? (e.g. to years, to the sex and economic activity filters, to the regional/country-level organization).

**1.3** In the final section of this part of the data module, we want to peel back the layers of data that go into this relatively simple, high-level Global Informal Employment chart that you created. What is this visualization (1.A.) not showing us? By aggregating our observations into averages by years and regions, what data issues are we obscuring? We don’t need to do any more data processing! We will simply make two new visualizations with the same data, in the same workbook.

**Creating a world map.**
First, we will create a world map of our data that communicates the coverage (geographical) and frequency (time) of reporting on informal employment. At the bottom of your workbook window, find the tab to create a “New Worksheet”. This will open up a blank sheet. This time, click and drag the “Latitude (generated)” field from the bottom of the left hand panel over to the “Rows” bar. Drag the “Longitude (generated)” field to the “Columns” bar. You now have a blank world map.

We can visualize the countries in our dataset by dragging the “country” field into the Marks>Detail button. Now all the countries with data in the dataset contain a dot. We want to visualize the amount of data each country is reporting, and we can do that with color. Drag the “inf_emp_rate” field to the Marks>Color button. Where this field appears in the Marks panel, right click and change the Measure to “Count”. Finally, we again want to filter out all of the observations for a given year except for “sex” = “total” and “economic_activity” = “total”. Repeat this step from 1.2(G)(c). Now we have a completed visualization, showing a map of all the years of observations in our dataset by country! The darker the country, the more years of reporting that country has for informal employment. Title this chart “Global Informal Employment Coverage” and update the sheet name.

**Creating a time series bar chart.** 
For this visualization, we want to keep the filters we used for our map. Duplicate the map worksheet by right-clicking on the map tab and selecting “Duplicate”. In this new sheet, remove the “Latitude” and “Longitude” fields from the Columns and Rows bars by clicking them and dragging them off screen. Now drag the “year” field into the Columns bar. Drag the “ILO Subregion - Broad” field into the Rows bar, and then the “inf_emp_rate” field into the Rows bar to the right of the previous field. Change the “inf_emp_rate” from “Sum” to “Count”.

Change the coloring of your chart by dragging the “ILO Subregion - Broad” field into the Marks>Color button. You can then sort the subregions by which one has the most observations by right clicking on the “ILO Subregion - Broad” field in the Rows bar and selecting “Sort”. In the pop-up window, select Sort by “Field”, Sort Order “Descending”, Field Name “inf_emp_rate”, and Aggregation “Count”. Exit the window. Because the “country” field should still be in the Marks panel, listed as a “Detail” field, you should be able to hover over your bars and see the specific country each observation belongs to. Does your visualization look like this?

Reflecting on the two visualizations you just created, provide analysis on the following questions:
  1. Observing the coverage of the informal employment dataset as visualized by the map, what do you notice as global trends? What countries are reporting data, and which are not? What countries appear to be providing far more data than any others, or any of their neighbors?
  2. Using your second visualization, are the trends you observed in the map confirmed by the bar chart? What regions have the most coverage? Also, what do you observe about the years of reporting, and the change in reporting over time?
  3. Reflect on your analysis from Part 1.2., are the differences in data coverage by region reflected at all in the IMF blog-style bar chart you created and analyzed? What might an audience of the Part 1.2 bar chart assume about data coverage between regions?
  4. How does data quality affect or change your assessment and comparison of informal economy/jobs charts? Do you still think the Part 1.2 bar chart is a useful visualization of this dataset?

**Additional work:** how could you effectively visualize data deprivations while communicating the existing data on informal employment? Consider trying to use color or size options to visualize both the average and the count of “inf_emp_rate”!


**Part 2. Exploring the relationships between informal employment data and other proxy measures of decent work**
In this section, we’ll create a series of similar charts (scatterplots) that compare indicators often used as proxy measures for decent work with data on informal employment that you explored in Part 1.

You will not use the workbook you created in the first part of the data module. Instead, we have provided a workbook with our version of the visualization you created in Part 1, in addition to a host of new, connected datasets on decent work. You should have already downloaded this workbook (“Decent Work Workbook_210419.TWBX”) from OSF after following the README.txt. Open this workbook in Tableau and right click on the data to explore. When you’re familiar with what’s included in this workbook, proceed to the next step of exploring proxy variables for different work including: Unemployment, Wages, Social Protections and Child Labor. Once you’ve created four scatterplots that visualize these measures, your final task will be to create a dashboard for further exploration. 

Remember, data visualization is about choices, and there’s no perfect way to visualize data! Kirk (2019) writes that good data visualizations are (1) trustworthy (they don’t mislead the viewer through confusing graphics or intentional changes), (2) accessible (they aren’t overly complicated to a reasonable person) and (3) elegant (they look appealing; people want to stop and stare). In this part of the module, focus on making your visualizations meet these metrics. 

**2.1** Classic unemployment rate and informal employment rate: Create a scatterplot of informal employment and unemployment, including a trend line. What do you notice about the relationship between informal employment and unemployment data?

Drag [unemployment rate] to the rows shelf and select “average” for aggregation measure. Drag [informal employment rate] to columns and select “average” for aggregation measure again. This averages the data across all years. You’re working with percentages so ensure that both axes show % before moving on. (Hint: click “format” on both measures to change the numbers to percentages.) You should automatically see a single dot in the top right hand corner of your scatterplot. 

Drag [country] to ‘detail’ on the Marks tab. You should see a bunch of dots appear on your plot. If a small gray button appears that says ‘# null” on the bottom right hand corner of your plot, click it and explore the null data. Based on the information you see classified as ‘null,’ you can decide to filter, edit or show the null data at its default position. 

Right now, your chart shows data for all years of reporting (average) by country in addition to all types of economic activity for all ages and both men and women. How can you tell if you’ve got duplicate data in this view? By creating filters: To create an accurate view of your data, drag [sex] to the filters tab and select ‘Total’ only. Drag [economic activity] to your filters tab and select ‘Total’ again. You can right click on these dimensions in the Filters card to display the filters and give your view the option to display this data, but setting “total” as default will prevent misleading first-looks at this chart. Do the same with age, selecting an appropriate category that gives your viewers the most accurate view at first look. 

Right click to edit both the y and x axis. Change the axis titles to something that makes sense to you and un-click ‘Show zero’’ to see what happens.

Format the chart. Here’s the way to make it look like our example: [requires download]

Change ‘Shape’ in the Marks card to filled-in circles. Click on ‘Color’ in the Marks card to make your countries all the same color. 

Change the size and shape of the chart by clicking ‘Format’ > ‘Cell size’ in the toolbar and making the view smaller, wider, etc. 

Change the font size and grid lines in the Format tab to make the chart as simple as possible. What’s the key message you want your viewer to take from this chart? 

Finally, add a trend line to the chart to view statistical analysis of this data. Select ‘Analytics’ from the Data pane on the left hand side of your workbook. Drag ‘Trend line’ to your view. Select a trend line and explore the different options to analyze this data. Right click on the line to display statistical analysis including the p-value of this correlation and the r-squared value. What can you tell about the relationship between unemployment and informal employment data from this view? 

Give your chart a name that presents your primary takeaway. What’s the most important message this chart communicates to your audience? 

**2.2** Informal Employment and Wages: Are wages higher or lower in countries with more informal jobs? Create a scatterplot just like the one you made for unemployment, this time comparing wages with informal employment rates. The goals here are to create similar visualizations you can use to frequently-used proxy variables for decent work to informal employment. Start by completing each chart. If you want to get creative, do so in the dashboard once you’ve built the basic charts. 

Now create a similar chart using what you learned in 2.1 to compare median monthly wages (in purchasing power-adjusted 2017 US dollars) to informal employment rates by country. 
Make changes to this chart’s formatting, display disaggregated or explore other options in the ‘Analytics’ tab. Give your chart a title that summarizes your findings. 

**2.3** Informal Employment and social protections: Does informality correspond to the level of social protections in countries? 

Create a chart that compares these two data points. Don’t worry: A scatterplot is fine. The goal is to see a relationship--not to make an innovative chart...yet. 
This time, see if you can color code regions based on income ranking by the World Bank. What’s the pattern you see in this chart? 

**2.4** Informal Employment and Child Labor: Social protections in Western democracies include bans on people under a certain age holding jobs. But what happens in informal jobs? Is child labor more common in countries with higher informal employment? 

Create a final chart that compares informal employment with child labor rates (“average child economic activity” in this dataset refers to the percentage of kids, by age and sex, who are engaged in productive economic activity, i.e.”work.”) Don’t forget to include options for viewers to filter by age and sex. 

**2.5** Put it all together: Create a dashboard using the charts you’ve made in Part 2b - 2e so you can visually see how these measures compare.  

Create a new dashboard. Choose ‘Floating’ in the Objects Panel and drag “Global Informal Employment” (the first chart in this workbook from Part 1) to the dash. Select ‘Fit’ > ‘Entire View’ and expand this bar chart to show the data clearly. Make sure to keep your objects “floating,” at least in the beginning as you experiment with displaying charts in this dashboard.

Now experiment with adding the four charts you created in Part 2 to this dashboard. Pick two that clearly communicate the story you want to tell about informal employment. Adjust the formatting of charts and display options to make sure the data is clear. Give your dashboard a title and experiment with adding filter or highlighting actions by clicking ‘Dashboard’ > ‘Actions’ in the toolbar. Then answer the following questions. 

**Module Discussion Questions:** 
  1. How does what you explored in Part 1 regarding the quality and coverage of reporting on informal employment affect your interpretation of the proxy measures you compared to informal employment rates in Part 2? Data analysts and policy professionals often must “make do” with existing data just like this. What are some ways you could provide context to viewers of your final dashboard regarding the availability of data on informal employment? 
  2. Take a moment to explore the dashboard you created. Given the positive assumptions we make about low unemployment, how does its association with high informal employment challenge that view? What do we notice happening to wages and social protections as informal employment rates go up? Why do you think this happens? Does looking at these charts together provide any new insights into the value of informal employment as an appropriate measure of decent work? What about unemployment data? 
  3. What are some other characteristics of countries or domestic labor markets/economies that might explain these strong correlative relationships? (e.g. strong institutions, consider adding social protection measure)
  4. Does your data work in this module, including the visualizations you created, support treating informal employment as a proxy for decent work? Why or why not? 
What other measures or data would we need to create an indicator for decent work?

 
