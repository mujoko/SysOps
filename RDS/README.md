# Relational Database Service
## RDS with CloudWatch
RDS with CloudWatch
* CloudWatch metrics associated with RDS (gathered from the hypervisor):
** DatabaseConnections
** SwapUsage
** ReadIOPS / WriteIOPS
** ReadLatency / WriteLatency
** ReadThroughPut / WriteThroughPut
** DiskQueueDepth
** FreeStorageSpace
* Enhanced Monitoring (gathered from an agent on the DB instance)
** Useful when you need to see how different processes or threads use the CPU
** Access to over 50 new CPU, memory, file system, and disk I/O metrics

## RDS Performance Insights
* Visualize your database performance and analyze any issues that affect it
* With the Performance Insights dashboard, you can visualize the database
load and filter the load:
..* By Waits => find the resource that is the bottleneck (CPU, IO, lock, etc…)
..* By SQL statements => find the SQL statement that is the problem
..* By Hosts => find the server that is using the most our DB
..* By Users => find the user that is using the most our DB
* DBLoad = the number of active sessions for the DB engine
* You can view the SQL queries that are putting load on your database

source
https://aws.amazon.com/blogs/database/tuning-amazon-rds-for-mysql-with-performance-insights/