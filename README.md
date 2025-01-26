<h1>Advancement Services Reporting</h1>


<h2>Objective 🎯</h2>




1. Use the data to pull Current Campaign Production by Financial Category for Fiscal Year 2024.
Once you have this information, you will also need to pull budget totals for Financial Category
for Campaign Production. Once you have both data sets pulled, create a report that gives a
graph for campaign production FY2024 budget vs actual.
2. Use the data to pull Current Campaign Revenue by Financial Category for Fiscal Year 2024. Once
you have this information, you will also need to pull budget totals for Financial Category for
Campaign Revenue. Once you have both data sets pulled, create a report that gives a graph for
campaign revenue FY2024 budget vs actual.
3. Using the production data, create a report that shows FY totals of Campaign Production actuals
and budget by Fiscal Year. Include a trendline to actuals to show movement year-over-year.
4. Use the revenue data, create a report that shows FY totals of Campaign Revenue actuals and
budget by Fiscal Year. Include a trendline on actuals to show movement year-over-year.
Questions:
1. Where do we need to focus on Campaign Production regarding Financial Category?
2. Where do we need to focus on Campaign Revenue regarding Financial Category?
3. What other information would you need to help understand how University Relations is doing?


<h2>Background Information 🏞️</h2>

Advancement Services is responsible for entering, maintaining, and retrieving data related to fundraising and donations within a non-profit organization. They provide insights on fundraising data, which includes building donor ratings and scores, predicting revenue and production, and analyzing trends by financial category over time.  Advancement Services also creates financial and constituent reports for internal and external stakeholders related to fundraising. Additionally, they use their findings to research and identify new prospects as well as update information on current prospects and donations. 

<h2>Business Questions 🔎</h2> 
  
  -  Where do we need to focus on Campaign Production regarding Financial Category?
  -  Where do we need to focus on Campaign Revenue regarding Financial Category?





<h2>Solution ⚡️ </h2>

To

<h2>Process and Tools 🔨 </h2>

1. A [Python script](https://github.com/lewisdecarolis19/GithubUtilizationMetrics/blob/main/Get_GitHub_Data.py), developed in <b>Jupyter Notebooks</b>, interacts with the [GitHub REST API](https://docs.github.com/en/rest?apiVersion=2022-11-28) to gather repository data in JSON format.  The script handles the default pagination of the API, and nested for loops are used to iterate through 2 repositories and 4 endpoints.
    - Data specifically pertains to commits, pull requests, pull request comments, and contributors.
    - The data is structured into data frames using the <b>Pandas</b> library and then concatenated and appended into a list of finalized data frames.
    - The <b>ExcelWriter</b> function is used to submit each data frame in the list to its own tab in an output spreadsheet.
    - The spreadsheet is pathed locally to a synced Sharepoint folder.  When the script is ran, the file in Sharepoint is replaced with a file containing new data.
    - The Python script is scheduled to run every morning through <b>JupyterLab</b>.


<h2>Results and Recommendations 🚀</h2>

🚧 In Progress 🚧

<h2>Project Files 📄</h2>

-  [Python Script](https://github.com/lewisdecarolis19/GithubUtilizationMetrics/blob/main/Get_GitHub_Data.py)

