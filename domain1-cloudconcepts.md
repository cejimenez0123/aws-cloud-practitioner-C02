## Domain 1: Cloud Concepts (24% of scored content)

![AWS Cloud Practitioner Domains](https://github.com/emiliedionisio/aws-cloud-practitioner-C02/blob/main/1-cloudconcepts.png)

#### 1.1: Define the benefits of the AWS Cloud
#### Knowledge of: Value proposition of the AWS Cloud
#### Skills in:
- Understanding the economies of scale (for example, cost savings)
- Understanding the benefits of global infrastructure (for example, speed of deployment, global reach)
- Understanding the advantages of high availability, elasticity, and agility

<!-- Type your questions and answers below -->

#### What is Cloud Computing?
Cloud computing is the on-demand delivery of IT resources over the internet with pay-as-you-go pricing. On-demand delivery indicates that AWS has the resources you need, when you need them. 

#### What are the three deployment models for cloud computing, their definitions, and uses?
- Cloud-based Deployment Model, you can migrate existing applications to the cloud, or you can design and build new applications in the cloud. You can build those applications on low-level infrastructure that requires your IT staff to manage them.
  - Run all parts of the application in the cloud.
  - Migrate existing applications to the cloud.
  - Design and build new applications in the cloud.
- On-premises deployment is also known as a private cloud deployment.  In this model, resources are deployed on premises by using virtualization and resource management tools.
  - Deploy resources by using virtualization and resource management tools.
  - Increase resource utilization by using application management and virtualization technologies.
- Hybrid deployment, cloud-based resources are connected to on-premises infrastructure. You might want to use this approach in a number of situations. For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.
  - Connect cloud-based resources to on-premises infrastructure.
  - Integrate cloud-based resources with legacy IT applications.




### What are the Benefits of cloud computing and their definitions?
  - Trade fixed expense for variable expense – Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can pay only when you consume computing resources, and pay only for how much you consume.

  - Benefit from massive economies of scale – By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers is aggregated in the cloud, providers such as AWS can achieve higher economies of scale, which translates into lower pay as-you-go prices.??? Lower cost per indivdual user?

  - Stop guessing capacity – No longer worry if you have high enough infrastructure capaciy, no idle resources when it is not being used. Able to scale up in a few minutes.

  - Increase speed and agility – In a cloud computing environment, new IT resources are only a click away, which means that you reduce the time to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower. ???

  - Stop spending money running and maintaining data centers – Focus on projects that differentiate you, rather than the infrastructure everyone needs like servers.

  - Go global in minutes – Low latency across the globe. Better experience at minimal cost to users.

###    What are the Amazon EC2 instance types and their definitions?
Instance types are the combination of features like CPU, memory, and storage that let you provide an optimize when to recieve resources.

???How is instance when it is part of the desktop. Instance vs AMI?

- General Purpose Instances
  - These instances offer a balanced mix of CPU, memory, storage, and networking resources, making them suitable for a wide range of applications.

    M7g, M6i, M6g, M5, M4, T4g, T3, T2: Popular choices for web servers, small to medium-sized databases, and development environments.

- Compute Optimized Instances
  - Prioritize raw compute power for applications demanding high CPU performance.
Ideal for batch processing, scientific simulations, and video encoding.

- Memory Optimized Instances
  - Designed for applications requiring large amounts of memory.
 Well-suited for in-memory databases, real-time data processing, and analytics.
 

- Storage Optimized Instances
  - Optimized for workloads that require high performance storage.

     Ideal for databases, data warehousing, and big data analytics.
     What's an example of big data

- Accelerated Computing Instances
 - Provide specialized hardware acceleration for specific workloads.
 Suitable for machine learning, deep learning, high-performance computing, and graphics-intensive applications.
Whats an example of real time data processing?
###   What is a Load Balancer?
Evenly distributes traffic between servers
###    What is the primary purpose of AWS Regions in the global infrastructure?
 AWS Regions offer low latency, low packet loss(data fidelity, what is sent arrives), and high overall network quality.

### Describe the function of Amazon CloudFront in AWS's architecture.
  - Data distrubuted globally so information that far away from customer can be cached closer to the customer.
###    How do AWS Edge locations enhance the performance of Amazon CloudFront?
When a user requests content that you're serving with CloudFront, the request is routed to the edge location that provides the lowest latency (time delay), so that content is delivered with the best possible performance.
### Explain how Amazon Route 53 integrates with AWS Edge locations to enhance user experiences.
Route 53, a ?highly scalable DNS(router to other servers/domain/web pages) web service, acts as the traffic manager, directing users to the appropriate edge location based on various factors, including:

    Geographic location: Users are directed to the closest edge location for minimal latency.
    Health checks: Route 53 continuously monitors the health of edge locations and redirects traffic if an issue arises.
    Traffic distribution: Load balancing can be implemented to distribute traffic evenly across multiple edge locations.
###  
### How are AWS Lambda and AWS Outposts different in what they offer for cloud computing?

AWS Lambda 
**AWS Lambda is ideal for serverless, event-driven computing tasks that need to scale automatically and are short-lived.**
  - Severless Computing
    - No need to provision servers. Only pay when used.
  - Event Driven
    - Lambda responds to events such as change data in S3 bucket, updates to a DynamoDB table, or HTTP requests via Amazon Gateway 
    Amazon Gateway?(API)
  - Automatic Scaling
    - Scales precise with the workload. Runs in response to each individual trigger
  - Short lived tasks
    - Best suited for short lived tasks
  - Usage Model
    - Pay only for what you use

AWS Outposts
**AWS Outposts is perfect for enterprises looking for a consistent AWS hybrid cloud experience, with applications that need to remain on-premises for compliance, low latency, or local data processing.**
  - Hybrid Cloud
    - AWS infrastructure are extended to any center,co-location, or on premises in limited space or smaller capacity requirements
  - On-Premises Deployment
    - low latency access to on-premises systems, local data processing, or the need to comply with **data residency requirements**.
  - Consistent AWS experiences
    - Same AWS hardware and software infrastructure. Able to use **AWS services, APIs, and tools on-premises**
  - Longer Term Workloads
    - **Suitable for extended workloads or require significant on premises infrastructure**
  - Usage Model
    - Purchasing hardware commiting to a usage model similar on premises, but they have AWS tools and infrastructure 
### What is high availability?
  Managing of large workloads efficently for extended periods of time
### What are the benefits of AWS having a global infrastructure with multiple regions?
  - **Low Latency**
    - Built close to end users
  - **Disaster Recovery and fault tolerance**
    - Fail over - if one location fails, resources are available at another location
    - Geographical Redundancy - if one region fails, can continue to work at other regions
### What is an AWS Region?
  A geographical area with multiple availability zones(locations of centers)
### Why is data sovereignty important in AWS Regions?
  - Compliance with local laws
    - Some industried are required to keep information within the country
  - Data Privacy
    - Protection from foreign gov't
    - Avoid cross border transfers
  - Data Control and Security
    - Country specific security measures
  - Reliability and Availability
    - Closer to organizations for performance and disaster recovery
### How do AWS Regions enhance disaster recovery capabilities?
  - Geographical Redundacy
### What are the four main factors to consider when choosing an AWS Region?
  - **Compliance**
  - Latency 
    - Reduced network latency imporves user experience
  - Cost
    - Some regions have lower cost than others
  - Services and features 
    - New features are rolled out gradually to new regions
### What is an AWS Availability Zone? 
  - A data center
### What is the purpose of having multiple Availability Zones within an AWS Region? 
  - **High Availability**
  - **Fault Isolation**
  - **Cost Efficency**
    - Spreading usage across availability zones, has potentional to reduce costs by optimizing resources
  - **Compliance and Data Residency**
### How does AWS ensure low latency communication between Availability Zones?
### Why is it important to run EC2 instances across multiple AZs?
  - **High Availability**
    - If an AZ goes down, application remains available
    - **Load Balancing** balance traffic among healthy instances, ensuring consistent availability, and experience
  - **Scalability**
    - 
  - **Fault Tolerance**
    - AZ are isolated from each other
    - Redundancy: If one AZ fails others can takes the load
  - Disaster Recovery
  - Improved Performance
    - **Optimize resources** across regions with load balancer
      - Handle traffic spike efficently
      
### How do regional AWS services enhance high availability?
  - **Elastic Load Balancing between multiple AZ**
  - **Autoscaling: Adjusts based on active instances.** Helps maintain performance and availability during traffic spikes or failure at a specific AZ. 
  - **Cross region replication** AWS S3,RDS, and DynamoDB. Replicate data across different regions. Can failover(move traffic to a instance in case of regional outage)
### What is the purpose of Amazon CloudFront?
  - Cloudfront is a CDN ( content delivery network.) Reduce latency by migrating data to a region closer to users. Deliver web pages, images, video  to users with low latency.
  - **Caching frequently acceseed resources closer to users**
### What are edge locations in AWS?
  - **Protection from DDoS attacks with AWS Shield**
  - **Cloudfront offers encryption for ssl/tls and https.** Offers feattures
  like AWS WAF( Web Application Firewall)
  - **Content access controls**
  - Made to handle traffic spikes without impacting performance
### What is AWS Outposts?
  - **Outposts let's organization run AWS resources on premises would in cloud**
    - **Hybrid Cloud w/ Outpost**: Seamless experience, in case of increase traffic can run resources on cloud, in what's called cloud bursts
    - Local Data Storage Data Sovereignty
    - **Fully manaaged by AWS** AWS delivers,installs, and maintains outposts. Amazon handles software patches and updates just like in the cloud.
    - **Low Latency** integrates with onpremises data

### How do Availability Zones within AWS Regions contribute to disaster recovery and high availability?
  - AZ provide redundancy incase of failure of a seperate discrete outage at a another AZ. 
  - **Load Balancing with low latency**
  - Cost efficent avoid the higher cost of cross region data
  - **Simplifies audits and reduces complexity** for data sovereignty while still providing fault tolerance and disaster recovery capabilites.
### How do AWS Edge locations and Amazon CloudFront improve content delivery?
  Edge Locations cache resources closer to custoemers so they get information quicker.
### What is an API in the context of AWS?
Application Programming Interface, predertermined way to interact with AWS services
ex. Launch EC2 instance
### What is the primary method of interacting with AWS services?
  - AWS Management Console
    - USECASE:Best for beginners creating s3 buckets, and launching ec2 instances, managing IAM USERS
  - AWS SDK & API
    - Interact with AWS services programtically
    - RESTful API
    - USECASE: Accessing S3 storage, launching EC2 instances, or interacting with databases like DynamoDB
  - **Infrastructure as Code(IOC)** Tools
    - Define AWS infrastructure with JSON and YAML. Automates 
    - Terraform
    - USECASE: Managing complex enviroments, ensuring consistency, and automating the deployment of resources
  - AWS CLI
    - Script and automate tasks by executing commands directly from the terminal
    - Flexible: Helpful for repetitive tasks and CI/CD integration
    - USECASE: Suitable for Developers, DevOps Engineers, System adminstrators
### What are the main ways to interact with AWS services?
### Why is automation important in cloud deployment?
  - Efficency
  - Cost Management
    - **Optimize Resource Usage** Ensure you're only using what you need
    - Budget adherance
  - Security and Compliance
      - Consistent security practices
  - **Consistency and Reliability**

    - Compliance Automation
  - **Scalability**
    - Scale resources up or down based on demand
  - Disaster Recovery Resilience
    - Automated failover executed quickly and efficently.
  - Continuos Integration/ Continuos Deployment
### What is the primary advantage of using AWS Elastic Beanstalk over manual methods like the AWS Management Console?
### What is AWS Elastic Beanstalk used for?
Elastic Beanstalk is a service for deploying and scaling web applications and services. Upload your code and Elastic Beanstalk automatically handles the deployment—from capacity provisioning, load balancing, and auto scaling to application health monitoring.
### How does AWS CloudFormation help in managing AWS resources?
With CloudFormation we can modify and update the resources in your existing stacks in a controlled and predictable way. By using templates to manage your stack changes, you have the ability to apply version control to your AWS infrastructure just as you do with the software running on it.
### What are the main components of AWS Global Infrastructure?
### Which AWS services automatically run across multiple Availability Zones?
### What is the recommended best practice for deploying infrastructure in AWS?

####  What is Amazon EC2?
    - A webservice from AWS that creates scalable virtual servers
####   What is Amazon EC2 and its primary benefits?
  A web service from AWS that creates scalable virtual servers. Pay only for the compute time used. Auto scaling **Adjusting the number of instances, based on conditions. Can handle traffic automatical**

####  What is a Security Group in EC2?
    - A virtual firewall
    - controls inbound and outbound traffic from EC2 server instance
#### What are the four main purchasing options for EC2 instances, and what are their key characteristics?
   - **On Demand Instance**
    - For unpredictable, short term workload where flexibility is key.
   - **Reserved Instances**
    - For long term, steady state with predictable usage
   - **Spot Instances**
    - For cost sensitive, workloads that can handle interruptions
   - **Saving Plans**
    - More flexible, can get discount for consistent usage of **1 year and 3 year** terms
    
  #### How does EC2 pricing work?
    - **Pay As You Go**
      - BASED ON
        - Instance Type
        - Purchasing Options
        - Data Transfer Costs
        - Stoage Costs
   #### What is an Amazon Machine Image (AMI)?
    - Virtual Computer
    - Runs an OS (Linux, Windows, Unix)
    - Can come preconfigured with applications
   #### How does EC2 integrate with other AWS services?
    - **Amazon RDS** EC2 connect with RDS to manage and query database
      - Offload database management to RDS run logic on EC2
    - **Amazon S3** Use it for storing and retreiving data
      - Host Static Websites, media files, or back ups in S3
    - EC2 instances run within a VPC
    - **Amazon CloudWatch** Detailed monitoring of instance performance metrics I/O, network traffic, CPU
    - **Elastic Load Balancing** Load distribution accross EC2 instances. Ensures high availability and reliability.
   #### What are the different computing models available in AWS?
    - Compute Instance
      - ec2
    - Edge Instance 
      - Extends AWS functionality to local devices
    - High Performance Computing
      - EC2 instances for high performance computing tasks
    - Batch Processing
      - Efficently run batch computing workloads at any scale
      - USECASE: Scientic processing, data analysis
    - Platform as a Service
    - Container Based Computing
    What is an instance and its use cases?
    What are containers and their advantages?
    What is serverless computing and its use cases?
    When would you consider a hybrid deployment model?
    What are some of the popular AWS computing services?
    What is AWS Lambda?
    What is Amazon ECS?
    How does AWS Fargate differ from Amazon EC2?
    What are the benefits of using AWS Elastic Beanstalk?
    How does EC2 demonstrate elasticity?
    What level of control do users have over EC2 instances?
    How does EC2 integrate with other AWS services?
    What security features does Amazon EC2 provide?
    What are the main architectural components of Amazon EC2?
    What factors should you consider when choosing a region for your EC2 instance?
    What is the purpose of a VPC in Amazon EC2?
    What are subnets and their role in EC2?
    How do security groups protect your EC2 instances?
    What are the steps to launch an EC2 instance?
    What is the importance of tagging in EC2?
    Can you automate EC2 scaling?
    What security features does EC2 offer?
    What are the benefits of using AMIs?
--------
#### 1.2: Identify design principles of the AWS Cloud
#### Knowledge of: AWS Well-Architected Framework
#### Skills in:
- Understanding the pillars of the Well-Architected Framework (for example, operational excellence, security, reliability, performance efficiency, cost optimization, sustainability)
- Identifying differences between the pillars of the Well-Architected Framework

#### 1.3: Understand the benefits of and strategies for migration to the AWS Cloud
#### Knowledge of:
- Cloud adoption strategies
- Resources to support the cloud migration journey
#### Skills in:
- Understanding the benefits of the AWS Cloud Adoption Framework (AWS CAF) (for example, reduced business risk; improved environmental, social, and governance (ESG) performance; increased revenue; increased operational efficiency)
- Identifying appropriate migration strategies (for example, database replication, use of AWS Snowball)

#### 1.4: Understand concepts of cloud economics
#### Knowledge of:
- Aspects of cloud economics
- Cost savings of moving to the cloud
##### Skills in:
- Understanding the role of fixed costs compared with variable costs
- Understanding costs that are associated with on-premises environments
- Understanding the differences between licensing strategies (for example, Bring Your Own License [BYOL] model compared with included licenses)
- Understanding the concept of rightsizing
- Identifying benefits of automation (for example, provisioning and configuration management with AWS CloudFormation)
- Identifying managed AWS services (for example, Amazon RDS, Amazon Elastic Container Service [Amazon ECS], Amazon Elastic Kubernetes Service [Amazon EKS], Amazon DynamoDB)






Answer the following questions about the topics in AWS Educate: Getting Started with Compute Lab and type the questions and answers on GitHub under Domain 1.





