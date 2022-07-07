WEEK 1:
data centers: server farms
virtualization: lets you divide hardware resources on a single physical server into smaller units, called virtual machines
contact centers: call centers,
amazon connect: omni channel cloud contact center that helps companies provide superior customer service at lower cost,
three deployment models for cloud computing: public cloud, private cloud, and hybrid cloud.
Amazon EC2, Amazon Elastic Compute Cloud: a service that lets you run virtual servers in the cloud, provides secure, resizable compute capacity in the cloud as EC2 instances
EC2 scalability: begin with only the resources you need and designing your architecture to automatically respond to changing demand by scaling in or out,
cloud computing: is the delivery of computing services over the internet by using a pay as you go pricing 
                model.  You are billed only for what you use which helps you: lower your operating costs, run your infrastructure more efficiently, scale as your business needs change.  You are basically renting computing power and storage from someone else's datacenter.  

On premises, Private Cloud: you manage everything from servers to application.  
IAAS, Infrastructure as a Service: model closest to you managing physical servers.  The cloud provider provides 
                                    servers, however you manage virtual machine, os, runtime, as well.
PAAS, Platform as a Service: The cloud provider manages servers as well as os, virtual machine, and runtime,  
                            you manage applications and data and access.
SAAS, Software as a Service: The cloud provider manages all aspects of hardware, software, and application,
                             you only manage data and access only.

Serverless computing: means that your code runs on servers without needing to provision or manage the 
                    servers.the cloud service provider automatically provisions, scales, and manages the 
                    infrastructure required to run code.  These architectures are highly scalable and event driven.  They use resources only when a specific function or trigger occurs.  
AWS LAMBDA: service for serverless computing, (allows you to run code without needing to provision or manage 
            servers ), triggers in response to events, and scales automatically,
Amazon SQS, Simple Queue Service: service that allows you to send, store, and receive messages between software 
                                components, other services, or users, without losing messages or requiring other services to be available.
Amazon Simple Notification Service, (SNS): publish/subscribe service where subscribers can be web servers, 
                                    email addresses, lambda functions, or several other options. 
containers: provide you with a standard way to package your application's code and dependencies into a single 
            object.  Also used for processes and workflows in which there are essential requirements for security, reliability, and scalability.  
Amazon Elastic Container Service, (ECS): container management system that enables you to run and scale 
                                        containerized applications in AWS, highly scalable, high performance, supports Docker containers (most popular)
Amazon EKS, Elastic Kubernates Service: fully managed service that you can use to rub Kubernetes on AWS, 
                                        Kubernates is open source, scalable
AWS Cloudformation: treat your infrastructure as code, means you can build an environment by writing lines of 
                    codes instead of using the AWS management console to individually provision resources

availability zone: single data center or a group of data centers within a region
edge location: site that amazon cloudfront uses to store cached copies of your content closer to your customers 
                for faster delivery
Amazon VPC, virtual private cloud: a networking service that allows you to establish boundaries around your AWS 
                resources, allows you to organize your resources into subnets, which are sections of a VPC that contain resources
    internet gateway: allows public traffic from the internet to access your VPC
    VPG, virtual private gateway: allows you to establish a VPN connection between your VPC and a private 
                                network, use to access private resources in a VPC
    Network Access control list, ACL: virtual firewall that checks packet permissions for subnets

Amazon Route 53: DNS web service
latency: the time between when content requested and received


WEEK 2:
block level storage volumes: behave like physical hard drives
Amazon EBS, elastic block store: service that provides block level storage volumes that you can use with EC2 
                                instances, data persists if you stop or terminate EC2 instance

object storage: each object consists of data, metadata, and key,
Amazon S3, simple storage service: service that provides object level storage.  Amazon S2 stores data as 
                                    objects in buckets, offers unlimited storage space, versioning and permission controls, you pay for what you use

How is EBS different from S3? : S3 is accessbile via the internet from API where EBS is accessed by the single 
                                instance attached to EBS and can only be used by one instance at a time 

file storage: multiple clients can access data that is stored in shared file folders, ideal for use cases in 
            which a large number of serrvices and resources need to access the same data at the same time
Amazon EFS, Elastic File System: scalable file system used with AWS Cloud services and on premise resources

Amazon RDS, Relational Database Service: services that enables you to run relational databases in the AWS cloud
Amazon DynamoDB: key value database service 
Amazon Redshift: data warehousing service that you can use for big data analytics
AWS DMS, database migration service: enables you to migrate relational databases, nonrelational, and other 
                                    types of data stores.  The source and target databases can be of the same type or different types,

shared responsibility model: customers are responsible for security in the cloud and AWS is responsible for 
                            security of the cloud

AWS IAM, Identity and Access Management: enables you to manage access to AWS services and resources securely
IAM identity: provides access to an AWS account,
IAM user: identity that you create in AWS with permission policies
IAM role: identity that you create in AWS with permission policies, however a role does not have to be uniquely 
        associated with one person, a role is inteded to be assumable by anyone who needs it
IAM policy: document that allows or denies permissions to AWS services and resources, enable you to customize 
            users' levels of access to resources
AWS Shield: service that protects applications against DDos attacks,
AWS KMS, key management service: enables you to perform encryption operations through the use of cryptographic 
                                keys
AWS WAF: web application firewall that lets you monitor network requests that come into your web apps
AWS Cloudwatch: basically a metrics repository for other aws services and resources, provides built in code 
                monitoring and logging for lambda functions

