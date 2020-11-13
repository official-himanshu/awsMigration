# Case-studies
## 1. YAMAHA
	Established in 1960 as Yamaha International Corporation, Yamaha Corporation of America (YCA) offers a full line of musical instruments and audio/visual products to the U.S. market. YCA is a wholly-owned subsidiary of Yamaha Corporation, Japan, and is one of the largest global subsidiary companies. The company had been managing all of its applications and infrastructure internally, with one data center at headquarters in Buena Park, CA, used primarily as a backup facility, and all production, test and development systems running in a colocation arrangement at an AT&T hosted data center in Irvine, CA.

#### Problem
	Yamaha was spending too much time replacing hardware and handling routine maintenance tasks and too much budget on buying capacity.

#### Goal
	They wanted their IT people to spend 70% of their time on new initiatives and only 30% on routine maintenance activities.

#### Solutions
	They migrate their production systems to AWS and manage the environment, saving the company $500,000 annually and freeing their IT people to get important projects done.

#### Challenges of on-premises infrastructure
	With 30-month replacement cycles for its leased hardware, the Yamaha IT infrastructure group was spending too much time replacing hardware and handling routing maintenance tasks such as patching Windows servers. “We really need our IT people spending 70% of their time on new initiatives and only 30% on routine maintenance activities, yet that wasn’t happening,” says Vimal Thomas, VP, Information Technology Division, at Yamaha. IT was also buying 30% more capacity than was needed or used, to guarantee performance and uptime, wasting budget that could have been used in other areas.

#### Journey to the cloud
	Yamaha had a rapid timeline for moving its infrastructure to AWS, as Thomas wanted the process to be complete prior to an important ERP upgrade to Oracle R12. Yamaha and 2nd Watch began by migrating the development and testing systems to AWS. By August 2014, all production systems aside from Oracle and Cisco Voice had been moved to the cloud. Due to some uncertainties about how Oracle would run on AWS, Yamaha decided to keep the ERP system running internally, though Thomas says it will eventually migrate to the cloud as well. 2nd Watch also helped Yamaha configure database mirroring in MS SQL 2008 to ensure high availability.

	Additionally, 2nd Watch is providing ongoing services to Yamaha, including configuring AWS availability zones for data replication and disaster recovery, designing file system backup, designing scripts to automate the shutdown and startup process of non-production systems, identifying AWS management tools for hosts, networks, security and storage, network design and security and overall design/configuration of AWS EBS and AWS Elastic IP.











### 2. Spotify (est. 2006) 
	Spotify is a media services provider primarily focused on its audio-streaming platform, which lets users search for, listen to, and share music and podcasts.

#### Migration Objective 
	Spotify’s leadership and engineering team agreed: The company’s massive in-house data centers were difficult to provision and maintain, and they didn’t directly serve the company’s goal of being the “best music service in the world.” They wanted to free up Spotify’s engineers to focus on innovation. They started planning for migration to Google Cloud Platform (GCP) in 2015, hoping to minimize disruption to product development, and minimize the cost and complexity of hybrid operation. 

#### Migration Strategy and Results 
	Spotify invested two years pre-migration in preparing, assigning a dedicated Spotify/Google cloud migration team to oversee the effort. Ultimately, they split the effort into two parts, services and data, which took a year apiece. For services migration, engineering teams moved services to the cloud in focused two-week sprints, pausing on product development. For data migration, teams were allowed to choose between “forklifting” or rewriting options to best fit their needs. Ultimately, Spotify’s on-premise to cloud migration succeeded in increasing scalability while freeing up developers to innovate. 

#### Key Takeaways
##### Gaining stakeholder buy-in is crucial.
	Spotify was careful to consult its engineers about the vision. Once they could see what their jobs looked like in the future, they were all-in advocates. 
##### Migration preparation shouldn’t be rushed. 
	Spotify’s dedicated migration team took the time to investigate various cloud strategies and build out the use case demonstrating the benefits of cloud computing to the business. They carefully mapped all dependencies. They also worked with Google to identify and orchestrate the right cloud strategies and solutions. 
##### Focus and dedication pay huge dividends. 
	Spotify’s dedicated migration team kept everything on track and in focus, making sure everyone involved was aware of past experience and lessons already learned. In addition, since engineering teams were fully focused on the migration effort, they were able to complete it more quickly, reducing the disruption to product development.










