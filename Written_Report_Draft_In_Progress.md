# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this project was to analyze various Kickstarter fundraising outcomes in relation to their launch dates and their funding goals, focusing specifically on theater plays. The client had already initiated a fundraising campaign for a theater play which appeared to come close to its target goal in a short amount of time.

## Analysis and Challenges

#### Dataset

The dataset was provided by the client in the form of a spreadsheet in an Excel Workbook.

#### Methods

Additional columns were added to the supplied spreadsheet to a) break out fundraising subcategories from parent categories, b) normalize timestamp information converting it to a date format, and c) extract the year that individual fundraising events occurred (see screenshot below for details). These were needed to complete the analysis. The other parts of the analysis, followed by a summary of challenges and difficulties encountered, are described in subsequent sections.

<insert screenshot of columns added>

### Analysis of Outcomes Based on Launch Date

The client requested an analysis of outcomes for the broader “theater” parent category relative to the time of year the fundraisers were launched. The client was interested in fundraising events that had already achieved an outcome (success, failure, or cancelation), so events that were still in progress were filtered out. A pivot table was created using certain selected fields to achieve this.  The screenshot below shows the pivot table fields selected. (Note that the outcomes were filtered as described above):

<insert pivot table field screenshot here>

The screenshot of the pivot table below shows the data collected based on the selected fields. (Note that there were no instances of cancelations in October for any year in the data range.):

<insert pivot table screenshot here>

Finally, a chart was prepared to give a visual representation of the data:

<insert Theater Outcomes by Launch Date here>

Note in the chart above that although successful and failed campaigns tended to rise and fall together both in the first few months of the year and the last few months of the year, the successful campaigns rose much higher in May than the failed ones, and even though the total number of successful campaigns began to fall after that, they still outpaced the failed ones by significantly higher margin in June and July before settling back a more typical distance above failed campaigns in August. In contrast, the number of failed campaigns was relatively even for May through July.

### Analysis of Outcomes Based on Goals

The client requested an analysis of campaign outcomes relative to the funding target of the campaigns and wanted to “drill down” to just the “plays” portion of the theater category for this investigation. To accomplish this, a table was created on a new spreadsheet in the workbook provided by the client as shown below. (Note that there were no theater plays canceled in any funding target range in this dataset. Also note that most data points are in funding goal ranges below $15,000, and the number of data points in funding goals categories above $25,000 appear by visual inspection to be insufficiently large enough to draw conclusions from, although no statistical analysis was undertaken to confirm this.):

<insert Outcomes Based on Goals table here>

A chart was prepared based on percentages calculated in the last three columns of the table described (and shown) above. The chart is shown below:

<insert Outcomes Based on Goals chart here>

In the chart above, the number of successful appears to gradually diminish starting from a high of almost 76 percent in the less than $1000 range and then slowly reducing to 45 percent in the $20,000 to $24,999 range. In higher funding ranges, the percentage values appear erratic. This could possibly be due to insufficient data available for these ranges.

### Challenges and Difficulties Encountered

There were several challenges in putting together the analysis. For the “theater outcome by launch date” analysis, getting the right placement in the pivot table fields proved tricky; placing the “Date Created Conversion” column in the “Rows” field solved the problem. Also, the anomaly of no data for canceled campaigns in October left a blank section in the chart. It was decided that this was tolerable based on the requirements. For the “outcomes based on goals” analysis, the COUNTIFS function was used, and determining the right three or four “criteria range, criteria” pairs per formula proved troublesome at first.

## Results

### Conclusions

#### Outcomes based on Launch Date

The best month to start a theater-related fundraising campaign appeared to be May followed by June and then July. The worst month to launch a campaign appeared to be December. Although it was not calculated, all months except December appeared to offer a 50% or better chance of success (by visual inspection).

#### Outcomes based on Goals

Lower fundraising goals for theater plays appeared to be both more popular choices and more successful. The $1,000 to $4,999 goal range had significantly more data points than any other range and was the second most successful (goals that were less than $1,00 had a slightly better outcome).

### Limitations

The data set only spanned campaigns over a three-year period. Since economic conditions change over time, a larger dataset spanning as increased number of years might be less susceptible to economic swings. Also, more recent data would be helpful.

Similarly, a larger dataset might increase confidence in analysis of fund raising involving larger goals.


### Further Work

Although it is uncertain if there is sufficient data for the analysis, comparing outcomes in different nations or locales might prove interesting. Also, the three years that the dataset spans could be compared with each other.




