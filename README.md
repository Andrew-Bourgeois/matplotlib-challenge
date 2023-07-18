# matplotlib-challenge
UNC-CH-DA - Module 5 - Matplotlib Challenge

**Instructions for Running Scripts:**
* Clone the repository to your local machine
* Ensure you cd into the /matplotlib-challenge directory, and use the **pymaceuticals_Bourgeois.ipynb** Jupyter Notebook.
* The 'Resources' folder containing the relevant csvs should also be located in the /matplotlib-challenge folder.

**BACKGROUND:** Pymaceuticals, Inc., is a new pharmaceutical company specializing in anti-cancer medications. Currently scanning for treatments for squamous cell carcinoma (SCC), a common skin cancer.

Using study of 249 SSC infected mice, given a range of drug treatments over 45 days, compare the performance of the drug Capomulin against other drugs.

Generate all tables and figures needed for a technical report and clinical study, and provide a top-level summary of the results for the executive team.

**REQUIREMENTS**
**Prepare the Data (20 points)**
    *  The datasets are merged into a single DataFrame. (6 points)
    *  The number of mice are shown from the merged DataFrame. (2 points)
    *  Each duplicate mice is found based on the Mouse ID and Timepoint. (6 points)
    *  A clean DataFrame is created with the dropped duplicate mice. (4 points)
    *  The number of mice are shown from the clean DataFrame. (2 points)

**Generate Summary Statistics (15 points)**
    *  The mean of the tumor volume for each regimen is calculated using groupby. (2 points)
    *  The median of the tumor volume for each regimen is calculated using groupby. (2 points)
    *  The variance of the tumor volume for each regimen is calculated using groupby. (2 points)
    *  The standard deviation of the tumor volume for each regimen is calculated using groupby. (2 points)
    *  The SEM of the tumor volume for each regimen is calculated using groupby. (2 points)
    *  A new DataFrame is created with using the summary statistics. (5 points)

**Create Bar Charts and Pie Charts (15 points)**
    *  A bar plot showing the total number of timepoints for all mice tested for each drug regimen using Pandas is generated. (4.5 points)
    *  A bar plot showing the total number of timepoints for all mice tested for each drug regimen using pyplot is generated. (4.5 points)
    *  A pie plot showing the distribution of female versus male mice using Pandas is generated. (3 points)
    *  A pie plot showing the distribution of female versus male mice using pyplot is generated. (3 points)

**Calculate Quartiles, Find Outliers, and Create a Box Plot (30 points)**
    *  A DatFrame that has the last timepoint for each mouse ID is created using groupby. (5 points)
    *  The index of the DataFrame is reset. (2 points)
    *  Retrieve the maximum timepoint for each mouse. (2 points)
    *  The four treatment groups, Capomulin, Ramicane, Infubinol, and Ceftamin, are put in a list. (3 points)
    *  An empty list is created to fill with tumor volume data. (3 points)
    *  A for loop is used to display the interquartile range (IQR) and the outliers for each treatment group (10 points)
    * A box plot is generated that shows the distribution of the final tumor volume for all the mice in each treatment group. (5 points)

**Create a Line Plot and a Scatter Plot (10 points)**
    * A line plot is generated that shows the tumor volume vs. time point for one mouse treated with Capomulin. (5 points)
    * A scatter plot is generated that shows average tumor volume vs. mouse weight for the Capomulin regimen. (5 points)

**Calculate Correlation and Regression (10 points)**
    *  The correlation coefficient and linear regression model are calculated for mouse weight and average tumor volume for the Capomulin regimen. (10 points)


**REFERENCES**
* For referencing the .agg() method Syntax and Paramters: https://pandas.pydata.org/docs/reference/api/pandas.core.groupby.DataFrameGroupBy.agg.html?highlight=agg#pandas.core.groupby.DataFrameGroupBy.agg 

* For formatting elements in the boxplot(subplots) figure: https://stackoverflow.com/questions/65648502/how-to-change-outlier-point-symbol-in-python-matplotlib-pyplot 

* For dropping a row using a column value: https://sparkbyexamples.com/pandas/pandas-delete-rows-based-on-column-value/#:~:text=Use%20drop()%20method%20to,or%20on%20another%20column%20value.

* Finging "duplicated" data: https://www.geeksforgeeks.org/find-duplicate-rows-in-a-dataframe-based-on-all-or-selected-columns/ 