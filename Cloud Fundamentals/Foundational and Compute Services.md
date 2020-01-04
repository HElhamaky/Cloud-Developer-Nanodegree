## Amazon EC2
> Secure and resizable compute capacity in the cloud. Launch applications when needed without upfront commitments.

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides ** resizable ** compute capacity in the cloud. It is designed to make web-scale computing easier for developers.

Amazon EC2’s simple web service interface allows you to obtain and configure capacity with **minimal friction**. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment. Amazon EC2 *reduces the time* required to obtain and boot new server instances to minutes, allowing you to *quickly scale capacity*, both up and down, as your computing requirements change. Amazon EC2 changes the economics of computing by allowing you to *pay only for capacity* that you actually use. Amazon EC2 provides developers the tools to build *failure resilient applications* and isolate themselves from common failure scenarios.

### Benefits
#### ELASTIC WEB-SCALE COMPUTING
Amazon EC2 enables you to increase or decrease capacity within minutes, not hours or days. You can commission one, hundreds or even thousands of server instances simultaneously. Of course, because this is all controlled with web service APIs, your application can automatically scale itself up and down depending on its needs.
#### COMPLETELY CONTROLLED
You have complete control of your instances. You have root access to each one, and you can interact with them as you would any machine. You can stop your instance while retaining the data on your boot partition and then subsequently restart the same instance using web service APIs. Instances can be rebooted remotely using web service APIs. You also have access to console output of your instances.
#### FLEXIBLE CLOUD HOSTING SERVICES
You have the choice of multiple instance types, operating systems, and software packages. Amazon EC2 allows you to select a configuration of memory, CPU, instance storage, and the boot partition size that is optimal for your choice of operating system and application. For example, your choice of operating systems includes numerous Linux distributions, and Microsoft Windows Server.
#### DESIGNED FOR USE WITH OTHER AMAZON WEB SERVICES
Amazon EC2 works in conjunction with Amazon Simple Storage Service (Amazon S3), Amazon Relational Database Service (Amazon RDS) and Amazon Simple Queue Service (Amazon SQS) to provide a complete solution for computing, query processing and storage across a wide range of applications.
#### RELIABLE
Amazon EC2 offers a highly reliable environment where replacement instances can be rapidly and predictably commissioned. The service runs within Amazon’s proven network infrastructure and datacenters.
#### SECURE
Amazon EC2 works in conjunction with Amazon VPC to provide security and robust networking functionality for your compute resources. Your compute instances are located in a Virtual Private Cloud (VPC) with an IP range that you specify. You decide which instances are exposed to the Internet and which remain private.

* Security Groups and networks ACLs allow you to control inbound and outbound network access to and from your instances.
* You can provision your EC2 resources as Dedicated Instances. Dedicated Instances are Amazon EC2 Instances that run on hardware dedicated to a single customer for additional isolation.
* If you do not have a default VPC you must create a VPC and launch instances into that VPC to leverage advanced networking features such as private subnets, outbound security group filtering, network ACLs and Dedicated Instances.

#### INEXPENSIVE
Amazon EC2 passes on to you the financial benefits of Amazon’s scale. You pay a very low rate for the compute capacity you actually consume.

* **On-Demand Instances**
    * On-Demand Instances let you pay for compute capacity by the hour with no long-term commitments. This frees you from the costs and complexities of planning, purchasing, and maintaining hardware and transforms what are commonly large fixed costs into much smaller variable costs. On-Demand Instances also remove the need to buy “safety net” capacity to handle periodic traffic spikes.

* **Reserved Instances**
    * Reserved Instances provide you with a significant discount compared to On-Demand Instance pricing. There are three Reserved Instance payment options (No Upfront, Partial Upfront, All Upfront) that enable you to balance the amount you pay upfront with your effective hourly price.

* **Spot instances**
    * Spot instances are spare compute capacity in the AWS cloud available to you at steep discounts compared to On-Demand prices. EC2 Spot enables you to optimize your costs on the AWS cloud and scale your application's throughput up to 10X for the same budget. By simply selecting Spot when launching EC2 instances, you can save up-to 90% on On-Demand prices.

