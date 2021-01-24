# matplotlib-challenge

## Background
The purpose of this assignment was to evaluate the data from a recent animal study done by Pymaceuticals, Inc. The company's latest development is a new drug, Capomulin, designed to treat squamous cell carcinoma (SCC), a commonly occurring type of skin cancer. The purpose of this study was to compare the performance of Capomulin against other drug regimens.

Over the course of 45 days, 249 mice subjects were treated through a variety of drug regimens. The study was comprised of 249 mice subjects who had been identified with SCC tumor growth. Over the course of 45 days, the mice were treated through a variety of drug regimens. Tumor development was observed and measured over the study period.

## Raw Data
The raw data referenced and used for this analysis can be found in the 'data' file incuded with this submission. 

## Dataset Modifications
During the preliminary review of the study data, one duplicated mouse was identified. This mouse and all corresponding data was removed from the dataset and the final analysis is based on 248 mice subjects.

## Analysis
The following analysis was done and is included in the Jupyter notebook materials, file name 'main_matplotlib.ipynb:

* A summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.
* A bar plot using Pandas's DataFrame.plot() that shows the total number of measurements taken for each treatment regimen throughout the course of the study.
* A pie plot using Pandas's DataFrame.plot() that shows the distribution of female or male mice in the study.
* Calculations for the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.
* Calculations for the quartiles and IQR to quantitatively determine if there are any potential outliers across all four treatment regimens.
* Using Matplotlib, a box and whisker plot of the final tumor volume for all four treatment regimens was generated to show any outliers.
* Using one randomly chosen mouse that was treated with Capomulin, a line plot of tumor volume vs. time point for that mouse was generated.
* A scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen was generated.
* Calculations for the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment were unfortunately not able to be completed by the deadline of this assignment. The plot the linear regression model on top of the previous scatter plot was also not completed.
## Observations and Insights
Three observations that can be made from the data include:
1. The distribution between male and female mouse participants was essentially equal.
2. A subgroup of all Drug Regimens was used to calculate the final stats. This subgroup included the following regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. It is reasonable that these four regimens were selected for deeper analysis because they provide accurate sample representations of the full study data. Propriva is the only drug regimen that would not provide a strong representative sample of the data due to this regimen having significantly less measurements in comparison to the other nine regimens.
3. When evaluating the data of the four regimens, there was only one outlier, as shown by the dot outside of the boxplot fences for the drug regimen Infubinol. It would be reasonable to drop this mouse from the study data
