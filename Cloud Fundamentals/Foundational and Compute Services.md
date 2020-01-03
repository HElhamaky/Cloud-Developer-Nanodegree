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

## Virtual Private Cloud
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


## Summary

#### Servers In The Cloud
Servers in the cloud have revolutionized the IT industry.

* Scale capacity up and down based on demands.
* Storage, more memory, and computing power can be added as needed.
* Obtain servers in minutes.
* No need for onsite hardware or capital expenses.

#### Elastic Cloud Compute
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

#### Elastic Block Store
Elastic Block Store (EBS) is a storage solution for EC2 instances and is a physical hard drive that is attached to the EC2 instance to increase storage.

#### Tips
* EBS is found on the EC2 Dashboard.
* There are several EBS volume types that fall under the categories of Solid State Drives (SSD) and Hard Disk Drives (HDD).

#### Security
Security in the cloud allows you to have complete control over your virtual networking environment.

* Configure your virtual network with public or private facing subnets
* Launch your servers in the selected network to secure access


#### Virtual Private Cloud (VPC)
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