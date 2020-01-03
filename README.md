# AWS Certified Database - Specialty Exam Preparation Guide and Study Tips
In late November of 2019, AWS [announced](https://aws.amazon.com/blogs/database/new-aws-certification-purpose-built-to-validate-database-expertise/) a new specialty certification focusing specifically on database technologies.  The AWS Certified Database - Specialty Exam beta period started in early December of 2019 with the standard certification exam target date being April of 2020.  At the start of December, I participated in the beta writing one of the beta exams.  As of this writing, I do not know my results and whether on not I achieved the certification.  Nevertheless, I thought it would be useful to share my experience.  I'll try to list the topics covered by the exam questions, and provide insight and useful resources that are helpful in preparing for the exam.

## Exam Description
The database certification exam covers five domains:
- Domain 1: Workload-Specific Database Design (26%)
- Domain 2: Deployment and Migration (20%)
- Domain 3: Management and Operations (18%)
- Domain 4: Monitoring and Troubleshooting (18%)
- Domain 5: Database Security (18%)
  
The exam's goal is to test user's competence to:
- Understand the various AWS database services
- Recommend and design database solutions appropriate to satisfy specific requirements

AWS suggests that the examinee has:
- Minimum of 5 years of experience working with relational and NoSQL databases, including on-prem and cloud based implementations
- Minimum of 2 years of hand-on experience with AWS
  
## Exam Topics
- **Amazon RDS** is one of the core services offered by AWS, so having good understanding and thorough knowledge of this service is critical to succeeding in the exam.
  - You should have expertise in analyzing and identifying requirements / use cases when a relational database (and specifically RDS) is the appropriate solution.  You should also have a good understanding of the service capabilities and limitations.
  - Multi-AZ: Know technical details of its implementation and when it is appropriate (e.g. disaster recovery scenarios)
  - Read-Replicas: Know technical details and in what situations is it useful (e.g. off-loading read traffic)
  - Know the numerous engine options RDS has available
    - There are engine specific questions, so you should have some familiarity with each engine (e.g. Oracle TDE, PostgreSQL specific capabilities)
  - Backups
  - Option Groups
  - DB Parameter Goups
  - SQL Performance Insights (what is it, when is it applicable, and how is it different from CloudWatch)
- Alongside RDS, **DynamoDB** is probably the most crucial of AWS databse services.  You should know it inside and out.
  - Understand Primary Keys/Partition Keys/Sort Keys.  Be able to design/choose them in a particular scenario and use them.
  - Global Secondary Indexes / Local Secondary Indexes.  Understand difference between them and applicable use cases.
  - DynamoDB Streams
  - Global Tables (and its use cases)
  - Data Modeling
    - Partition Sharding (e.g. adding random suffix)
    - Composite Keys
  - Best Practices
  - Querying and Filtering
  - DAX
  - Have a good understanding of the underlying technical architecture
- **Amazon Aurora**
  - Understand the technical architecture and use cases
  - Difference between Aurora Read Replicas/RDS Read Replicas
- **CloudWatch**
  - Understand the service functionality 
  - How to use in troubleshooting scenarios
  - Performance monitoring and notification/alerting scenarios
- **Database Migration**
  - There are questions around AWS SCT (Schema Conversion Tool) and AWS DMS (Database Migration Service).  You should have a general understanding of both, difference between them, and when you would use one vs the other.
- **ElastiCache**
  - Have a good understanding of use cases when caching is appropriate
  - Focus on Redis
  - Understand Redis architecture, Multi-AZ, etc.
  - Understand various caching strategies (Lazy Loading, Write-Through) and benefits/limitation of each
- **DatabaseDB**
  - I don't recall many questions on this service, however you should have general familiarity with it
- **Neptune**
  - I don't recall many questions here.  However, you should have general understanding of graph database concepts and graph database applications.
- **Security**
  - Understand options and solutions for data encryption (both data at rest and data in transit)
  - Authentication options and capabilities
  - Access Management (IAM)
  - Have good understanding of services like Parameter Store and KMS
- **Networking**
  - Understand how to integrate various services with VPC (e.g VPC Endpoints)
  - Know how to secure access at network level
- **Solutions Architecture**
  - There were a number of questions very reminiscent of questions from AWS Solutions Architect Exam.  I *strongly* suggest attaining AWS Solutions Architect Associate Certification before attempting this specialty exam.
  - Understand AWS Lambda and how it can be used in conjunction with all the other services mentioned above
- **Deployment and CI/CD**
  - There were quiet a few (more than I expected) questions relating to deployment and CI/CD concepts.  I would *strongly* suggest attaining the AWS DevOps Engineer Professional certification prior to writing this specialty exam (or at least AWS Developer Associate Certification).  You need to understand the various DevOps services AWS offers (e.g. CloudFormation, CodeBuild, CodeDeploy) and how they can be utilized to assist deployment scenarios.

## General Tips
As mentioned above, I strongly suggest having both AWS Solutions Architect - Associate and AWS Certified Developer - Associate certifications (or preferably AWS DevOps Engineer - Professional) prior to entering to write this specialty exam. The experience and knowledge required to attain those certifications will go a long way in helping you do well in this exam.

## Resources
Include links here.
