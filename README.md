# An Analysis of ***kickstarter Campaigns with Excel***
## **Overview of Project**
This project is to analyze campain data with excel and display the trend how campain outcomes are influenced by variety of parameters.  
### **Purpose**
Analyze and visualize campaign outcomes (successful, failed, and canceled) for theater and plays based on launch date and goals, respectively. 
## **Analysis and Challenges**
### **Analysis of outcomes based on Launch date**
The campain outcomes (successful, failed, and canceled) for theater are analyzed and grouped in the launch month. The relationship between outcomes and lanuch month is displayed in pivot table and line chart. 
### **Analysis of outcomes based on Goals**
The campain outcomes (successful, failed, and canceled) for plays are analyzed and grouped in the category of dollar-amount ranges. The relationship between outcomes and dollar-amount ranges is displayed in a line chart. 
### **Challenges and Difficulties Encountered**
The campain outcomes for successful, failed, and canceled campain are selected using filter function from outcomes column. Results for theater only or plays only are shown using filter function in subcategory column. Pivot Table is established for theater outcomes by launch date and a line graph is generated to show their relationship. For the analysis of plays outcomes based on goals, percentage successful, failed and canceled campain are calculated in the ranges of dollar-amount, and a line chart is created to show their relationship. I encountered challenge when I tried to calculate the number successful, number failed and number canceled. Even though I filtered the outcomes column to show the successful, failed or canceled campain data only, but the calulated value by COUTIFS(kickstarter!D:D, "<1000", kickstarter!R:R, "plays") is still done based on the overall outcomes data, I solved problems by chaning the argument for COUNTIFS function to the new way: COUNTIFS(kickstarter!F:F, "successful", kickstarter!D:D, "<1000", kickstarter!R:R,"plays"). One more problem I encountered is when I tried to show the values on y-axis in % format. I solved problem by changing Format Cells into percentage.
## **Results**
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90361056/133930925-99869bf1-5016-4f2a-8965-695a157440e8.png)

-Two conclusions draw about the outcomes based on launch date: (1) the peak of the successful theater compain is around May. Theater compain is more successful in spring and summer season then in winter, probably more campain events can be hold when weather is nice. (2) the theater compain is not likely by canceled in any month during and never be canceled in Oct.

![Plays Outcomes_vs_Goals](https://user-images.githubusercontent.com/90361056/133930958-aa1805de-0deb-40b8-97c9-b0c99bb08696.png)
-The conclusion about the Outcomes based on Goals: plays compain is never been canceled and is most successful if the goal is in the dollar-amount range of<$5000. The outcomes turn out good also in the range of $35000-$44999.

-The limitations of this dataset: it doesn't show what kinds of factors influence the change of the outcomes. Such as in the data set for theater outcomes by lauch date. It looks that the successfu and failed campain follow the same trend. The number of successful increase only because there are more campain launched in the months of May and June, but it doesn't reflect how to increase the rate of successful.

-Some other possible tables and/or graphs that could be created: more factors can be added into the tables and chart, such as not only looking at the launch date but also considering the during of campain, to display how long the goal can be reached. And backers_count data migh be healpful to see how any people get involed, which can give some clue about the popularity of those campain in population. 