### 3. Cloud Migration: A Case Study of Migrating an Enterprise IT System to IaaS

	This case study explain the potential benefits and risks associated with the migration of an IT system in the
	oil & gas industry from an in-house data center to Amazon EC2 from a broad variety of stakeholder
	perspectives across the enterprise.

	This case study is basically a cloud migration of in house infrastructure to AWS cloud.
	The anonymous situation is like there is COMPANY C who owned some assests in oil and gas corporation from COMPANY A. Company C needed a data acquisition system to allow them to manage their offshore operations by monitoring data from their assets on a minute by minute basis. Company C’s assets rely on the production facilities of Company A (a major oil company), therefore the data comes onshore via Company A’s communication link. 

	Company C does not have the capabilities to develop their own IT systems, hence they outsourced the development and management of the system to Company B, which is an IT solutions company with a small data center.

	1. So basically company B as all applicaion servers that host number of data reporting and monitoring application. The end users at Company C access these applications using a remote desktop client over the internet.

	2. A database server that logs and archives the data coming in from offshore into a database. A tape drive is used to take daily backups of the database, the tapes are stored off-site.

#### Methodlogy used by the company B

	Stage 1: In this stage basically they gather all there documents related to there system under investigation.
	
	Stage 2: They now calculate the infrastructure cost from the invoices and project report and compare it with the cost of same architecture over the AWS cloud.

	Stage 3: In this stage they basically analyzed there support calls of database migration to the cloud like how there database migrate and operate over the cloud. For this they mannaully research all the database configurations and dependencies.

	stage4: The results from the above two stages were used to produce a poster. The poster was presented to Company B’s employees and six semi-structured interviews were performed at their offices. The interviews started by giving the interviewees an overview of Amazon EC2 as they were only partially familiar with this technology. Each interview was recorded and a transcript of each interview was produced. Each transcript was read be two researchers (one present at the interview and one not) and a number of issues were identified and agreed using a stakeholder impact analysis. Stakeholder impact analysis is a method of identifying potential sources of benefits and risks from the perspectives of multiple stakeholders, and is performed by analyzing interview transcripts.


#### Results 
	cost of on-premises
	
	->Company C paid £104,000 to Company B for the system in 2005, £19,400 of which was for the system’s infrastructure; the rest of the costs were for system development and deployment. The infrastructure included two servers (each having two Intel Xeon 3.4GHz processors, 2GB RAM, 6 x 72GB hard drives in a RAID 10 array resulting in around 200GB of effective storage, Windows Server 2003 OS), a tape drive, network equipment, a server rack, shelf spares. In addition, Company C pays £43,000 per year to Company B for system support and maintenance, £3,600 of which is for the running costs of the system infrastructure. Over a five year period, the total cost of the system infrastructure is therefore: £19,400 + (5 x £3,600) = £37,400.

	->Estimated cost over cloud The following specifications were used to calculate the costs of running the system on AWS: two Microsoft Windows On-Demand instance (AWS do not offer reserved instances for Windows) in Europe running 730 hours per month (i.e. 24x7); 20GB data transfer in; 20GB data transfer out; 200GB EBS storage (i.e. amount of effective storage on existing servers), 100 million EBS I/O request; 30GB EBS snapshot storage (for daily backups); 10 snapshot GET requests (in case backups need to be retrieved); 30 snapshot PUT requests (for daily backups).

#### Comparison of cost


	Comparison of infrastructure costs between
		cloud and Company B’s data center
						Amazon Server Instances
Period 		2 small  |   1 small+1 large   |   2 large  |   Company B on premises
1 Month 	 £200 	 |		£390 		   |    £590    |	 £620
1 Year 		£2,400   |      £4,680         |    £7,080  |    £7,440
5 Years 	£12,000  |	    £23,400 	   |    £35,400 |   £37,200










## 4 Crate & Barrel’s

#### Problem
Crate & Barrel’s traditional managed hosting platform couldn’t keep up with the rate of online customer demand.

#### Goal
They wanted a platform that could scale with demand to improve the customer experience.

#### Solution
They migrated their environment to AWS, decommissioning their data center and setting them up for a successful holiday shopping season.

