# tools of devops

Devops is a collaboration between development and operations and a culture and it has tools that faciliate this need. 
A good reference is Xebia periodic tools[1]

# tools of build automation
build automation -again- are tools that are used to automate the process of building targets from their source code, here are some great examples:
- Java has ant, gradle and maven
- JS has npm, gulp, grunt
- C/C++ utilize make automation tool
- Packer - helps in building machine images and containers 
#
# continuous integration tools

There are plenty of CI servers out there and each server provides a certain advantage over the other

- Jenkins: a fork of hudson, it's open-sourced and is the most popular option
- Travis CI: open source, built around github integrations which can be great if you use github as
  control. A very good advantage travis offers is that each build is built in a new clean slate VM
  which prompts consistency among builds
- Bamboo: a server CI by atlassin which integrates well with jira and altassian tools

There are plent other CI servers out there and we should pick the right based on many factors.
#

# tools for configuration mangement 

- ansible is the great agentless automation tool out there. It requires no master server and no agent
  utilizes the already built technologies of ssh and python to do the trick. It's the mainstream infrastructure as a code system

- puppet, built in ruby and uses declartive language like ansible. Puppet, however, requires the use 
  of a CI server which it uses as agents to deploy changes
- chef, uses procedural configuration and uses its own custom Chef DSL so if you want to do a functionality 
  outside chef capabilities, You'd have to learn its own stuff
- Salt agent/master, but can support agentless, support for even driven automation which means it 
  triggers actions without human intervention on certain pre-specified events.

# tools for virtualization and containerization 

types of virtualization technologies:
- virtualization: It uses software to create virtual version of something rather than actual one.
- hypervisor: It is software used to create and run virtual machines that run on baremetal servers
- Containers:  containers don't virtualize the Operation System but rather stimulates the OS by 
  providing the bare minimum thin layer of what the application needs to run. They use resources 
  effectively, unlike the other types that virtualizes everything.


# tools of monitoring

there are two types: infrastructure monitoring and application performance Monitoring (APM) which cares about responses time and 

<h2> infrastrucutre monitoring tools </h2>
- sensu modern replacement for nagios server-agent architecture, so you must have a server and a client on 
  each server
- NewRelic: SAAS as a master, and a client on each of your infrastrucutre. It also does APM as well. The 
  master is in their cloud 

<h2> applications performance monitoring  monitoring tools </h2>
- App Dynamics: server/agent architecture, and provides diagnoistics on code-level and is able to 
  identify issues at code level
- New relic, like we mentioned before it also does APM

<h2> aggregation and analysis of the data from monitoring tools </h2>

Most monitoring tools have analysis tools. It's very important as much as making the logs themseleves,
One of the most prominent tools in aggreation and does analysis is elastic stack which does the data collection in a server/client architecture where the main host has all the information on each

# Orchestration Tools

- docker swarm: utilizes docker images and makes a great orchestration tool with minimal headache
- kubernetes: also utilizes docker and something called runc engine and it's cross-platform
- Apache ZooKeeper is an open-source server for highly reliable distributed coordination of
  cloud applications. It is a project of the Apache Software Foundation 
- terraform: some say it's an IaaC but it's a great orchestration tool that integrates well with AWS
  and it be used in a conjoint operation with ansible and kubernetes together


so often more than the others, we can use more than one orchestration tool so each one does
something different, so it really depends on our use case :) 

[1] xebialabs.com/periodic-table-of-devops-tools