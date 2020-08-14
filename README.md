# GS-Quantify-2019
Context

Logs are an integral part of Goldman Sachs' day-to-day operations. We depend upon logs to monitor the behavior of thousands of applications which process millions of trades, help us manage risk, support algorithmic trading and so on. In all, these applications generate hundreds of millions of log lines every day which engineers comb through to identify and rectify application failures.

However, different applications built by different engineers tend to communicate the same kinds of failures in different ways. This makes the process of identifying similar failures across different applications difficult and tedious.

To that end, the log analytics team at Goldman Sachs is developing tools that would identify common kinds of failures. This would enable the engineers to easily spot failures and assess who is best equipped to respond to such failures.

The problem that you must solve is just this - given a set of log lines, assign each to a cluster. The overall goal of this problem is to identify the intent of each log line and group log lines with the same intent in the same cluster.

Your submission will be evaluated on the number and quality of your clusters, as well as the techniques that you use to form the clusters.
Some Examples of Correct Clustering
Example 1

The following lines are all part of the same cluster that queries an API for a list of servers:

gs-quantify-api 2019-30-06 13:00:10 Received 30 server IDs from API
gs-quantify-log 2019-31-07 09:30:55 Received 1550 server UIDs from API
gs-quantify-api 2019-08-31 13:30 Received 80 server UMMIDs from API

Example 2

The following belong to a cluster that processes datasets:

gs-quantify-data 2019-25-08 07:53:32 Loaded dataset DatasetName from DB2
gs-quantify-data 2019-25-08 09:53:32 Processed dataset DatasetName
gs-quantify-data 2019-25-08 10:03:32 Saved dataset DatasetName to DB2

Example 3

The following belong to a cluster that queries a particular REST API:

gs-quantify-api 2019-12-07 11:30:09.001001 Downloaded 81 records using "GET /magic_api/dataset_x.csv"
gs-quantify-api 2019-12-07 11:30:09.001001 Saved 755 records using "POST /magic_api/dataset_y"


### Models and techniques used - 
Word2vec text transformation
1. K-Means
2. DBSCAN 
