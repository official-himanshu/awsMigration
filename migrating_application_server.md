# Migrating Application server using SMS(Server migrating service)
We can migrate on-premise VMware,HyperV hosted application easily using SMS.

SMS is easy and fast for migrating on-premise VMware and Hyper-V hosted application server.

We can migrate any type of server hosted in VM ware in on premise data center to AWS cloud using Server migration service provided by AWS which is free of cost and valid till 90 days for one aws account.

SMS has several advantages over traditional migration approach-
1. It basically migrate server at nearly zero downtime.
2. You can easily schedule the migration at any time. Like every hour , every sunday , at night window etc.
3. You can also provide the landing zone for the server. Like if you want to automatic dedploy server within a provisioned VPc, subnet etc.
4. It takes less time then traditional migration.


## How does it work?

#### Steps to configure and setup AWS SMS for server migration. 

1. Suppose that we have On-premise data center.

2. And we have a AWS account.

3. We have various servers which is hosted in On-premises VM.

4. First we need to deploy Server Miration connector in our Virtual machine. And then configure it using its ip on aws console.

5. Once connector is deployed and configured then on AWS console start it for taking snapshots of VM and store those in S3 bucket.

6. Once the SMS is configured then it again trigger VM Import/Export service which create the AMI from the snapshots created by connector.

7. In SMS we can also define landing zone information like our VPC, subnet and SG, where we need to put our server.

8. With the combination of both landing zone and AMI it create a cloud formation template of given server configuration that we provide. With the help of this AWS cloud formation template it deploy our server in an EC2 instance. 

You can see these steps in given below figure.

![SMS image]()
