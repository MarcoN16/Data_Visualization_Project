# Project Overview
This script analyzes data obtained from a pharmaceutical company specializing in anti-cancer medications, focusing on screening potential treatments for squamous cell carcinoma (SCC), a common form of skin cancer. The dataset comprises information from their recent animal study involving 249 mice identified with SCC tumors, treated with various drug regimens over a 45-day period. The study's primary aim was to assess the effectiveness of Pymaceuticals' drug of interest, Capomulin, in comparison to other treatment regimens. The script generates tables and figures essential for the technical report of this clinical study.

# Preparation of Data
1.	Data Import and Merging: Initially, the script imports and merges two datasets, mouse_metadata and study_results, into a unified DataFrame.
2.	Duplicate Time Points Handling: The script identifies and addresses any mouse ID instances with duplicate time points. The associated data is displayed, and a new DataFrame excluding this data is created, ensuring a clean dataset for subsequent analysis.

# Summary Statistics Generation
The script computes summary statistics, consisting of:
•	Rows for each drug regimen.
•	Columns for statistical measures like mean, median, variance, standard deviation, and SEM (Standard Error of the Mean) of the tumor volume.

![Summary_Statistics](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/69f305b1-6e1b-4e04-9937-4c443bbf393d)

# Bar Charts and Pie Charts Creation
1.	Bar Charts: Two sets of bar charts are generated, displaying the total number of timepoints for each drug regimen throughout the study period.
2.	
o	The first chart utilizes the Pandas DataFrame.plot() method.

o	The second chart is created using Matplotlib's pyplot methods.

![bar_chart_pandas](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/153f968f-d9ce-45d0-a2c7-599dca9dcfb3)
![bar_chart_pyplot](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/b5762b88-dd09-4f3d-8a93-4437cdb263e2)

3.	Pie Charts: Two pie charts illustrate the distribution of female versus male mice in the study.
4.	
o	The first pie chart employs the Pandas DataFrame.plot() method.

o	The second pie chart is generated through Matplotlib's pyplot methods.

![pie_chart_pandas](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/092ce00f-f334-4c24-b52a-e4c9d267eea4)
![pie_chart_pandas](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/aa4f843b-1d9f-4454-93f0-6fd2403e0528)


# Quartiles, Outliers Identification, and Box Plot Generation
1.	Quartile Calculation and Outlier Identification: Analysis focuses on determining the final tumor volume for mice under four prominent treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Quartiles, Interquartile Range (IQR), and potential outliers across these regimens are computed.
2.	Box Plot Creation: Using Matplotlib, a box plot displays the distribution of final tumor volume for mice in each treatment group. Any potential outliers are highlighted by altering their color and style.
   
![Boxplot_pyplot](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/d38b5eb3-6034-4527-83f6-928a76372b85)


# Line Plot and Scatter Plot Creation
1.	Line Plot: A line plot showcasing the tumor volume versus time point for a specific mouse treated with Capomulin is generated.
2.	Scatter Plot: A scatter plot depicting mouse weight versus the average observed tumor volume for the complete Capomulin treatment regimen is produced.

![Example_mouse_treated_Capomulin](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/b991b9be-46e3-4803-88da-67e8ff9e4b24)
![Scatter_plot](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/d6c2f431-a747-4c8b-9fe6-b03e20f39b40)

 
# Correlation and Regression Analysis
1.	Correlation and Regression: The script concludes by calculating the correlation coefficient and developing a linear regression model to explore the relationship between mouse weight and the average observed tumor volume throughout the Capomulin treatment regimen.
   
![Linear_correlation](https://github.com/MarcoN16/Data_Visualization_challenge/assets/150491559/b411fe80-43e8-417c-bf62-80931e849566)

