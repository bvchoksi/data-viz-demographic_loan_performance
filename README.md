###Summary

My data visualization analyzes Prosper's peer-to-peer loan data and presents a story
about the performance of loans by various demographic indicators.

A comparison of good and bad loans is presented for 9 different demographic indicators, 
such as Credit Score, Employment Status, Debt-to-Income Ratio, and Income.

Prosper investors, or even other private lenders, can then use demographic indicators 
they deem important in setting a criteria to select a borrower.

###Design

The design was done exclusively in RStudio, because deep analysis was necessary to 
explore and transform the Prosper data set that contained 81 columns of information for 
over 100,000 loans.

The complete analysis, cleansing and transformation of data to be 
used for data visualization is included in the following files - analysis_etl.Rmd and 
analysis_etl.html.

Only loan status and borrowers' demographic attributes were considered for analysis. 
Unusable data was cleansed. The multiple loan statuses were condensed into meaningful 
categories. The demographic columns were also condensed or binned into categories to make 
the data visualization easier to understand.

From the outset, I considered a stacked bar chart as the correct form of visualization 
for the information I wanted to convey. A stacked bar chart could meaningfully portray 
good and bad loans as percentages in each category, while also indicating trends if any. 

A colorblind-safe and diverging color palette from ColorBrewer was chosen to portray good 
and bad loans. The transformed data was then plotted in R to gather feedback.

###Feedback

I elicited feedback throughout the design process from my wife Bijal who is a CPA, and 
brothers Rohan and Aditya who are businessmen/investors.

I had originally included the borrower's residential state in my R draft plots. The 
feedback I received from Rohan was that geography was too broad an indicator, and not 
useful.

The condensing and binning of demographic values into categories were vetted with all
three. Almost 70 occupations were condensed into just 4 skill levels with the help of 
Bijal's feedback.

The colors chosen to denote good and bad loans were found to be intuitive by all.

In R, only percentages of good and bad loans were plotted. However, as per the feedback
I received from Aditya, the quantum of loans in each category would be useful to assign 
a weight to each category. The quantum of loans would also help in knowing the decisions 
other investors are making in terms of avoiding borrowers in certain categories. Quantum 
of loans were indicated in the final data visualization created using Dimple.js and D3.

I experimented with line and bubble charts to see if it could better highlight trends, 
but it was found to be confusing by all as compared to the stacked bar charts.

Bijal recommended notes to draw attention to patterns or trends that would ensure the 
information meant to be conveyed is absorbed by the viewer. Annotations were added to 
the charts.

Andrew, the first reviewer made good suggestions that have been incorporated in this 
submission. The initial data viz straddled the explanatory-exploratory border. This 
version has a clearer narrative that I am driving.

###Resources

- http://dimplejs.org
- https://github.com/PMSI-AlignAlytics/dimple/wiki
- http://bost.ocks.org/mike/
- https://github.com/mbostock/d3/wiki/API-Reference
- http://stackoverflow.com
- http://www.sitepoint.com/create-data-visualizations-javascript-dimple-d3/








