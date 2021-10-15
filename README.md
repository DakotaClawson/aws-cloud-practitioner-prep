<br />
<p align="center">
  <h2 align="center">AWS Cloud Practitioner Exam Prep</h2>
  <p align="center">
    A guide to preparing for the AWS Cloud Practitioner exam!
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View AWS Exam Guide</a>
    ·
    <a href="https://www.aws.training/Details/eLearning?id=60697">AWS Cloud Practitioner Essentials Course</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-exam">About The Exam</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#cloud-concepts">Cloud Concepts</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#technology">Technology</a></li>
    <li><a href="#security-&-compliance">Security & Compliance</a></li>
    <li><a href="#billing-&-pricing">Billing & Pricing</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

---

<!-- ABOUT THE EXAM -->

## About The Exam

[![Product Name Screen Shot][product-screenshot]](https://example.com)
Description of the exam and stuf...

---

<!-- CLOUD CONCEPTS -->

## Cloud Concepts ☁️

### What is Cloud Computing?

The on-demand delivery of IT resources over the internet with pay-as-you-go pricing.
<br />

_Read more [here](https://aws.amazon.com/what-is-cloud-computing/)._

### What are the benefits of Cloud Computing?

<b> Agility </b>

- Access new resources within minutes!
  <br />

<b> Elasticity </b>

- No more guessing capactiy, the cloud will grow and shrink with your needs.
  <br />

<b> Cost Savings </b>

- The aggregated cloud usage from a large number of customers results in lower pay-as-you-go prices.
  <br />

<b> Deploy Globally in Minutes </b>

- Deploy applications to customers around the world quickly with LOW latency.

### Deployment Models

1. Cloud Based

- Run all parts of the application in the cloud.
- Migrate existing applications to the cloud.
- Design and build new applications in the cloud.

2. On-Premises (Private)

- Deploy resources by using virtualization and resource management tools.
- Increase resource utilization by using application management and virtualization technologies.

3. Hybrid

- Connect cloud-based resources to on-premises infrastructure.
- Integrate cloud-based resources with legacy IT applications.

### Types of Cloud Computing

1. <b> Infrastructure as a Service (IaaS) </b>
   <br/>
   Think of this as a foundation... you're just laying building blocks! 🧱

   - First layer / Lowest Level
   - Computer, Network, Storage
   - Flexible
   - Users: Traditional IT, Government, Universities

2. <b> Platform as a Service (PaaS) </b>
   <br/>
   Need to run a python web app? Need to be able to support Node.js? No problem! Support within a click of a button. ✅

   - Second Layer
   - Removes management of underlying hardware
   - Macroscopic Planning
   - Users: Individuals, Developers, Small Startups

3. <b> Software as a Service (SaaS) </b>
   <br/>
   Want to get something done without worrying about the logistics of how to do it? Simply sign in and start on your task! 👩‍💻

   - Third Layer / Highest Level
   - Capabilities and Hardware are abstracted
   - End User Software (Marketing, Email Services, etc...)
   - Users: Non-technical Users, Office, Students

### Compute in the Cloud

<h3 align="center">Amazon Elastic Compute Cloud (Amazon EC2)</h3>

Think of a server in a coffee shop. A customer makes a request (small cup of coffee) to the server. The server executes this request and delivers it to the customer (or client). Amazon EC2 is the server in this scenario.

<b>How Amazon EC2 works</b>

1. Launch an instance
2. Connect to an instance
3. Use it! 🎉

EC2 runs on top of physical host machines managed by AWS using virtualization technology (Virtual Machines).

- This idea of sharing underlying hardware is called multitenancy.

<b>Amazon EC2 Instance Types</b>
<br />
Each EC2 instance type is grouped under an instance family.
<br />

- General Purpose
  - balanced resources
- Compute Optimized
  - high performance processors
- Memory Optimized
  - process large datasets
- Accelerated Computing
  - hardware accelerators
- Storage Optimized
  - high, sequential read and write access to large datasets on local storage

<b>Amazon EC2 Purchase Options</b>
<br />
You only pay for the compute time that you use
<br />

- On-demand
  - short-term irregular workloads
  - most flexible with NO contract
- Amazon EC2 Savings Plans
  - commit to a 1-year or 3-year term
  - up to 72% off over On-Demand
- Reserved Instances
  - predictable usage
  - pay all, partial, or none up-front
  - commit to a 1-year or 3-year term
- Spot Instances
  - do not require contracts or commitments
  - use unused Amazon EC2 computing capacity (AWS can reclaim at any time)
  - up to 90% off On-Demand
- Dedicated Hosts
  - fully dedicated to your use

<b>Amazon EC2 Auto Scaling</b>
<br />
Enables you to automatically add or remove Amazon EC2 instances in response to changing application demand.
<br />

- Dynamic scaling --> responds to changing demand.
- Predictive scaling --> automatically schedules the right number of Amazon EC2 instances based on predicted demand.

Set Number of EC2 Instances:
<br />

- <i>Minimum capacity</i> is the number of Amazon EC2 instances that launch immediately after you have created the Auto Scaling group.
- <i>Desired capactiy</i>
- <i>Maximum capacity</i>

<b>Elastic Load Balancing</b>
<br />
Enables you to automatically add or remove Amazon EC2 instances in response to changing application demand.
<br />
In short, this works to evenly distribute traffic so servers don't get overwhelmed!
<br />

<b>Messaging and queuing</b>
<br />
<i>Monolithic application</i>: when one component fails, all fail.
<br />
A <i>microservices approach</i> solves this issue with loosely coupled components.
<br />

> <b>Amazon Simple Queue Service (Amazon SQS)</b> <br />
> Send, store, and receive messages between software components, without losing messages or requiring other services to be available.
>
> - Messages remain in queue until consumed OR deleted.

> <b>Amazon Simple Notification Service (Amazon SNS)</b> <br />
> A publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers.

### Additional Compute Services

1.  Serverless Computing

    The term “serverless” means that your code runs on servers, but you do not need to provision or manage these servers.

    🧠 Focus more on innovating new products and features instead of maintaining servers.

    > <b> AWS Lambda </b> <br />
    > Service that lets you run code WITHOUT needing to provision or manage servers.
    >
    > - Only pay for the compute time you consume
    > - Run code with zero administration

2.  Containers

    A standard way to package your application's code and dependencies into a single object.

    The following services provide container orchestration:

    > <b> Amazon Elastic Container Service (Amazon ECS) </b> <br />
    > Highly scalable, high-performance container management system that enables you to run and scale containerized applications on AWS.
    >
    > - Supports Docker 🐋
    > - Build, test, and deploy applications quickly

- > <b>Amazon Elastic Kubernetes Service (Amazon EKS)</b> <br />
  > Fully managed service that you can use to run Kubernetes on AWS.
  >
  > - Deploy and manage containerized applications at scale

You can use these services with EC2 instances OR:

> <b>AWS Fargate</b> <br />
> Serverless compute engine for containers. It works with both Amazon ECS and Amazon EKS.

- Manages your server infrastructure for you

### Global Infrastructure and Reliability

<br />
Data center clusters 🏢 → Availability Zones 📍 → Regions 🌎
<br />
<br />
There are cloud centers all over the world... need to expand your user base to Ireland? No problem- just one click away.
<br />
<br />
<b> Region </b>

Data centers are built in REGIONS. This ensures there is always coverage in case of any issues. (i.e natural disasters)
User will choose which region they want to run out of.

Factors in picking a region:

- Compliance (Regulations, laws, etc)
- Proximity (Where's your customers?)
- Feature Availability (Region may not have the features you want due to hardware)
- Pricing (Some locations are more expensive to operate in)

<b> Availability Zone </b>

A single data center or a group of data centers within a Region.

<b> Edge Location </b>

> <b>Amazon CloudFront</b> <br />
> A content delivery service. It uses a network of edge locations to cache content and deliver content to customers all over the world.

> <b>AWS Outposts</b> <br />
> AWS will build and store a mini-region in your own data center.

### Utilizing AWS Services

In AWS, EVERYTHING is an API call (application programming interface).

Interact using:

> <b>AWS Management Console</b>

> <b> AWS Command Line Interface (CLI) </b>

> <b> AWS Software Development Kits (SDKs) </b> <br/>
> Enables you to use AWS services with your existing applications or create entirely new applications that will run on AWS.

Provision Amazon EC2-based environments:

> <b>AWS Elastic Beanstalk</b><br />
> Helps you focus on business app, NOT infrastructure. <br />
> Deploys the resources necessary to perform the following tasks:
>
> - Adjust capacity
> - Load balancing
> - Automatic scaling
> - Application health monitoring

> <b>AWS CloudFormation</b><br />
> Infrastructure as code tool allows you to define wide variety of AWS resources. <br />
> Use JSON or yml text files to create a template for your environment.

---

<!-- TECHNOLOGY -->

## Technology 💻

### Connecting to AWS

<b> Virtual Private Cloud (VPC) </b> <br/>
Your own private network in AWS. A VPC allows you to define your private IP range for your AWS resources, and you place things like EC2 instances and ELBs inside of your VPC.

_Note: You place things into different subnets._

<b> Subnets </b> <br />
Chunks of IP addresses in your VPC that allow you to group resources together.

<b> Internet Gateway (IGW) </b> <br />
Attaching this to your VPC allows public traffic from the internet to access your VPC.

- Think of an internet gateway as being similar to a doorway that customers use to enter a coffee shop.

<b> Virtual Private Gateway </b> <br />
Allows access to private resources in a VPC.

- You are still using the same road as everyone else, but with an extra layer of protection. (Think of a bodyguard 💪)

> <b> AWS Direct Connect </b> <br />
> Enables you to establish a dedicated private connection between your on-premises data center and a VPC.
>
> - helps you to reduce network costs
> - increase the amount of bandwidth that can travel through your network

### Subnets and network access control lists

<b> Packet </b> <br />
A unit of data sent over the internet or a network.

<b> Network Access Control List (ACL) </b> <br />
Virtual firewall that controls inbound and outbound traffic at the subnet level.

- Think of it this as a passport control officer for 'packets'! 🛂

<b>Stateless Packet Filtering</b> <br />
They remember nothing and check packets that cross the subnet border each way: inbound and outbound.

_Stateless ALLOWS all inbound traffic by default._ 🟢

<b>Stateful Packet Filtering</b> <br />
They remember previous decisions made for incoming packets. <br />

The VPC that checks the packet permissions is known as a <b>Security Group</b>. <br />

_Stateful DENIES all inbound traffic by default._ 🔴

### Global Networking

<b>Domain Name System (DNS)</b><br />
The phonebook of the internet! DNS resolution is the process of translating a domain name to an IP address.

> <b>Amazon Route 53</b><br />
> a DNS web service. It gives customers a reliable way to route end users to internet applications hosted in AWS.
>
> - manage the DNS records for domain names

### Databases and Storage

<b>Instance Store</b><br />
Temporary block-level storage for an Amazon EC2 instance.

- Disk storage that is physically attached to the host computer for an EC2 instance
- When the instance is terminated, you LOSE any data in the instance store

> <b>Amazon Elastic Block Store (Amazon EBS)</b><br />
> Provides block-level storage volumes that you can use with Amazon EC2 instances.
>
> - If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available
> - Stores data in a _single_ Availability Zone.

<b>EBS Snapshot</b><br />

- First backup taken of a volume copies all the data
- Subsequent backups only saves the blocks of data that have changed

<b>Object Storage</b><br />
Each object consists of:

- data
- metadata
- key

> <b>Amazon Simple Storage Service (Amazon S3)</b><br />
> Provides object-level storage, storing data as objects in buckets. 🪣
>
> - Max object file size is 5 TB
> - Configure R/W permissions
> - Version control

<b>Amazon S3 Storage Classes</b>

When choosing, consider these two factors:

1. How often you plan to retrieve your data
2. How available you need your data to be

_Sorted by price: High to Low_

- <b>Standard</b>

  - Frequently accessed data
  - Stores data in a minimum of three Availability Zones

- <b>Standard-Infrequent Access (S3 Standard-IA)</b>

  - Infrequently accessed data
  - Similar to S3 Standard but has a lower storage price and higher retrieval price

- <b>One Zone-Infrequent Access (S3 One Zone-IA)</b>

  - Stores data in a single Availability Zone
  - Has a lower storage price than S3 Standard-IA
  - Save costs on storage
  - Good if you can reproduce your data in the event of an Availability Zone failure

- <b>Intelligent-Tiering</b>

  - Ideal for data with unknown or changing access patterns
  - Small monthly monitoring and automation fee per object

- <b>Glacier</b>

  - Low-cost storage designed for data archiving
  - Retrieve objects within a few minutes to hours
  - Ideal for data archiving

- <b>Glacier Deep Dive</b>
  - Lowest-cost object storage class ideal for archiving
  - Retrieve objects within 12 hours

<b>Amazon EBS vs Amazon S3</b>

Using complete objects or only occasional changes? S3 is victorious.

- S3 uses 'object' storage, meaning if changes are made the WHOLE file needs to be uploaded.

Doing complex read, write, change functions? EBS is your knockout winner.

- EBS uses 'block' storage, meaning only the changes made are uploaded.

> <b>Amazon Elastic File System (Amazon EFS)</b><br />
> Scalable file system used with AWS Cloud services and on-premises resources.
>
> - Stores data across _multiple_ Availability Zones

> <b>Amazon Relational Database Service (Amazon RDS)</b><br />
> Enables you to run relational databases in the AWS Cloud. <br />
> Automates tasks such as hardware provisioning, database setup, patching, and backups.
>
> - Uses more overhead because the DB is more complex
> - SQL

<b>Amazon RDS database engines</b><br />
Amazon RDS is available on _six_ database engines:

1. Amazon Aurora
2. PostgreSQL
3. MySQL
4. MariaDB
5. Oracle Database
6. Microsoft SQL Server

<b>Amazon Aurora</b><br />
An enterprise-class relational database

- Compatible with MySQL and PostgreSQL relational databases
- Replicates six copies of your data across three Availability Zones
- Continuously backs up your data to Amazon S3

> <b>Amazon DynamoDB</b><br />
> Key-value database service for non-relational database schemas. <br />
>
> - Serverless (don't have to maintain servers or install OS)
> - Automatically scales to fit capacity
> - No SQL
> - Very fast

> <b>Amazon Redshift</b><br />
> Data warehousing service that you can use for big data analytics <br />
>
> - Collect data from many sources
> - Understand relationships and trends across your data

> <b>AWS Database Migration Service (AWS DMS)</b><br />
> Migrate relational databases, nonrelational databases, and other types of data stores. <br />
>
> - Collect data from many sources
> - Understand relationships and trends across your data <br />
>   Works well for:
> - DB consolidation
> - Continous replication
> - Development and test migrations

### Additional Database Services

- <b>Amazon DocumentDB</b><br />
  - document database service that supports MongoDB workloads
- <b>Amazon Neptune</b><br />
  - a graph database service
- <b>Amazon Quantum Ledger Database (Amazon QLDB)</b><br />
  - a ledger database service allows you to review a complete history of all changes
- <b>Amazon Manages Blockchain</b><br />
  - create and manage blockchain networks with open-source frameworks
- <b>Amazon ElastiCache</b><br />
  - adds caching layers on your databases to improve read times of common requests
- <b>Amazon DynamoDB Accelerator</b><br />
  - in-memory cache for DynamoDB improves response times

---

<!-- SECURITY & COMPLIANCE -->

## Security & Compliance 🔒

---

<!-- BILLING & PRICING -->

## Billing & Pricing 💵

<!-- RESOURCES -->

## Resources

- [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
- [Img Shields](https://shields.io)
- [Choose an Open Source License](https://choosealicense.com)
- [GitHub Pages](https://pages.github.com)
- [Animate.css](https://daneden.github.io/animate.css)
- [Loaders.css](https://connoratherton.com/loaders)
- [Slick Carousel](https://kenwheeler.github.io/slick)
- [Smooth Scroll](https://github.com/cferdinandi/smooth-scroll)
- [Sticky Kit](http://leafo.net/sticky-kit)
- [JVectorMap](http://jvectormap.com)
- [Font Awesome](https://fontawesome.com)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
