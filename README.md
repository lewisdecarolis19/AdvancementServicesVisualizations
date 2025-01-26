<h1>Advancement Services Reporting</h1>


<h2>Objective 🎯</h2>
The objective of this 

<h2>Business Questions 🔎</h2> 
  
  -  How has the team's usage of GitHub changed over time?  What is the trend over the past ___ quarters or years? Is there a reason for this? 
  -  Are we utilizing Github for code reviews as intended?
  -  How does the number of internal cases requiring a code review submission compare to the actual number of pull requests? Which cases didn't have a pull request that should have?
  -  Are there certain types of internal cases that are more susceptible to not receiving a pull request?  Why is this?
  -  How many commits are pushed per pull request, on average? Are we commiting new code after it has been reviewed by the team?
  -  How many comments or reviewers does each pull request receive, on average?
  -  Who is contributing the most to the health of our repositories?  Who is not following our established protocols for code reviews?
  -  What type of contributions does the team need to improve? For example, are we good at leaving reviews on code but bad about committing new code after a review?
  -  Is the lack of contribution to the repository because of a training or process gap?  How can we fill this gap and support eachother better as a team?

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

