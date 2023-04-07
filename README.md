"Exploring International Debt Data: An Analysis of the World Bank's Dataset"

	In this analysis, we will explore The World Bank's international debt data, which sheds light on the amount of debt (in USD) owed by developing countries for various purposes, including infrastructure spending. Our goal is to answer key questions such as the total amount of debt owed, which country holds the largest debt, and the average amount of debt across different debt indicators. Join us as we uncover valuable insights from this dataset!




This analysis aims to answer the following questions based on The World Bank's international debt data:

What is the overall amount of debt owed by the countries in the dataset?
Which country holds the highest amount of debt, and what is the corresponding value?
What is the average debt amount across various debt indicators for different countries?
How can we find the unique values for countries, indicators, and codes in the dataset using the "DISTINCT" keyword in SQL?


The first line of code initiates a connection to the international_debt database, where the international_debt table is stored. Our initial query selects all columns from the international_debt table while limiting the output to the first ten rows, promoting a clean and concise output format.


![Screen Shot 2023-04-07 at 12 41 56 AM](https://user-images.githubusercontent.com/71097138/230547590-31f045d9-0946-4a41-a37f-1d04f3863892.png)


Calculating the count of unique countries present in the dataset:


After analyzing the first ten rows of the dataset, it is evident that Afghanistan has incurred debt across multiple debt indicators. However, we cannot deduce the number of unique countries within the dataset due to the possibility of duplicated country names. It is crucial to identify the count of distinct countries to ensure comprehensive statistical analysis. This section focuses on retrieving the number of unique countries present in the dataset.



![Screen Shot 2023-04-07 at 12 12 53 AM](https://user-images.githubusercontent.com/71097138/230547909-b4defb2c-ff6b-46aa-88f2-ac8670d1bf80.png)



Discovering the unique debt metrics(indicater_code)

The table contains records for a total of 124 countries. In the initial section, we observed that the indicator_name column provides a brief description of the reasons for incurring debt. The adjacent column, indicator_code, indicates the type of debt. Familiarizing ourselves with these diverse debt indicators can aid in comprehending the potential areas in which a country may have borrowed funds.



![Screen Shot 2023-04-07 at 12 24 21 AM](https://user-images.githubusercontent.com/71097138/230665615-9c95569b-c2d6-4552-a20c-61bc2562b85b.png)



Determining the Total Debt: Summing up the Amount of Debt Owed by Countries


As previously stated, a country's financial debt serves as an indicator of its economic condition. However, when considering the global perspective, how can we effectively calculate the total amount of debt owed? This approach can provide us with  valuable insights into the overall health of the world economy.



v![Screen Shot 2023-04-07 at 12 28 51 AM](https://user-images.githubusercontent.com/71097138/230665919-19cbb5d7-77f9-4cb8-aa8d-1f673c54eede.png)



dentifying the Country with the Highest Debt


Now that we have calculated the total amount of debt owed by various countries, let's determine which country has the highest debt and the corresponding amount. It's worth noting that this debt represents the sum of various categories of debt owed by the country. By identifying the country with the highest debt, we can gain insights into its socio-economic situation. We could also determine the category in which the country owes the most debt, but we'll focus on that later.


![Screen Shot 2023-04-07 at 3 58 04 PM](https://user-images.githubusercontent.com/71097138/230670207-8f43bb08-b61c-47ba-9467-4b7e20ad2d4c.png)


Calculating the Average Debt across Indicators

After obtaining an overview of the dataset and its summary statistics, we have a grasp of the various debt indicators in which countries incur debt. To delve deeper, we can determine the average amount of debt owed by each country. This information can help us understand the distribution of debt amounts across different indicators.


![Screen Shot 2023-04-07 at 12 41 56 AM](https://user-images.githubusercontent.com/71097138/230666418-bea6265e-99c7-45bf-9422-0edf96f221d5.png)


Exploring Long-Term Debt and Principal Repayments

The DT.AMT.DLXF.CD debt indicator has the highest average debt and mainly includes long-term debts. Investigating this category can provide insights into the economic conditions of countries relying on long-term debt. We aim to identify the country with the highest amount of debt in this category, specifically the highest amount of principal repayments, which reflects the active debt payment status.


![Screen Shot 2023-04-07 at 3 34 59 PM](https://user-images.githubusercontent.com/71097138/230667050-0fac7288-146a-4fb9-ac38-a831eba8a32a.png)


The indicator that appears most frequently in relation to debt:

Our analysis shows that Venezuela has the highest amount of debt in the long-term debt category (DT.AMT.DLXF.CD), as verified by The World Bank. It's important to validate our findings to ensure their accuracy. While long-term debt (DT.AMT.DLXF.CD) tops the chart in terms of average debt, we need to determine if it's the most common indicator for countries to owe their debt. Let's investigate further.



![Screen Shot 2023-04-07 at 3 47 49 PM](https://user-images.githubusercontent.com/71097138/230669077-9834b629-31e5-4b14-9912-bde36edf7ff1.png)


Other possible debt-related problems and final thoughts.

Our dataset contains six debt indicators that all countries have taken debt in, including DT.AMT.DLXF.CD. This suggests a shared economic issue among these countries, but there may be more to uncover. Moving away from debt indicators, we'll shift our focus back to the amount of debt and determine each country's maximum debt. This will help identify other possible economic challenges a country may be facing. Throughout this notebook, we explored global debt and uncovered interesting statistics while ensuring the accuracy of our findings.



![Screen Shot 2023-04-07 at 4 01 18 PM](https://user-images.githubusercontent.com/71097138/230671494-e7aad142-967a-4d80-9cf9-dc4b75106b4c.png)


Project Title: Investigating International Debt Statistics

Project Description:

This project is about exploring international debt data obtained from The World Bank. The data is from the year 2012 and includes information about the amount of debt owed by countries across the globe, categorized by the type of debt indicator. The project covers a variety of topics such as data cleaning, data exploration and visualization, and statistical analysis.

Additional Resources:

The World Bank: The World Bank website contains a wealth of information on global economic and financial trends, including debt statistics. You can find the latest updates on international debt trends, as well as reports and publications related to global economic development.

IMF (International Monetary Fund): The IMF provides data, analysis, and research on global economic and financial issues, including debt sustainability and debt relief. Their website offers a range of resources on global economic trends, as well as country-specific information on economic policies and performance.

OECD (Organisation for Economic Co-operation and Development): The OECD is an intergovernmental organization that aims to promote economic growth, prosperity, and sustainable development. 

Their website provides a range of data and analysis on global economic and social issues, including debt statistics and economic policy recommendations.

DataCamp: DataCamp is an online learning platform that offers courses and projects on data analysis, programming, and data science. The project used in this example is available on the DataCamp website, and there are many other similar projects and courses that can help you improve your data analysis skills.

Sources : https://www.datacamp.com/projects/754




