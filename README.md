# CHAOSS
![Chaoss](/GraphAndTables/Chaoss_Logo.png?raw=true "logo")

# Microtask Submission.

## Requirements:

1. Basic python development environment : virtualenv, [python 3](https://www.python.org/downloads/), pip3.
2. [GrimoireLab packages](http://grimoirelab.github.io/), ElasticSearch and mariaDB.
3. [Elasticsearch](http://elasticsearch-py.readthedocs.io/en/master/index.html) should be running on localhost:9200
4. [Kibana](https://www.elastic.co/products/kibana) can also be used in order to visualize data in better way.

## Problem Statement

### Microtask 1:
Produce a listing of the number of new committers per month, and the number of commits for each of them, as a table and as a CSV file. Use the GrimoireLab enriched index for git.
**New Committers per month**
![New commiter table]('/GraphAndTables/new commiters per month.png'?raw=true "new commiter")

**Number of commits**
![commits table]('/GraphAndTables/number of commits.png'?raw=true "table")

### Microtask 2:
Produce a chart showing the distribution of time-to-close (using the corresponding field in the GrimoireLab enriched index for GitHub issues) for issues already closed, and opened during the last six months.
![Graph](/GraphAndTables/Microtask2.png?raw=true "graph")

In order to run the notebook, download it and replace repo_name and org_name with the repository and organisation name of the github repo you want to analyse, replace raw_index and enriched_index with your desired index names and run the script to get the desired result. Also use github verification token to avoid problems regarding unauthenticated access and to bypass the rate limit GitHub API.

### Microtask 3:
Produce a listing of repositories, as a table and as CSV file, with the number of commits authored, issues opened, and pull requests opened, during the last three months, ordered by the total number (commits plus issues plus pull requests).
![Plot](/GraphAndTables/Repo_Total.png?raw=true "plot")

In order to run the notebook, download it and replace url with the url of the github organisation whose repositories you want to analyse, replace raw_index and enriched_index with your desired index names and run the script to get the desired result.

### Microtask 4:
Perform any other analysis you may find interesting, based on GrimoireLab enriched indexes for git and GitHub repositories.
I've implemented a basic fork metric to show how github api can be used to support metric that are not yet supported by grimoirelab.
**Number of Forks**
![Fork table]('/GraphAndTables/number of forks.png'?raw=true "plot")
### Microtask 5:
Produce a pull request for any of the GrimoireLab tools, and try to follow instructions until it gets accepted. Try do do something simple that you consider useful, not necessarily fix to the code: improvement of comments, documentation or testing will usually be easier to get accepted, and very useful for the project. Please, avoid just producing a random pull request just to have another microtask: the objective is not that you get one more microtask done, but that you understand how to interact with developers in the project contributing with something that could be useful).

For this microtask, I produced 3 pull requests:
[Pull request 1](https://github.com/chaoss/grimoirelab-manuscripts/pull/33)
[Pull request 2](https://github.com/chaoss/grimoirelab-manuscripts/pull/35)
[Pull request 3](https://github.com/chaoss/grimoirelab-tutorial/pull/16)