### About Crate and Barrel
Crate and Barrel is an industry-leading home furnishings specialty retailer, known for its exclusive designs, excellent value and superb customer service. In addition to a thriving direct marketing division that services more than 90 countries, the company operates stores throughout the U.S. and Canada as well as international franchise locations in Mexico, Peru, Philippines, Russia, Singapore, Taiwan, Turkey and the United Arab Emirates. Working directly with European ateliers and factories, Crate and Barrel was among the first to introduce affordable household goods and contemporary home décor to American consumers. Founded in 1962, the brand’s essence has translated perfectly to the omnichannel era more than 50 years after opening its first store. The Crate and Barrel family of brands, which includes CB2 and The Land of Nod, is owned by Otto Group, a global retail and services group based in Hamburg, Germany.

#### The business challenges & 2nd Watch solution
After over a decade of operation on traditional managed hosting platforms, Crate and Barrel’s eCommerce operation was faced with the need for a more nimble and cost effective hosting solution. The decision was made to migrate to the AWS platform, and 2nd Watch was selected as the migration and managed services partner.

The 2nd Watch professional services team migrated all three Crate and Barrel web and e-commerce properties from a traditional hosting facility to AWS, DECOMMISSIONING ONE DATA CENTER AND 25 SERVERS, and setting the company up for a successful holiday season. The teams worked through the design and implementation challenges that go along with migrating web properties to AWS, devised a migration strategy, and BUILT THE INFRASTRUCTURE IN THE NEW AWS ENVIRONMENT USING AWS EC2, RDS, ELB AND S3, INCLUDING A MIX OF SQL SERVER EC2 AND RDS INSTANCES IN BOTH PRODUCTION AND NON-PRODUCTION ENVIRONMENTS. Additionally, 2nd Watch implemented Cloud Protection Manager for snapshots/backups and assisted Crate & Barrel in transitioning its Land of Nod commerce site to its primary Crate & Barrel domain, decommissioned its mobile sites, and implemented autoscaling on its brand sites.

Today, the 2nd Watch managed cloud team supports Crate & Barrel’s AWS environment through management and optimization services.

#### The business benefits
Crate and Barrel will gain the flexibility and elasticity that comes with an AWS environment. The new environment has the ability to scale up on demand and handle hundreds of checkouts per minute. George Findling, Director of Emerging Technology, noted that the migration performed flawlessly through Black Friday and Cyber Monday without a single technical or operational incident.

By deploying the new environment on AWS, Crate and Barrel is able to take advantage of on-demand compute, scaling up and down as needed for the shopping season without oversubscribed capital purchases. The company anticipates significant reduction in the eCommerce platform monthly operating cost by migrating to AWS with the help of 2nd Watch.








## 5 Aspire Systems

### Need of on-premises data center
	a). Upfront hardware and software cost.
	b). Difficulty in capacity building and deployment
	c). Required dedicated resources for maintaining the data center. 

	Migrating to aws has following advantages:
	• 99.95% uptime of the servers
	• Less maintenance cost
	• Zero data loss and robust back-up protocols

### Challenges
	a). Multiple applications and platforms to be moved to AWS cloud which makes the process tedious
	b). Lack of documentation support and redundant data for on premise datacenter
	c). Poor application performance while accessing from different geo-locations

	This is very much challenging to migrate this much of ambiguity to cloud so Aspire systems came up with a program called “Trio  Migration” involving administrative migration, data center migration and Database migration.

### Solution
	So for this they use different tools and technologies like java, php, EKS, jenkins and amazon RDS/Aurora. So they divide the work in modules and each module has unique approach to ensure smooth migration.
	a). Since there applications are old and based on old architecture so they are rebuild and architectures agai so that they are suitable for cloud.
	b). They use CI/CD for faster process using jenkins as some of the application was rebuild.
	c). They use EKS for containerization deployment.


	1. Application migration:- For application migration, the cloud related changes are done to make sure that all application are ready for cloud deployment and enablement. All the application which are re-architecured are based on AWS kafka. They also done other enhancement like they update the java version and weblogic servers.

	2. Database Migration:- They migrate there Instance of Oracle SQL and MySQL on AWS Aurora/RDS with the help of DMS. And the DB which are not compatiable are hosted over Amazon EC2. Snowball devices are used for data transfer which has more than 1TB of data. 100+ TB of data migrated from on-premises to AWS.

