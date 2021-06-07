
## Describe “The Cloud”
Is using another server/computer that is settled remotely as it's your own. 

## What is a container (as it relates to computers and servers)?
container is the entire runtime environment, it consists of an app, packages, dependencies, libraries and config files. containers make the app runs quickly and reliably from one computing environment to another.

## What is auto-scaling?
Is the process of modifying the resources that is needed to the app automatically.

## What is bandwidth?
Is the maximum data to transfer across a given path. (network bandwidth, data bandwidth).

## How do cloud providers compute service costs?
The cost is calculated based on the resources the company or individual may use in the VM in order to run their apps/services smoothly.
These recourses may be storage, processor, bandwidth and RAM.


------------------------------------------

## Server Instances: 
An instance is a single copy of the software running on a single physical or virtual server. If you run two copies of the software on the same physical or virtual server, that counts as two instances.


## Containers:
Is a complete unit of the code (the entire runtime environment). it makes the apps run more faster and reliable from one cloud to another.

## Cloud Services:
Is a service that will allow the users to use different remote computers/VM as they own it, the benefits of Cloud services:
 - Reduce costs of hardware/software.
 - Load Balance.
 - Mobility.
 - Data access/ Backup.
 - maintenance.
 - More security and speed.
 - Collaboration.

Types of Cloud Services:
SaaS --> Software as a service. (google drive, gmail)
Paas --> platform as a service. (GitHub, Heroku, AWS Elastic beanstalk, Netlify)
Iaas --> Infrastructure as a service. (AWS EC2, Azure)

 
## Cloud Architecture
it refer to the set of softwares, applications, databases, recourses that the cloud can have to leverage its capabilities. It isn't only define the component but the relationship between them.


## AWS:
Amazon Web Services, a (huge) collection of services that Amazon provide as a cloud computing, some of the AWS services are AWS EC2, Elastic Beanstalk

## EC2/Beanstalk vs Heroku:
Elastic Compute cloud is a IaaS service that allow the user to control the app, data, runtime, middleware and OS
BeanStalk is a PaaS that allow the user to control only the application and the data.
Heroku is also a Paas. 

<br><br>


## Summery 

### Content Delivery Network (CDN)

A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. 

- CDNs work through servers nearest to the website visitor respond to the request.  


#### How it works?

- CDN copies the pages of a website to a network of servers that are spread out at geographically different locations
-  caching the contents of the page.
-  When a user requests a webpage the CDN will redirect the request from the  site’s server to a server in the CDN that is closest to the user .


#### benifits:

speed up the delivery of Internet content, it helps protect your website against certain forms of cyber attacks .



<br><br>


### “serverless” computing ? 

  “serverless” doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of . 


### AWS Lambda ?

AWS Lambda is one of the most popular serverless computing services out there. It is also the most popular provider used with the Serverless Framework. 

Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.


![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-RealTimeFileProcessing.a59577de4b6471674a540b878b0b684e0249a18c.png)


### criteria ?

- Scalable APIs.
- Data processing
- Task automation 

### benifits?

1. Pay per use: you pay only for the compute your functions use, plus any network traffic generated. 

2. Fully managed infrastructure: you don’t need to think about the underlying servers—AWS takes care of this for you.

3. Automatic scaling: There is no pre-scaled pool, no scale levels to worry about, no settings to tune . You only pay for each function’s run time.

