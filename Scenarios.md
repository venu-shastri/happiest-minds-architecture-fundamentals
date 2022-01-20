# Scenario - 1

Take, for instance, a classic web service. Internal network security was not a major concern for the organization when it was established, so the application only serves queries over unencrypted HTTP rather than HTTPS. The company has required the adoption of HTTPS for all company websites as a result of recent security problems. The source code for this application was built with an old version of the company's build system, which no longer works, adding to the anguish of the team assigned to upgrade this particular web service.. Containerizing this HTTP application is straightforward: the binary may be run in a container with an outdated Linux distribution running on top of a more contemporary kernel managed by the team's container orchestrator. Adding HTTPS to this application, on the other hand, is a far more difficult operation. The team is debating whether to resuscitate the old build system or port the source code of the application to the new build system. 

#### What is your team's recommendation?



# Scenario - 2 

For parameterizing an application, many apps require a configuration file, which can be a plain text file or something more structured like XML, JSON, or YAML. Many previously designed applications assumed that this file existed on the filesystem and read their configuration from there. In a cloud-native environment, however, using an API to update configuration is frequently beneficial. Instead of manually signing in to each server and updating the configuration file using imperative commands, you may execute a dynamic push of configuration information via an API. The urge for such an API stems from its ease of use as well as the possibility to incorporate automation, such as rollback, to make configuration (and reconfiguration) safer and easier.

New applications can be developed with the intention that configuration will be a dynamic attribute retrieved through a cloud API, but modifying and changing an existing application might be far more difficult. 

#### What is your team's proposal for using api-based configuration in an existing app?



# Scenario -3 

One of the most difficult aspects of making an application portable across many environments (e.g., public cloud, physical datacenter, or private cloud) is service discovery and configuration. Consider a frontend that stores its data in a SqlSServer database. This MySQL service may be supplied as software-as-a-service (SaaS) in the public cloud, but it may be necessary to dynamically spin up a new virtual machine or container running SqlServer in a private cloud. The problem is that building a portable application necessitates the application knowing how to connect to the right SqlServer service.

#### What is your team's strategy for dealing with the aforementioned problem?



# Scenario -4 

Real-world application development is a mixed bag of techniques. Some portions of your application may be created from the ground up by your team, while others may be totally made up of off-the-shelf open source or proprietary software that you consume as a precompiled binary. As a result of this heterogeneity, any real-world application you deploy will have been written in a number of languages and will use a variety of logging, monitoring, and other common services patterns. When each application provides metrics using a different format and interface, it is very difficult to collect all of those metrics in a single place for visualization and alerting . 

#### What is your team's strategy for dealing with the aforementioned problem?



# Scenario - 5

You are building applications using a Microservices Architecture and need to be able to debug problems that cross the different components of that architecture. A Microservices Architecture can span dozens or even hundreds of individual application
server processes. This results in hundreds of individual log files ,Microservices are often (but not always) implemented using cloud solutions that limit the lifetimes of the individual application server processes. When you use a solution like
Cloud Foundry or docker, when an individual server container dies, any state within that container is lost. How can you effectively view and search all of the different log files that emerge from all of the different distributed runtimes that comprise your collection of microservices?

# Scenario - 6

You are writing either a Single Page Application or a Native Mobile Application. The application must be able to operate efficiently even when Internet connectivity is not available at the highest speeds. How do you reduce the total number of calls to back-end microservices (particularly Backend for Frontend’s) for repeated information?

Forces:

- You don’t want to cross the network any more than necessary, especially when network
  bandwidth is at a premium in a mobile device.
- You don’t want to make the user wait any more than is absolutely necessary