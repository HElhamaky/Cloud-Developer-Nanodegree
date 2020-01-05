## Amazon S3
> Object storage built to store and retrieve any amount of data from anywhere

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon S3 is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.

### Benefits
* Industry-leading performance, scalability, availability, and durability
* Wide range of cost-effective storage classes
* Unmatched security, compliance, and audit capabilities
* Easily manage data and access controls
* Query-in-place services for analytics
* Most supported cloud storage service

## Amazon S3 Storage Classes
Amazon S3 offers a range of storage classes designed for different use cases. These include **S3 Standard** for general-purpose storage of frequently accessed data; **S3 Intelligent-Tiering** for data with unknown or changing access patterns; **S3 Standard-Infrequent Access (S3 Standard-IA)** and **S3 One Zone-Infrequent Access (S3 One Zone-IA)** for long-lived, but less frequently accessed data; and **Amazon S3 Glacier (S3 Glacier)** and **Amazon S3 Glacier Deep Archive (S3 Glacier Deep Archive)** for long-term archive and digital preservation. Amazon S3 also offers capabilities to manage your data throughout its lifecycle. Once an **S3 Lifecycle** policy is set, your data will automatically transfer to a different storage class without any changes to your application.  

### GENERAL PURPOSE
### Amazon S3 Standard (S3 Standard)
S3 Standard offers high durability, availability, and performance object storage for frequently accessed data. Because it delivers low latency and high throughput, S3 Standard is appropriate for a wide variety of use cases, including cloud applications, dynamic websites, content distribution, mobile and gaming applications, and big data analytics. S3 Storage Classes can be configured at the object level and a single bucket can contain objects stored across S3 Standard, S3 Intelligent-Tiering, S3 Standard-IA, and S3 One Zone-IA. You can also use S3 Lifecycle policies to automatically transition objects between storage classes without any application changes.

#### Key Features:

* Low latency and high throughput performance
* Designed for durability of 99.999999999% of objects across multiple Availability Zones
* Resilient against events that impact an entire Availability Zone
* Designed for 99.99% availability over a given year
* Backed with the Amazon S3 Service Level Agreement for availability
* Supports SSL for data in transit and encryption of data at rest
* S3 Lifecycle management for automatic migration of objects to other S3 Storage Classes  


### UNKNOWN OR CHANGING ACCESS
### Amazon S3 Intelligent-Tiering (S3 Intelligent-Tiering)
The S3 Intelligent-Tiering storage class is designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead. It works by storing objects in two access tiers: one tier that is optimized for frequent access and another lower-cost tier that is optimized for infrequent access. For a small monthly monitoring and automation fee per object, Amazon S3 monitors access patterns of the objects in S3 Intelligent-Tiering, and moves the ones that have not been accessed for 30 consecutive days to the infrequent access tier. If an object in the infrequent access tier is accessed, it is automatically moved back to the frequent access tier. There are no retrieval fees when using the S3 Intelligent-Tiering storage class, and no additional tiering fees when objects are moved between access tiers. It is the ideal storage class for long-lived data with access patterns that are unknown or unpredictable. S3 Storage Classes can be configured at the object level and a single bucket can contain objects stored in S3 Standard, S3 Intelligent-Tiering, S3 Standard-IA, and S3 One Zone-IA. You can upload objects directly to S3 Intelligent-Tiering, or use S3 Lifecycle policies to transfer objects from S3 Standard and S3 Standard-IA to S3 Intelligent-Tiering. You can also archive objects from S3 Intelligent-Tiering to S3 Glacier.

#### Key Features:

* Same low latency and high throughput performance of S3 Standard
* Small monthly monitoring and auto-tiering fee
* Automatically moves objects between two access tiers based on changing access patterns
* Designed for durability of 99.999999999% of objects across multiple Availability Zones
* Resilient against events that impact an entire Availability Zone
* Designed for 99.9% availability over a given year
* Backed with the Amazon S3 Service Level Agreement for availability
* Supports SSL for data in transit and encryption of data at rest
* S3 Lifecycle management for automatic migration of objects to other S3 Storage Classes


### INFREQUENT ACCESS
### Amazon S3 Standard-Infrequent Access (S3 Standard-IA)
S3 Standard-IA is for data that is accessed less frequently, but requires rapid access when needed. S3 Standard-IA offers the high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee. This combination of low cost and high performance make S3 Standard-IA ideal for long-term storage, backups, and as a data store for disaster recovery files. S3 Storage Classes can be configured at the object level and a single bucket can contain objects stored across S3 Standard, S3 Intelligent-Tiering, S3 Standard-IA, and S3 One Zone-IA. You can also use S3 Lifecycle policies to automatically transition objects between storage classes without any application changes.

#### Key Features:

