1. Difficulties You guys faced during the project
  - dockerfile tomcat homepage mistake

2. difference between git rebase and git merge
  - git rebase and git merge are both used to integrate changes from one branch into another, but they do it different ways:
  - Git merge combines the history of both the branches, creating a new commit node that ties that ties them together. This preserves complete history of both the branches.
  - Git rebase moves the commits of one branch to another, creating a linear history. Cleaner way of combining histories, used with remote and local repos.

3. what the different git branching methods?
  - git flow
  - github flow
  - gitlab flow
  - feature branch flow
  - trunk based development

4. What is continuous integration?
  - developers frequently merge their code changes into a shared repository
  - each integration is automatically built and tested to detect errors quickly
  - code commit >> automatic build >> automatic testing >> feedback

5. What is contnuous deployment?
  - automate the deployment of code changes directly to production
  - without any manual intervention
  - accelerates the feedback loop with users
  - reduces time to market new features and fixes
  - riskier way of doing things

6. What is continuous delivery?
  - deployment of code changes to staging or testing environment
  - manual approval is required to deploy to production
  - allow frequent and reliable releases

7. What is EC2 instance and other AWS services?
  - core service in AWS
  - provides scalable computing capacity in the cloud
  - allows you to launch virtual servers
  - customizable configurations of CPUs, Storage, Networking, and instance types
  - provides persistent EBS volume storage
  - other services like EC2 are:
  - S3: Object storage service for storing large amount of data, durable, scalable, secure
  - RDS: relational database service for MySQL, PostgreSQL, Oracle
  - AWS VPC: provides you your isolated private cloud network, control input and output data
  - AWS Lambda: Serverless computing
  - Amazon DynamoDB: NoSQL Database Service

8. Different storage services in AWS:
  - s3: (simple storage service)
    - object storage
    - can store large amount of data, can be used as backup, content storage
    - scalable, durable
    - accessible via HTTP
    - cross-region replication, versioning
   
  - EBS: (ELastic Block Storage)
    - block storage
    - provides persistent block storage, used for databses, file systems, EC2 instances
    - scalable upto 16TB
    - accessible as a mounted drive
    - can create snapshot, encrypt data, can provision IOPS for high performance

  - EFS: (ELastic File System)
    - File Storage
    - provides scalable storage, on-premise resource. for BigData and analytics, content management
    - auatomacally scales from gigabyte to petabyte without disrupting applications
    - accessible via NFS (Network File System)
    - provides lifecycle management

  - other storage services are: Amazon Glacier, Amazon FSx

9. Explain about the kubernetes architecture





1. do docker work in redhat instance?
  - Yes you can install Docker engine on Redhat 8 or Redhat 9. But by default podman is present on rdhat machines. You have to forcefully stop podman to use docker.
  - For that stop and remove all podman containers and uninstall podman, install docker and start the daemon.

2. What is ansible
  - ansible is open-source automation tool for management of systems, application deployment, orchestration of workflows
  - ansible uses simple human readble language(YAML) to describe automation jobs
  - ansible is built using python
  - provide agentless architecture: no need of software on managed nodes, uses SSH for communication
  - provides Idempotency: repeated tasks produce same results
  - provides Extensibility: Supports custom modules and plugins
  - some simple modules on ansible are: apt, yum, copy, file, service, user, group

3. What is SLO and SLI in DevOps
  - key concepts used to measure and manage the performance and reliability of services
  - Service Level Objective: specific, measurable target for the performance of a service. Ex. 99.9% uptime
  - Service Level Indicator: measurement of performance against the SLO. Ex. Actual Uptime

4. What are the alternatives of kubernetes
  - Docker Swarm: native clustering
  - Openshift: from Redhat - for enterprise use
  - AWS Fargate: serverless compute engine
  - Google cloud Run: serverless plaform
 
5. What is dockerfile
  - written in simple, declarative language
  - series of instructions that Docker will use to build an image.
  - some basic commands are: FROM, WORKDIR, COPY, RUN, ENV, EXPOSE, CMD

