# Matplotlib Homework - The Power of Plots

## Background

What good is data without a good plot to tell the story?


The purpose of this data analysis is to demonstrate different plots charts using pandas and Matplotlib based on the following criteria:

Pymaceuticals specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer. In this study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. You have been tasked by the executive team to generate all of the tables and figures needed for the technical report of the study. The executive team also has asked for a top-level summary of the study results.

## Steps

* There are two csv files for the data analysis. I used `pd.merge()` method. The file names are [Mouse_metadata.csv](Pymaceuticals/data/Mouse_metadata.csv) and [Study_results.csv](Pymaceuticals/data/Study_results.csv)

* During the analysis, there was one mouse identified ('g989') which had a duplicate record. It was excluded from the combined data which made total of 248 mice for the analysis.

* In the analysis, We have showed different types of plots using both pandas `DataFrame.plot()` and Matplotlib's `pyplot()`. The bar plots shows total number of mice used for treatment regimen. The pie bar shows the gender grouping of the mice used for the analysis.

* Calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Calculated the quartiles and IQR and quantitatively determine and outlier were identified.

* Using Matplotlib, generated a box and whisker plot of the final tumor volume for all four treatment regimens and highlighted the potential outliers in the plot.

* Randomly selected a mouse l509 that was treated with Capomulin. Created the scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

* Lastly, calculated the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. The plot demonstrated the results of recreating the previous scatter plot and placing the linear regression model on the top. 


# Observations and Insights

* The Study shows they had examined and sample of 249 mice. One mouse had duplicated data which was excluded. The analysis shows that there were 49.0% Female and 51.0% male.

* The correlation between Mouse Wegith (g) and Average Tumor Volume is 0.84. This number shows strong positive correlations which shows that when the mouse weight increases the average tumor volume also increases.

* From the selected four treatments, Capomulin and Ramicane reduces the size of tumors better than other two treatments.

* Out of 10 treatment regimens used for the animal study but only four treament were identified as promising treatments. They are Capomulin, Ramicane, Infubinol, and Ceftamin.

* The regression analysis help us understand to show how much the average of tumor volume will change when the weight of the mic change.