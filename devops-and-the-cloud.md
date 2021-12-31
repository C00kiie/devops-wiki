# devops and the cloud
while devops is a culture of collaboration as we have mentioned in the previous chapters,
it just happens that cloud shares a load of good practices with the devops culture.
We are going to explain what kind of services cloud offers
#


# Types of architectures

- tradational stack: where you are provided with a phyiscal server and you have to take care of:
  - Networking
  - storage
  - servers
  - virtualization
  - Operation Systems
  - Middle ware
  - Runtime 
  - Data
  - applications
  
  and you have to manage each layer on your own.

- Infrastructure as a service (IaaS): you are provided with the low-level infrastructure and it's provisioned 
  for and managed for you. You'd have to manage less which saves time, in any case, IAAS provides you with:
  - Networking
  - storage
  - servers
  - virtualization
  - Operation Systems
  
  while those are provisioned automatically by the cloud, we'd still have to manage:
  
  - Middle ware
  - Runtime 
  - Data
  - applications
  examples: AWS ec2, azure VMs/Containers, Google compute engine
 
- Platform as a service (PaaS): you are provided with provisioning for every layer except for data and 
  applications only. Examples: AWS Elastic beanstalk, Heroku, Google App Engine

- Function as a service (FaaS): all layers are provisioned - even the application and data - and you'd be
  left to manage a single function that does a one purpose. Examples are AWS Lambda, Azure functions, Google Cloud computing.

- Software as a Service (SaaS): everything is managed and provisioned by the cloud, and you'd only 
  interact with the application and consume it/feed it data. A great example is Gmail and Office365 which are
  managed entirely by the cloud and you only use the applications they offer 
#
# Google Cloud platform (GCP)
- Google App Engine (PaaS): deploy your code, and don't worry about the rest of it.
  it also has built in support for microservices and has an out-of-the box autoscaling. Certain
  Configurations are considered serverless

- Google Compute Engine (IaaS): deploy and orchestrate VMs and containers. It's integratable with ansible and 
  chef, puppet and salt. Much more like the EC2 of AWS

- Google Cloud Function (FaaS): deploy a function and don't worry about anything else!
- Gcp also offers a monitoring tools called stackdriver which provides monitoring, logging and diagnostics
  for your applications on GCP. Stackdriver can also be used to monitor AWS infrastructure.

- Cloud Deployment Manager: much more like ansible but interacts with GCP mainly which provides IaaC
- Google Cloud Kubernetes Engine: a high-level orchestration tool and allows us to do continous integration
  with the help of jenkins 

#
# Microsfot Azure
- Visual Studio Team Services offers remote Git repositories as well as continuous integration.
- Azure also supports Jenkins which can be used to do continuous integration for Java applications.
- Continuous Deployment Triggers. These triggers can be used to kick off automated deployments
  in a way that is integrated with your continuous integration process.
- Azure also has many tools to help you do Orchestration. One of these is the Azure Container Registry. 
  This is a repository of container images that can then be orchestrated using other orchestration tools.
- One such tool is the Azure Container Service, which is a Kubernetes implementation
  that provides orchestration within the Azure platform.
- Azure Web Apps,which provide cloud hosting for web applications
  in a way that is integrated with the Azure DevOps Pipeline.

- Azure Application Insights: It provides application performance monitoring,
  diagnostics and analytics. It also supports machine learning, which is a very powerful monitoring tool.
  What machine learning does is it analyzes your monitoring data,
  your application logs, performance metrics. All of this data is analyzed
  using machine learning algorithms. These algorithms are able to detect anomalies
  in the performance of your application  and notify you about problems
  before customers even notice them. Machine learning algorithms are great at detecting problems
  Machine learning algorithms are great at detecting problems

- Azure has a FaaS or Serverless solution
  called Azure Functions. These functions provide autoscaled serverless functions
  within the Azure platform.

These are just a few of the features that Azure offers to support DevOps.
If you're using Microsoft Azure, make sure that you take advantage of them.

#
# Amazon Web Services

- EC2 which (IaaS): it's very scalable and has a wide variety of cost effective ranges of hardare.
  and integrates well with the rest of AWS features
- AWS Elastic Beanstalk (PaaS): provides out-of-the box load balancing and autoscalling and can still give you
  access to the resources and customize the stack

- AWS CodeBuild: continuous integration on the cloud
- AWS CodeDeply: Continuous deployment
- AWS CodePipeline: full code pipeline from build to deploy
- AWS CodeStar: integrates all of the above code tools and integrates with management tools and jira issue
  tracker
- CloudFormation: stack templating engine, which acts as ansible for AWS and spins the whole infrastructure 
  with YAML 
- AWS Lambda (Serverless FaaS)
- Amazon Cloudwatch: track metrics and logs, set alarms, and automate responses to the monitoring data

There are many other features that AWS offer but this article falls short on it and it wouldn't sane to give a definition of each service that AWS offers.

