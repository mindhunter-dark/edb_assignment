# About
Load the list of commits for a public Github repository into a SQLite DB and perform some analysis on the loaded data.

## Tools Used
1. Jupyter Notebook
2. SQLite

## Folder Structure
1. Assignment.ipynb - The main Jupyter Notebook
2. github_commits.db - The database file which stores the data
3. requirements.txt - The packages required to run the Python code
4. secrets/API.json - The url and Access token to call the Github API. You can create your own TOKEN [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
5. secrets/DDL.json - The DDL of the tables in the database
6. secrets/DML.json - The DML of the tables in the database
7. secrets/DQL.json - The actual queries which compute the final result-sets for the problems
8. DataEngineeringAssignment.pdf - The problem statement

## Database tables
For each new repository, a new table will be created. You can run the code multiple times to get the commits for multiple repositories

1. **commits_{owner}_{repo}**
### Schema
sha TEXT            - sha of the commit
author_name TEXT    - Name of the author(committer)
author_email TEXT   - Eail of the author(committer)
commit_time TEXT    - Time of the commit (ISO format)

## Input required from user
1. URL of the public repository in the format "https://github.com/{owner}/{repo}" Ex:- "https://github.com/apache/airflow"
2. Start date - Date from which the commits are to be pulled
3. End date - The date until which commits will be pulled (this date excluded)

## How to execute
The Jupyter notebook can be run **online** in a **web browser** by clicking on this link below

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mindhunter-dark/edb_assignment/HEAD?labpath=Assignment.ipynb)

**Notes**
1. Binder may take some time to load the online noteboook
2. Run the first cell in the notebook. Give the input and the program will load the data
3. Run the next set of cells for the solutions to the three problems
