# intro into devops and its concepts

what we will explain today are these concepts
- build automation
- Continuous delivery
- Coninuous deployment
- configuration management 
- infrastructure as a code IAAC
- orchestration
- monitoring 
- microservices  archietcture (on the other end the tradational monolithic archietcture)


<h2>build automation </h2>
build automation is simply the process that is used to make the code into binaries without human intervention, and is ready to be deployed (given we did the standards of continous delivery on it). One of the most important aspects about it
is it has to be IDE so 
#
<h2>Continuous delvery </h2>
Continuous Delivery is the simple act of keeping your code deployable, and safely getting changes into
the code without breaking the production. it includes unit tests and integrations (merging code automatically)
every time somebody pushes new code. If a developer were to push a broken code into the repoistery, the CD will
quickly notify the developers and will use older releases to fallback to it, in this case, the responsibility of
the broken code falls onto developers (teehee)
#
<h2> Continuous deployment </h2>
continuous deployment is the process of having a CD/CI line that pushes the changes onto production as soon
as possible. The more frequently you do the deployments, the less frequently you'll have to risk deploying major
changes that could potentially break. Even if a build were to fail at production, the CI automatically will fallback to the previous successful build and deploys its to the customer as soon as possible
#
<h2> infrastructure as a code </h2>
infrastrucutre as a code is the coolest thing that happened ever. It's basically writing the steps you have to 
do in order to deploy something into code, that could be versioned and tracked as well[1]
#
<h2> Configuration Management </h2>
the configuration management is the act of tracking configurations across servers and applications to ensure
the process is identical and gives the same results each time.
the benefits are (and not limited to):
- Insight into your infrastructure configuration
- reduces configuration drift that elimanitates the need for who logged on and what they did on that server
and more than that can be read at [2]
#
<h2> Orchestration </h2>
Orchestration is a higher level of infrastructure as a code. infrastructure as a code deals with one system
deployment process wheres orchestration organizes and orchestrates multiple systems so they can be readily 
deployable at any time. 
#
<h2> Monitoring </h2>
Monitoring is an effiective tool to collect data of your deployed infrastructure and does real-time notifications so teams can be notified before a big outage arrives. A good example is the following:
"You work as a developer in netflix, and an outage happened midnight when no one was even in the office,
luckily the monitoring tools that monitors server response time is getting slower and slower, it pushes a 
notification to let people fix the issue before it becomes an outage. Even in the case of outage, you'd still
be able to find valuable data that was collected at that time."
#
<h2> Microservices </h2>
Microservice is dividing your infrastructure as entities that don't have to live together in one system.
Instead of having one huge executable/app that does everything, you break it into smaller parts that
communicates using standarized APIs.
Let's say you had an app which had everything together packed: UI, payments, authentication.
You could easily divide them into three components which promopts a lot of good benefits:
- we wouldn't have to be restricted to one language
- we don't care about how each component works as long as it works, all the details are hidden 
  and encompassed   into a microservice 
- promopts scalability
- separation of concerns (SoC)



[1]https://datafloq.com/read/infrastructure-code-benefits-tools/11355
[2]https://www.javelin-tech.com/3d/people/why-configuration-management/