# hack-careem

Project Name: -> Make Commerce Happen

Project Description: ->

Careem's vision is to become the biggest mover of people and goods across MENA. 
In this sphere, a major challenge is around the logistics of delivering shipments to customers. 
Build a platform that can work with commerce companies who need a shipment delivery service. 
The platform should be a B2B one where commerce companies will request quotations for their shipments 
and the platform will look into its transportation resources to find the most cost-effective and reliable 
way to deliver shipments. The platform will be provided some inputs on different hubs and transportation 
resources from that for the last mile delivery. For inter-city shipment delivery, the platform can work with 
partners to deliver the shipments through trains, flights and trucks if required. The partner information 
will also be part of the input to the platform and is expected to change.

The scheduling capabilities the platform has built in is expected to have the following features:

Cost effectiveness in making deliveries
Reliable delivery with ETA information for customers
Working with a variety of partner services for both inter and intra-city shipments
Reliable transportation shipment modes (e.g. is a bike the best way to transport a Fridge?!)
Ability to adapt to changing partner costs, as well as adding or deleting old or new partners as 
and when they come in or leave the system
Things to Think About
What REST frameworks you will use
In-memory vs. persistent storage
Testing (unit testing/integration testing/mocking etc.)
Optimized dispatching algorithms
Service Oriented Architecture
Asynchronous processing of location updates like message queues
Horizontal scaling
Design patterns, dependency injection etc.


HLD (attached) Description: ->
1. Names are self explanatory.
2. Because of the limitation of Time and Space on draw.io webtool I abstracted the "Enterprise Messaging Service 
& Load Balanced Service Discovery (Infra & App Both) Abstraction Layer" service which provides 
the Infra & App Load balancing as a service and also provides Enterprise Messaging abstraction. 
In practice these two are separate services which again can be an abstraction to multiple different services. 
For Example, Enterprise Messaging can have underline Kafka messaging as well as MQ Based in 2 different services.
3. 


Technology To Use are: ->
1. Messaging Services: Kafka, ActiveMQ
2. Caching: ElasticSearch or Solr
3. Dashboard: Kibana for ElasticSearch and Banana for Solr
4. Persistent: MySQL or MariaDB
5. Server Language: Java8 as a main and depending on the ndividual services dynamics we can employ Scala and NodeJS too.
8. App Framework: Spring Boot or better "vert.x as it's generic and can be used along with any server language.
9. ORM: OpenJPA or Hibernate or better not use any as our DB as hibernate can be bottleneck in fast transactional environmnet.
10. Framework on Top of ORMs: Use Kundera as it can be used with any ORM and across RDBMS and NOSQL DB's.
11. Testing Tools: JUnit, Mockito, PowerMockito
12. Code Coverage: Sonar
13. Issue Tracker: Jira
14. Collaboration Tool: Confluence
15. Module Repositories: Nexus
16. Source Repo: Git
17. Source Repo Visual Tool: SourceTree and BitBucket
18. Service Discovery Tools: Consul with LinkerD (which allows integration with any Cloud/NonCloud Service Orchestrator)
19. Webservice Approach: RESTful Services
20. App Service Approach & Tools: Microservices using Docker container and Kubernetes Service Orchestrator
21. Cloud Services: AWS or Azure. 
We can use multiple services offered by them like S3 (for storing images and other heavy data), 
function i.e. serverless architecure support (best for User Authorization and Authentication Services to incure less cost, if rarely called)
22. UI: Google Material, React/Angular2, ReactNative and many Development Tools like Gulp for Build, Webpack, etc..
23. Development Tools: Eclipse for Server, Atom/Bracket/Webstorm/Sublime, Idea for both
24. Analytics: ApacheSpark
25. NoSQL DB: Cassandra