* Same low latency and high throughput performance of S3 Standard
* Designed for durability of 99.999999999% of objects across multiple Availability Zones
* Resilient against events that impact an entire Availability Zone
* Data is resilient in the event of one entire Availability Zone destruction
* Designed for 99.9% availability over a given year
* Backed with the Amazon S3 Service Level Agreement for availability
* Supports SSL for data in transit and encryption of data at rest
* S3 Lifecycle management for automatic migration of objects to other S3 Storage Classes

### Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA)
S3 One Zone-IA is for data that is accessed less frequently, but requires rapid access when needed. Unlike other S3 Storage Classes which store data in a minimum of three Availability Zones (AZs), S3 One Zone-IA stores data in a single AZ and costs 20% less than S3 Standard-IA. S3 One Zone-IA is ideal for customers who want a lower-cost option for infrequently accessed data but do not require the availability and resilience of S3 Standard or S3 Standard-IA. It’s a good choice for storing secondary backup copies of on-premises data or easily re-creatable data. You can also use it as cost-effective storage for data that is replicated from another AWS Region using S3 Cross-Region Replication.

S3 One Zone-IA offers the same high durability†, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval fee. S3 Storage Classes can be configured at the object level, and a single bucket can contain objects stored across S3 Standard, S3 Intelligent-Tiering, S3 Standard-IA, and S3 One Zone-IA. You can also use S3 Lifecycle policies to automatically transition objects between storage classes without any application changes.

#### Key Features:

* Same low latency and high throughput performance of S3 Standard
* Designed for durability of 99.999999999% of objects in a single Availability Zone†
* Designed for 99.5% availability over a given year
* Backed with the Amazon S3 Service Level Agreement for availability
* Supports SSL for data in transit and encryption of data at rest
* S3 Lifecycle management for automatic migration of objects to other S3 Storage Classes
† Because S3 One Zone-IA stores data in a single AWS Availability Zone, data stored in this storage class will be lost in the event of Availability Zone destruction.

### ARCHIVE
### Amazon S3 Glacier (S3 Glacier)
S3 Glacier is a secure, durable, and low-cost storage class for data archiving. You can reliably store any amount of data at costs that are competitive with or cheaper than on-premises solutions. To keep costs low yet suitable for varying needs, S3 Glacier provides three retrieval options that range from a few minutes to hours. You can upload objects directly to S3 Glacier, or use S3 Lifecycle policies to transfer data between any of the S3 Storage Classes for active data (S3 Standard, S3 Intelligent-Tiering, S3 Standard-IA, and S3 One Zone-IA) and S3 Glacier.

#### Key Features:

* Designed for durability of 99.999999999% of objects across multiple Availability Zones
* Data is resilient in the event of one entire Availability Zone destruction
* Supports SSL for data in transit and encryption of data at rest
* Low-cost design is ideal for long-term archive
* Configurable retrieval times, from minutes to hours
* S3 PUT API for direct uploads to S3 Glacier, and S3 Lifecycle management for automatic migration of objects

### Amazon S3 Glacier Deep Archive (S3 Glacier Deep Archive)
S3 Glacier Deep Archive is Amazon S3’s lowest-cost storage class and supports long-term retention and digital preservation for data that may be accessed once or twice in a year. It is designed for customers — particularly those in highly-regulated industries, such as the Financial Services, Healthcare, and Public Sectors — that retain data sets for 7-10 years or longer to meet regulatory compliance requirements. S3 Glacier Deep Archive can also be used for backup and disaster recovery use cases, and is a cost-effective and easy-to-manage alternative to magnetic tape systems, whether they are on-premises libraries or off-premises services. S3 Glacier Deep Archive complements Amazon S3 Glacier, which is ideal for archives where data is regularly retrieved and some of the data may be needed in minutes. All objects stored in S3 Glacier Deep Archive are replicated and stored across at least three geographically-dispersed Availability Zones, protected by 99.999999999% of durability, and can be restored within 12 hours.

#### Key Features:

* Designed for durability of 99.999999999% of objects across multiple Availability Zones
* Lowest cost storage class designed for long-term retention of data that will be retained for 7-10 years
* Ideal alternative to magnetic tape libraries
* Retrieval time within 12 hours
* S3 PUT API for direct uploads to S3 Glacier Deep Archive, and S3 Lifecycle management for automatic migration of objects

## Amazon DynamoDB
>Fast and flexible NoSQL database service for any scale

Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. DynamoDB lets you offload the administrative burdens of operating and scaling a distributed database so that you don't have to worry about hardware provisioning, setup and configuration, replication, software patching, or cluster scaling. DynamoDB also offers encryption at rest, which eliminates the operational burden and complexity involved in protecting sensitive data. 

With DynamoDB, you can create database tables that can store and retrieve any amount of data and serve any level of request traffic. You can scale up or scale down your tables' throughput capacity without downtime or performance degradation. You can use the AWS Management Console to monitor resource utilization and performance metrics.

DynamoDB provides on-demand backup capability. It allows you to create full backups of your tables for long-term retention and archival for regulatory compliance needs. 

