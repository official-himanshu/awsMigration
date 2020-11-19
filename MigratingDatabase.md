### Ways to migrate database.
1. Backup and restore -- In this we generally take up complete full backup of our database in the form of .bak file and then restore in our new sql server. In this we basically get full object presevation like foreign key, private key, constraints, indexes etc. We can also store this .bak file in our S3 bucket and restore this into RDS instance. Or we can restore in ec2 hosted sql server. but it has some drawback like it required a downtime. In this we perform lift and sift process.

2.  SQL server replication or Use AlwaysOn Availabilty group.

3. Use aws DMS:- By this we basically bulk load data and replicate on-going changes.