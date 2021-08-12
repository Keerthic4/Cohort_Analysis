# Analysis Outline
In this small project, we are analyzing the data consisting list of marketing & Advertising company customers and list of charges which is converted into multiple cohort analysis chart
A cohort analysis was performed, separated based on what country the customers are from as follows:
1.	American customers, 
2.	Australian customers and,
3.	Canadian customers
Finally, the master data (no geographic separation) is used to prepare a cohort layer cake.

# Tools used
1.	Jupyter notebook (Python language for data analysis), 
2.	Exploratory desktop free version (for making Cohort Layer Cake).
3.	All the codes are present in the Jupyter notebook.

# Summary of Analysis
The given dataset encountered significant data quality issues. Columns, such as card__country, have empty values in certain records. Mitigation: If only a small number of rows are empty, filter out the record entirely from the training set for prediction. Else, if it is a core field, impute based on the distribution in the training dataset. Here impute is not possible. Going with 1678 non-null entries.
Making assumption- All the DateTime and currency in a proper format, and there is no need for any conversion.
From the data analysis, we found the highest-paid countries are KE(Kenya), IN (India). The highest refunded countries are DK (Denmark), IN (India). The top 3 most frequently represented countries on the data frame are the US, AU, CA.
In general, you can see from the retention rate Data Frame:
•	Retention Rate 1st index i.e., 1st Month is 100% as all the customers for that particular customer signed up in 1st Month
•	The retention rate may increase or decrease in Subsequent Indexes.
•	Values towards Bottom Right have a lot of NaN values.
From heatmaps, it is clear that business is not making a profit from American customers from June 2020 to Sep 2020. From Oct 2020 to Dec 2020 company is making a profit. For Dec 2020 and 1st cohort, Month_Index company produces the highest average profit for American customers of 288.2.
From heatmaps, it is clear that business is not making a profit from Australian customers in Aug 2020. From Oct 2020 to Dec 2020 company is making a profit. For Nov 2020 and 1st cohort, Month_Index company produces the highest average profit for Australian customers of 285.1.
From heatmaps, it is clear that business is not making a profit from Canadian customers in Sep 2020. From Oct 2020 to Dec 2020 company is making a profit. For Nov 2020 and 2nd cohort, Month_Index company produces the highest average profit for Canadian customers of 317.1.
In general, the company is making an average profit from the top 3 most frequently represented countries that are US, AU, CA from Oct 2020 to Dec 2020.
Finally created a CSV for master data (no geographic separation) to prepare a cohort layer cake.

# Cohort Layer Cake Analysis