You can create on-demand backups and enable point-in-time recovery for your Amazon DynamoDB tables. Point-in-time recovery helps protect your tables from accidental write or delete operations. With point-in-time recovery, you can restore that table to any point in time during the last 35 days. 

DynamoDB allows you to delete expired items from tables automatically to help you reduce storage usage and the cost of storing data that is no longer relevant. 

### High Availability and Durability
DynamoDB automatically spreads the data and traffic for your tables over a sufficient number of servers to handle your throughput and storage requirements, while maintaining consistent and fast performance. All of your data is stored on solid-state disks (SSDs) and is automatically replicated across multiple Availability Zones in an AWS Region, providing built-in high availability and data durability. You can use global tables to keep DynamoDB tables in sync across AWS Regions.

### BENEFITS
#### Performance at scale
DynamoDB supports some of the world’s largest scale applications by providing consistent, single-digit millisecond response times at any scale. You can build applications with virtually unlimited throughput and storage. DynamoDB global tables replicate your data across multiple AWS Regions to give you fast, local access to data for your globally distributed applications. For use cases that require even faster access with microsecond latency, DynamoDB Accelerator (DAX) provides a fully managed in-memory cache.

#### No servers to manage
DynamoDB is serverless with no servers to provision, patch, or manage and no software to install, maintain, or operate. DynamoDB automatically scales tables up and down to adjust for capacity and maintain performance. Availability and fault tolerance are built in, eliminating the need to architect your applications for these capabilities. DynamoDB provides both provisioned and on-demand capacity modes so that you can optimize costs by specifying capacity per workload, or paying for only the resources you consume.

#### Enterprise ready
DynamoDB supports ACID transactions to enable you to build business-critical applications at scale. DynamoDB encrypts all data by default and provides fine-grained identity and access control on all your tables. You can create full backups of hundreds of terabytes of data instantly with no performance impact to your tables, and recover to any point in time in the preceding 35 days with no downtime. DynamoDB is also backed by a service level agreement for guaranteed availability.

### APPLICATIONS
#### Serverless Web Apps
Build powerful web applications that automatically scale up and down. You don't need to maintain servers, and your applications have automated high availability.
![](https://d1.awsstatic.com/Test%20Images/MasonTests/Lambda_WebApplications.2139ddbc8a84f5564ee5846995f28c88e9db5c2d.png)

#### Mobile Backends
Use DynamoDB and AWS AppSync to build interactive mobile and web apps with real-time updates, offline data access, and data sync with built-in conflict resolution.
![](https://d1.awsstatic.com/Test%20Images/MasonTests/Lambda/Lambda_MobileBackends.35e0e7cb2b8c1f7c276435c56e341916adb2033d.png)

#### Microservices
Build flexible and reusable microservices using DynamoDB as a serverless data store for consistent and fast performance.
![](https://d1.awsstatic.com/Test%20Images/MasonTests/Lambda/Lambda_StreamProcessing.8464961e382ff17c57750f7b1dc23c1ef7e4c233.png)

[Read More on DynamoDB >>](https://aws.amazon.com/dynamodb/)

## Summary
### Storage in the Cloud
Storage and database services in the cloud provide a place for companies to collect, store, and analyze the data they've collected over the years at a massive scale.

### Storage & Database Services
* Amazon Simple Storage Service (Amazon S3)
* Amazon Simple Storage Service (Amazon S3) Glacier
* DynamoDB
* Relational Database Service (RDS)
* Redshift
* ElastiCache
* Neptune
* Amazon DocumentDB

### S3 & S3 Glacier
Amazon Simple Storage Service (or S3) is an object storage system in the cloud.
#### Storage Classes
S3 offers several storage classes, which are different data access levels for your data at certain price points.
* S3 Standard
* S3 Glacier
* S3 Glacier Deep Archive
* S3 Intelligent-Tiering
* S3 Standard Infrequent Access
* S3 One Zone-Infrequent Access

#### Tips
* S3 is found under the Storage section on the AWS Management Console.
* A single object can be up to 5 terabytes in size.
* You can enable Multi-Factor Authentication (MFA) Delete on an S3 bucket to prevent accidental deletions.
* **S3 Acceleration** can be used to enable fast, easy, and secure transfers of files over long distances between your data source and your S3 bucket.

***

### DynamoDB
DynamoDB is a NoSQL document database service that is fully managed. Unlike traditional databases, NoSQL databases, are schema-less. Schema-less simply means that the database doesn't contain a fixed (or rigid) data structure.

#### Tips
* DynamoDB is found under the Database section on the AWS Management Console.
* DynamoDB can handle more than 10 trillion requests per day.
* DynamoDB is serverless as there are no servers to provision, patch, or manage.
* DynamoDB supports key-value and document data models.
* DynamoDB synchronously replicates data across three AZs in an AWS Region.
* DynamoDB supports GET/PUT operations using a primary key.