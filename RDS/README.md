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