* **Dedicated Host**
    * An Amazon EC2 Dedicated Host is a physical server with EC2 instance capacity fully dedicated to your use. Dedicated Hosts can help you address compliance requirements and reduce costs by allowing you to use your existing server-bound software licenses including Microsoft Windows Server, Microsoft SQL Server, SUSE Linux Enterprise Server, Red Hat Enterprise Linux, or other software licenses that are bound to VMs, sockets, or physical cores, subject to your license terms.

#### EASY TO START
Quickly get started with Amazon EC2 by visiting the AWS Management Console to choose preconfigured software on Amazon Machine Images (AMIs). You can quickly deploy this software to EC2 via the EC2 console.



## Amazon Elastic Block Store (Amazon EBS)
Amazon Elastic Block Store (Amazon EBS) provides **block level storage volumes** for use with EC2 instances. EBS volumes **behave like raw, unformatted block devices**. You can mount these volumes as devices on your instances. You can **mount multiple volumes** on the same instance, but each volume can be **attached to only one instance at a time**. You can create a **file system** on top of these volumes, or **use them in any way** you would use a block device (like a hard drive). You can **dynamically change the configuration of a volume** attached to an instance.

EBS volumes are **highly available and reliable storage volumes** that can be attached to any running instance that is in the **same Availability Zone**. EBS volumes that are attached to an EC2 instance are exposed as storage volumes that **persist independently from the life of the instance**. With Amazon EBS, you **pay only for what you use**. For more information about Amazon EBS pricing, see the Projecting Costs section of the [Amazon Elastic Block Store page](http://aws.amazon.com/ebs/).

You can **attach multiple volumes** to the same instance within the limits specified by your AWS account. Your account has a limit on the number of EBS volumes that you can use, and the total storage available to you. For more information about these limits, and how to request an increase in your limits, see [Request to Increase the Amazon EBS Volume Limit](https://console.aws.amazon.com/support/home#/case/create?issueType=service-limit-increase&limitType=service-code-ebs).

Amazon EBS is recommended when data must be quickly accessible and requires **long-term persistence**. EBS volumes are particularly well-suited for use as the **primary storage for file systems, databases, or for any applications** that require *fine granular updates and access to raw, unformatted, block-level storage*. Amazon EBS is well suited to both **database-style applications** that *rely on random reads and writes*, and to **throughput-intensive applications** that *perform long, continuous reads and writes*.

[Read More on EBS >>](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)

## Virtual Private Cloud (VPC)
A virtual private cloud (VPC) is an on-demand configurable pool of shared computing resources allocated within a public cloud environment, providing a certain level of isolation between the different organizations (denoted as users hereafter) using the resources. 

The isolation between one VPC user and all other users of the same cloud (other VPC users as well as other public cloud users) is achieved normally through allocation of a private IP subnet and a virtual communication construct (such as a VLAN or a set of encrypted communication channels) per user. 

In a VPC, the previously described mechanism, providing isolation within the cloud, is accompanied with a VPN function (again, allocated per VPC user) that secures, by means of authentication and encryption, the remote access of the organization to its VPC resources. 

With the introduction of the described isolation levels, an organization using this service is in effect working on a 'virtually private' cloud (that is, as if the cloud infrastructure is not shared with other users), and hence the name VPC.

VPC is most commonly used in the context of cloud infrastructure as a service. In this context, the infrastructure provider, providing the underlying public cloud infrastructure, and the provider realizing the VPC service over this infrastructure, may be different vendors.

## Amazon Virtual Private Cloud
> Provision a logically isolated section of the AWS cloud where you can launch AWS resources in a virtual network that you define

Amazon Virtual Private Cloud (Amazon VPC) lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define.

You have complete control over your virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. You can use both IPv4 and IPv6 in your VPC for secure and easy access to resources and applications.

You can easily customize the network configuration of your Amazon VPC. For example, you can create a public-facing subnet for your web servers that have access to the internet. You can also place your backend systems, such as databases or application servers, in a private-facing subnet with no internet access. You can use multiple layers of security, including security groups and network access control lists, to help control access to Amazon EC2 instances in each subnet.

### Benefits
#### Secure
Amazon VPC provides advanced security features, such as security groups and network access control lists, to enable inbound and outbound filtering at the instance and subnet level. In addition, you can store data in Amazon S3 and restrict access so that it’s only accessible from instances inside your VPC. For additional security, you can create dedicated instances that are physically isolated from other AWS accounts, at the hardware level.

#### Simple
Create a VPC quickly and easily using the AWS Management Console. Select from common network setups and find the best match for your needs. Subnets, IP ranges, route tables, and security groups are automatically created. You spend less time setting up and managing, so you can concentrate on building the applications that run in your VPCs.

#### Customizable
Control your virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. Customize the network configuration, such as by creating a public-facing subnet for your webservers that has access to the internet, and placing your backend systems such as databases or application servers in a private-facing subnet with no internet access.

[Read More on Amazon VPC >>](https://aws.amazon.com/vpc/)

### Amazon VPC Concepts
Amazon VPC is the **networking layer** for Amazon EC2.

The following are the key concepts for VPCs:

* A *virtual private cloud* (VPC) is a virtual network dedicated to your AWS account.

* A *subnet* is a range of IP addresses in your VPC.

* A *route table* contains a set of rules, called routes, that are used to determine where network traffic is directed.

* An *internet gateway* is a horizontally scaled, redundant, and highly available VPC component that allows communication between instances in your VPC and the internet. It therefore imposes no availability risks or bandwidth constraints on your network traffic.

* A VPC *endpoint* enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered by PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection. Instances in your VPC do not require public IP addresses to communicate with resources in the service. Traffic between your VPC and the other service does not leave the Amazon network.

### Accessing Amazon VPC
You can create, access, and manage your VPCs using any of the following interfaces:

* **AWS Management Console**— Provides a web interface that you can use to access your VPCs.

* **AWS Command Line Interface (AWS CLI)** — Provides commands for a broad set of AWS services, including Amazon VPC, and is supported on Windows, Mac, and Linux. 

* **AWS SDKs** — Provides language-specific APIs and takes care of many of the connection details, such as calculating signatures, handling request retries, and error handling. 

* **Query API**— Provides low-level API actions that you call using HTTPS requests. Using the Query API is the most direct way to access Amazon VPC, but it requires that your application handle low-level details such as generating the hash to sign the request, and error handling. 

[Read More from Amazon VPC Documentation >>](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)



## AWS Lambda
> Run code without thinking about servers. Pay only for the compute time you consume.

AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume.

With Lambda, you can run code for virtually any type of application or backend service - all with zero administration. Just upload your code and Lambda takes care of everything required to run and scale your code with high availability. You can set up your code to automatically trigger from other AWS services or call it directly from any web or mobile app.

### Benefits

#### NO SERVERS TO MANAGE
AWS Lambda automatically runs your code without requiring you to provision or manage servers. Just write the code and upload it to Lambda.

#### CONTINUOUS SCALING
AWS Lambda automatically scales your application by running code in response to each trigger. Your code runs in parallel and processes each trigger individually, scaling precisely with the size of the workload.

#### SUBSECOND METERING
With AWS Lambda, you are charged for every 100ms your code executes and the number of times your code is triggered. You pay only for the compute time you consume. 

#### CONSISTENT PERFORMANCE
With AWS Lambda, you can optimize your code execution time by choosing the right memory size for your function. You can also enable Provisioned Concurrency to keep your functions initialized and hyper-ready to respond within double digit milliseconds.

## Lambda Use cases
What can you build with AWS Lambda? Learn more about the use cases below:

### Data processing
You can use AWS Lambda to execute code in response to triggers such as changes in data, shifts in system state, or actions by users. Lambda can be directly triggered by AWS services such as S3, DynamoDB, Kinesis, SNS, and CloudWatch, or it can be orchestrated into workflows by AWS Step Functions. This allows you to build a variety of real-time serverless data processing systems.
#### REAL-TIME FILE PROCESSING
You can use Amazon S3 to trigger AWS Lambda to process data immediately after an upload. For example, you can use Lambda to thumbnail images, transcode videos, index files, process logs, validate content, and aggregate and filter data in real-time.

![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-RealTimeFileProcessing.a59577de4b6471674a540b878b0b684e0249a18c.png)

#### REAL-TIME STREAM PROCESSING
You can use AWS Lambda and Amazon Kinesis to process real-time streaming data for application activity tracking, transaction order processing, click stream analysis, data cleansing, metrics generation, log filtering, indexing, social media analysis, and IoT device data telemetry and metering.

![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-RealTimeStreamProcessing.d79d55b5f3a5d6b58142a6c0fc8a29eadc81c02b.png)

#### EXTRACT, TRANSFORM, LOAD
You can use AWS Lambda to perform data validation, filtering, sorting, or other transformations for every data change in a DynamoDB table and load the transformed data to another data store.
![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-ExtractTransformLoad.21c3171be43ce5afb20bf6e54b0a5054c05a0803.png)

### Backends
You can build serverless backends using AWS Lambda to handle web, mobile, Internet of Things (IoT), and 3rd party API requests. Take advantage of Lambda’s consistent performance controls, such as multiple memory configurations and Provisioned Concurrency, for building latency-sensitive applications at any scale.

#### WEB APPLICATIONS
By combining AWS Lambda with other AWS services, developers can build powerful web applications that automatically scale up and down and run in a highly available configuration across multiple data centers – with zero administrative effort required for scalability, back-ups or multi-data center redundancy.
![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-WebApplications%202.c7f8cf38e12cb1daae9965ca048e10d676094dc1.png)

#### IOT BACKENDS
You can build serverless backends using AWS Lambda to handle web, mobile, Internet of Things (IoT), and 3rd party API requests.
![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-IoTBackends.3440c7f50a9b73e6a084a242d44009dc0fbe5fab.png)

#### MOBILE BACKENDS
AWS Lambda makes it easy to create rich, personalized app experiences. You can build backends using AWS Lambda and Amazon API Gateway to authenticate and process API requests. Use AWS Amplify to easily integrate your backend with your iOS, Android, Web, and React Native frontends.
![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-MobileBackends_option2.00f6421e67e8d6bdbc59f3a2db6fa7d7f8508073.png)

[Getting Started With AWS Lambda >>](https://aws.amazon.com/lambda/) 

## AWS Elastic Beanstalk
> Easy to begin, Impossible to outgrow

AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS.

You can simply upload your code and Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring. At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time.

There is no additional charge for Elastic Beanstalk - you pay only for the AWS resources needed to store and run your applications.

Elastic Beanstalk supports applications developed in Go, Java, .NET, Node.js, PHP, Python, and Ruby. When you deploy your application, Elastic Beanstalk builds the selected supported platform version and provisions one or more AWS resources, such as Amazon EC2 instances, to run your application.

You can interact with Elastic Beanstalk by using the AWS Management Console, the AWS Command Line Interface (AWS CLI), or eb, a high-level CLI designed specifically for Elastic Beanstalk.

To use Elastic Beanstalk, you create an application, upload an application version in the form of an application source bundle (for example, a Java .war file) to Elastic Beanstalk, and then provide some information about the application. Elastic Beanstalk automatically launches an environment and creates and configures the AWS resources needed to run your code. After your environment is launched, you can then manage your environment and deploy new application versions. The following diagram illustrates the workflow of Elastic Beanstalk.

![](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/images/clearbox-flow-00.png)

After you create and deploy your application, information about the application—including metrics, events, and environment status—is available through the AWS Management Console, APIs, or Command Line Interfaces, including the unified AWS CLI.

### Benefits

#### Fast and simple to begin
Elastic Beanstalk is the fastest and simplest way to deploy your application on AWS. You simply use the AWS Management Console, a Git repository, or an integrated development environment (IDE) such as Eclipse or Visual Studio to upload your application, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring. Within minutes, your application will be ready to use without any infrastructure or resource configuration work on your part.

#### Developer productivity
Elastic Beanstalk provisions and operates the infrastructure and manages the application stack (platform) for you, so you don't have to spend the time or develop the expertise. It will also keep the underlying platform running your application up-to-date with the latest patches and updates. Instead, you can focus on writing code rather than spending time managing and configuring servers, databases, load balancers, firewalls, and networks.

#### Impossible to outgrow
Elastic Beanstalk automatically scales your application up and down based on your application's specific need using easily adjustable Auto Scaling settings. For example, you can use CPU utilization metrics to trigger Auto Scaling actions. With Elastic Beanstalk, your application can handle peaks in workload or traffic while minimizing your costs.

#### Complete resource control
You have the freedom to select the AWS resources, such as Amazon EC2 instance type, that are optimal for your application. Additionally, Elastic Beanstalk lets you "open the hood" and retain full control over the AWS resources powering your application. If you decide you want to take over some (or all) of the elements of your infrastructure, you can do so seamlessly by using Elastic Beanstalk's management capabilities.

[More on AWS Elastic Beanstalk >> ](https://aws.amazon.com/elasticbeanstalk/)


## Summary

### Servers In The Cloud
Servers in the cloud have revolutionized the IT industry.

* Scale capacity up and down based on demands.
* Storage, more memory, and computing power can be added as needed.
* Obtain servers in minutes.
* No need for onsite hardware or capital expenses.

### Elastic Cloud Compute
Elastic Cloud Compute or EC2 is a foundational piece of AWS' cloud computing platform and is a service that provides servers for rent in the cloud.

#### Pricing Options
There are several pricing options for EC2.
* On Demand - Pay as you go, no contract.
* Dedicated Hosts - You have your own dedicated hardware and don't share it with others.
* Spot - You place a bid on an instance price. If there is extra capacity that falls below your bid, an EC2 instance is provisioned. If the price goes above your bid while the instance is running, the instance is terminated.
* Reserved Instances - You earn huge discounts if you pay up front and sign a 1-year or 3-year contract.

#### Tips
* EC2 is found under the Compute section of the AWS Management Console.
* Spot instances can save you up to 90% off the on-demand pricing.
* There are several instance types that provide varying combinations of CPU, memory, storage, and networking capacity.

***

### Elastic Block Store
Elastic Block Store (EBS) is a storage solution for EC2 instances and is a physical hard drive that is attached to the EC2 instance to increase storage.

#### Tips
* EBS is found on the EC2 Dashboard.
* There are several EBS volume types that fall under the categories of Solid State Drives (SSD) and Hard Disk Drives (HDD).

***

### Security
Security in the cloud allows you to have complete control over your virtual networking environment.

* Configure your virtual network with public or private facing subnets
* Launch your servers in the selected network to secure access

***

### Virtual Private Cloud (VPC)
Virtual Private Cloud or VPC allows you to create your own private network in the cloud. You can launch services, like EC2, inside of that private network. A VPC spans all the Availability Zones in the region.

VPC allows you to control your virtual networking environment, which includes:

* IP address ranges
* subnets
* route tables
* network gateways
#### Tips
* VPC is found under Networking & Content Delivery section of the AWS Management Console.
* The default limit is **5 VPCs per Region**. You can request an increase for these limits.
* Your AWS resources are automatically provisioned in a default VPC.
* There are no additional charges for creating and using the VPC.
* You can store data in Amazon S3 and restrict access so that it’s only accessible from instances in your VPC.

***

### Compute Power In The Cloud
Compute power in the cloud is a faster way to build applications, providing:

* no servers to manage (i.e. serverless)
* ability to continuously scale
* ability to run code on demand in response to events
* pay only when your code runs

***


### Lambda
AWS Lambda provides you with computing power in the cloud by allowing you to execute code without standing up or managing servers.
#### Tips
* Lambda is found under the Compute section on the AWS Management Console.
* Lambdas have a time limit of 15 minutes.
* The code you run on AWS Lambda is called a “Lambda function.”
* Lambda code can be triggered by other AWS services.
* AWS Lambda supports Java, Go, PowerShell, Node.js, C#/.NET, Python, and Ruby. There is a Runtime API that allows you to use other programming languages to author your functions.
* Lambda code can be authored via the console.

***

### Elastic Beanstalk
Elastic Beanstalks is an orchestration service that allows you to deploy a web application at the touch of a button by spinning up (or provisioning) all of the services that you need to run your application.

#### Tips
* Elastic Beanstalk is found under the Compute section of the AWS Management Console.
* Elastic Beanstalk can be used to deployed web applications developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker.
* You can run your applications in a VPC.


