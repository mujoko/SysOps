# EBS Volume & EFS 
## EBS Volume
* It’s a network drive (i.e. not a physical drive)
	* It uses the network to communicate the instance, which means there might be a bit of
	latency
	* It can be detached from an EC2 instance and attached to another one quickly
* It’s locked to an Availability Zone (AZ)
	* An EBS Volume in us-east-1a cannot be attached to us-east-1b
	* To move a volume across, you first need to snapshot it
* Have a provisioned capacity (size in GBs, and IOPS)
	* You get billed for all the provisioned capacity
	* You can increase the capacity of the drive over time

## EBS Volume Types
* EBS Volumes come in 4 types
	* GP2 (SSD): General purpose SSD volume that balances price and performance for a
	wide variety of workloads
	* IO1 (SSD): Highest-performance SSD volume for mission-critical low-latency or highthroughput
	workloads
	* ST1 (HDD): Low cost HDD volume designed for frequently accessed, throughputintensive
	workloads
	* SC1 (HDD): Lowest cost HDD volume designed for less frequently accessed workloads
* EBS Volumes are characterized in Size | Throughput | IOPS (I/O Ops Per Sec)
* Only GP2 and IO1 can be used as boot volumes


# EFS – Elastic File System
EFS – Elastic File System
* Use cases: content management, web serving, data sharing, Wordpress
* Uses NFSv4.1 protocol
* Uses security group to control access to EFS
* Compatible with Linux based AMI (not Windows)
* Performance mode:
	* General purpose (default)
	* Max I/O – used when thousands of EC2 are using the EFS
* EFS file sync to sync from on-premise file system to EFS
* Backup EFS-to-EFS (incremental – can choose frequency)
* Encryption at rest using KMS