resource policy: used to tell the lambda service which events have permission to invoke the lambda function,
event source: triggers your lambda function, lots of services can be event sources,
different execution models for lambda functions: push events (synchronous and asynchronous), and polling events 
                                                (stream based and non stream based)
    push events: services delivers events directly to function,
    polling events: lambda polls for events and delivers to function,
cold start: environment is bootstrapped, then function code executes
warm start: code executes without going through bootstrap process
three core components to configuring lambda: memory, timeout, and concurrency

serverless deployment: you are designing the entire structure to very detailed specifications to deploy function: the code, dependencies, and you model your infrastrucutre in a cloudformation template and use that to deploy your desired stack without writing custom scripts, 

SAM, serverless application model: application framework that allows you to deploy your serverless stack to 
                                each AWS account, you can incorporate additional tools to create an automated CI/CD pipeline for your serverless applications that is integrated with SAM

AWS xray: traces path and timing of an invocation of lambda function to locate bottlenecks and failures
AWS cloudtrail: logs api calls made by or on behalf of a function
DLQs, dead letter queues: help you capture application errors that you cannot just discard but must respond to

CX, customer experience: the process design teams follow to optimize customer experience at all touchpoints before, during, and after conversion.  CX encompasses every single interaction a user has with a particular brand.
3 keys for exceptional customer service: embrace the new, own the relationship and build trust, and use the no 
                                        but approach


WEEK 3:
effective rate for employees: focusing on increasing productivity rather than quantity of employees to negate 
                        need for more workers and also to increase wages to increase employee retainment rate
how to improve:
    geo strategy: optimize geographic footprint by placing work in most cost efficient locations,
    optimize cx delivery: make employees feel valued by enabling hybrid workplaces to meet employee needs, 
                        implement efficient software and processes to help emloyees tasks become easier,
    leverage technology: automation reduces cost and employee effort, improves productivity while providing 
                        superior service

omni channel contact centers: various channels within single stream provide access to consolidated data, agent 
                            can easily switch between channels, and allows customers to switch from one channel to another
voice channel: traditional inbound or outbound voice communications
chat: proactive or reactive chat sessions through a web site or mobile app
tasks: allow agents to create and complete tasks in an automated process

CCP, contact control panel: customizable interface that agents use to engage with contacts across multiple 
                        channels
contact flows: features that let you define the customer experience within the contact center from start to 
            finish, you can play prompts, get input data, invoke lambda functions, and integrate lex bot, and so much more because they can integrate with CRMs and databases to dynamically adapt the experience based on customer or history 
routing profile: links a collection of queues to agents and determines the contacts that an agent receives and routing priority

Amazon Connect features a native integration with amazon Lex for NLP over text and voice
consider when creating connect instance: customers' location, agents' location, regulatory or compliance data 
                            requirements, on premise, cloud, or saas workloads that integrate to contact center

routing consists of: queues, routing profiles, contact flows

queue: waiting area that holds contacts to be answered by agents
prompts: audio files played in call flows
contact: interaction with a customer in your contact center
contact attributes: refer to key value pairs that contain data about a contact, they allow you to pass data 
                    between amazon connect and other services
quick connects: a list of destinations for common transfers, can be external 
                number, agent, or queue

WK4:
reference powerpoints
WEEK 5:
reference powerpoints

Okta: identity and access management service that provides single sign on for many different applications, can 
    be integrated with Amazon Connect


AMAZON CONNECT ESSENTIALS COURSE:

IVR, interactive voice responses: used to assist contacts navigating through the existing queues to reach an agent that is able to assist them
agent: employees or customer service representative taking calls

ease of customization is a huge benefit for amazon connect, allows for incredible customer experiences because we can customize them to fit business needs,
power derives from lambda, also other crm integrations, 

did numbers, direct dial in: generic local numbers
toll free numbers: used to ensure that there is no charge to someone placing a call

contact flows:
    you have to set the active queue before transfer to queue block,
    only certain blocks will be available to certain type of contact flow,

lex: 
    provides an incredible amount of customization through the use of attributes in lambda
    uses speech recognition and nlp to build an intricate chat bot
utterances: configured phrases that can be typed or spoken to invoke a given intent
intents: result in an action based on our user input, input can be received through text or natural language understanding
    can have several slots and each slot has a type
slots: are the actual input data from a customer required to fulfill an intent, basically like a variable
fullfillment: how the request is ocmpleted after the customer contact has provided all information required to 
            fullfill intent.  could be passed to lambda or return the information back to the client via response

CHAT:
    you can wait an extended period of time with wait block
    you cannot initiate chat conversations from the CCP
    you cannot receive calls while on chat-including from other agents
    customers and agents cannot send attachments through chat interface
    only one channel is routed at a time
    total duration of contact flow cannot exceed 25 hours
    lex has a default session timeout duration of five minutes, this timeout can be increased up to 24 hrs
    test environment used to test chat uses the basic queue and basic routing profile.  By default, routing profile allows up to 2 chats, but this can be increased

    BEFORE WE TEST CHAT WE NEED TO PRECONFIG:
    update security profiles to allow the chat test mode,
    update routing profile to permit chat channel,
    configure a disconnect flow where we can add wait action blocks if we'd like

reaching more customers with web and mobile chat on amazon connect post has a lot of useful information



