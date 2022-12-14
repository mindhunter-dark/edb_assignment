**About**

Load the list of commits for a public Github repository into a SQLite DB and perform some analysis on the loaded data.

**Tools Used**
1. Jupyter Notebook
2. SQLite

**Folder Structure**
1. Assignment.ipynb - The main Jupyter Notebook
2. github_commits.db - The database file which stores the data
3. requirements.txt - The packages required to run the Python code
4. secrets/API.json - The url and Access token to call the Github API. You can create your own TOKEN [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
5. secrets/DDL.json - The DDL of the tables in the database
6. secrets/DML.json - The DML of the tables in the database
6. secrets/DQL.json - The actual queries which compute the final result-sets for the problems

**Input required from user**
1. URL of the public repository in the format "https://github.com/{owner}/{repo}" Ex:- "https://github.com/apache/airflow"
2. Start date - Date from which the commits are to be pulled
3. End date - The date until which commits will be pulled (this date excluded)


The Jupyter notebook can be run **online** in a **web browser** by clicking on this link below

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mindhunter-dark/edb_assignment/HEAD?labpath=Assignment.ipynb)

Notes on Binder:
1. It may take some time to load the online noteboook
