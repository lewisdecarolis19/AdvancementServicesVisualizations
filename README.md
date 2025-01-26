<h1>Advancement Services Reporting</h1>


<h2>Objective 🎯</h2>


This project aims to report on the non-profit's current campaign production and revenue. The task involves creating data visualizations for reports shared with both internal and external stakeholders. These visuals should clearly show differences between actual revenue and production versus target numbers, breaking down data by financial category and year. Ultimately, these charts will illustrate fundraising performance and trends, highlighting areas needing improvement to achieve goals. 
<br><br>
A dashboard is being developed to further identify key trends and insights as well as gauge performance in greater detail.  Currently, the included visualizations are meant to act as easily interpreted supplements to written reports, and they are not meant to be drilled down into or sliced further by the user.


<h2>Background Information 🏞️</h2>

Advancement Services is responsible for entering, maintaining, and retrieving data related to fundraising and donations within a non-profit organization. They provide insights on fundraising data, which includes building donor ratings and scores, predicting revenue and production, and analyzing trends by financial category over time.  Advancement Services also creates financial and constituent reports for internal and external stakeholders related to fundraising. Additionally, they use their findings to research and identify new prospects as well as update information on current prospects and donations. 

In Advancement Services, revenue and production differ. Revenue measures actual cash received, including payments, bequests, irrevocable planned gifts, and pledges. It reflects the amount collected by the fundraising campaign, excluding new activities or expectancies. Production measures new activity or expectancies like outright gifts, bequest expectancies, planned gifts, and pledges, excluding payments. Both metrics gauge performance but from different perspectives.

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

