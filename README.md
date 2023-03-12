# Fundamentals of Software Architecture - M. Richards, N. Ford
Questions

## Chapter 1: Introduction
#### 1. What are the four dimensions that define software architecture? 
Architecture characteristics, Design Principles, Structure, Architecture Decisions
#### 2. What is the difference between an architecture decision and a design principle?
A design principle differs from an architecture decision in that a design prinicple is a guideline rather than a hard and fast rule
#### 3. List the eight core expectations of a software architect 
Make architecture decisions, continually analyse the architecture, keep current with latest trends, ensure compliance and experience, have business domain knowledge, possess interpersonal skills, understand and navigate politics
#### 4. What is the First Law of Software Architecture? 
Everything in software architecture is a trade-off

## Chapter 2: Architectural Thinking
#### 1. Describe the traditional approach of architecture versus development and explain why that approach no longer works 
The traditional view of architecture separates between the architect who is in charge of 
#### 2. List the three levels of knowledge in the knowledge triangle and provide an example of each.
#### 3. Why is it more important for an architect to focus on technical breadth rather than technical breadth?
#### 4. What are some of the ways of maintaining your technical depth and remaining hands-on as an architect?
## Chapter 3: Modularity
#### 1. What is meant by the term connascence?
#### 2. What is the difference between static and dynamic connascence connascence?
#### 3. What does connascence of type mean? Is it static or dynamic connascence?
#### 4. What is the weakest form of connascence?
#### 5. Which is preferred within a code base -- static or dynamic connascence?

## Chapter 4: Architecture Characteristics Defined
#### 1. What three criteria must an attribute meet to be considered an architecture characteristic?
#### 2. What is the difference between an implicit characteristic and an explicit one? (Provide an example of each)
#### 3. Provide an example of an operational characteristic
#### 4. Provide an example of a structural characteristic
#### 5. Provide an example of a cross-cutting characteristic
#### 6. Which architecture characteristic is more important to strive for -- availability or performance?
## Chapter 5: Identifying Architecture Characteristics
#### 1. Give a reason why it is a good practice to limit the number of characteristics ("-ilities") an architecture should support
#### 2. True or False: most architecture characteristics come from business requirements and user stories.
#### 3. If a business stakeholder states that time-to-market (i.e., getting new features and bug fixes pushed out to users as fast as possible) is the most important business concern, which architecture characteristics would the architecture need to support?
#### 4. What is the difference between scalability and elasticity?
#### 5. You find out that your company is about to undergo several major acquisitions to significantly increase its customer base. Which architectural characteristics should you be worried about?
## Chapter 6: Measuring and Governing Architecture Characteristics
#### 1. Why is cyclomatic complexity such an important metric to analyze for architecture?
#### 2. What is an architecture fitness function? How can they be used to analyze an architecture?
#### 3. Provide an example of an architecture fitness function to measure the scalability of an architecture.
#### 4. What is the most important criteria for an architecture characteristic to allow architects and developers to create fitness functions?
## Chapter 7: Scope of Architecture Characteristics
#### 1. What is an architectural quantum, and why is it important to architecture?
#### 2. Assume a system consisting of a single user interface with four independently deployed services, each containing its own separate database. Would this system have a single quantum or four quanta? Why?
#### 3. Assume a system with an administration portion managing static reference data (such as the product catalog, and warehouse information) and a customer-facing portion managing the placement of orders. How many quanta should this system be and why? If you envision multiple quanta, could the admin quantum and customer-facing quantum share a database? If so, in which quantum would the database need to reside?
## Chapter 8: Component-Based Thinking
#### 1. We define the term component as a building block of an application—something the application does. A component usually consist of a group of classes or source files. How are components typically manifested within an application or service?
#### 2. What is the difference between technical partitioning and domain partitioning? Provide an example of each.
#### 3. What is the advantage of domain partitioning?
#### 4. Under what circumstances would technical partitioning be a better choice over domain partitioning?
#### 5. What is the entity trap? Why is it not a good approach for component identification?
#### 6. When might you choose the workflow approach over the Actor/Actions approach when identifying core components?
## Chapter 9: Architecture Styles
#### 1. List the eight fallacies of distributed computing.
#### 2. Name three challenges that distributed architectures have that monolithic architectures don’t.
#### 3. What is stamp coupling?
#### 4. What are some ways of addressing stamp coupling?
## Chapter 10: Layered Architecture Style
#### 1. What is the difference between an open layer and a closed layer?
#### 2. Describe the layers of isolation concept and what the benefits are of this concept.
#### 3. What is the architecture sinkhole anti-pattern?
#### 4. What are some of the main architecture characteristics that would drive you to use a layered architecture?
#### 5. Why isn’t testability well supported in the layered architecture style?
#### 6. Why isn’t agility well supported in the layered architecture style?
## Chapter 11: Pipeline Architecture
#### 1. Can pipes be bidirectional in a pipeline architecture?
#### 2. Name the four types of filters and their purpose.
#### 3. Can a filter send data out through multiple pipes?
#### 4. Is the pipeline architecture style technically partitioned or domain partitioned?
#### 5. In what way does the pipeline architecture support modularity?
#### 6. Provide two examples of the pipeline architecture style.
## Chapter 12: Microkernel Architecture
#### 1. What is another name for the microkernel architecture style?
#### 2. Under what situations is it OK for plug-in components to be dependent on other plug-in components?
#### 3. What are some of the tools and frameworks that can be used to manage plug-ins?
#### 4. What would you do if you had a third-party plug-in that didn’t conform to the standard plugin contract in the core system?
#### 5. Provide two examples of the microkernel architecture style.
#### 6. Is the microkernel architecture style technically partitioned or domain partitioned?
#### 7. Why is the microkernel architecture always a single architecture quantum?
#### 8. What is domain/architecture isomorphism?
## Chapter 13: Service-Based Architecture
#### 1. How many services are there in a typical service-based architecture?
#### 2. Do you have to break apart a database in service-based architecture?
#### 3. Under what circumstances might you want to break apart a database?
#### 4. What technique can you use to manage database changes within a service-based architecture?
#### 5. Do domain services require a container (such as Docker) to run?
#### 6. Which architecture characteristics are well supported by the service-based architecture style?
#### 7. Why isn’t elasticity well supported in a service-based architecture?
#### 8. How can you increase the number of architecture quanta in a service-based architecture?
## Chapter 14: Event-Driven Architecture Style
#### 1.  What are the primary differences between the broker and mediator topologies?
#### 2.  For better workflow control, would you use the mediator or broker topology?
#### 3.  Does the broker topology usually leverage a publish-and-subscribe model with topics or a point-to-point model with queues?
#### 4.  Name two primary advantage of asynchronous communications.
#### 5.  Give an example of a typical request within the request-based model.
#### 6.  Give an example of a typical request in an event-based model.
#### 7.  What is the difference between an initiating event and a processing event in event-driven architecture?
#### 8.  What are some of the techniques for preventing data loss when sending and receiving messages from a queue?
#### 9.  What are three main driving architecture characteristics for using event-driven architecture?
#### 10. What are some of the architecture characteristics that are not well supported in event-driven architecture?
## Chapter 15: Space-Based Architecture
#### 1.  Where does space-based architecture get its name from?
#### 2.  What is a primary aspect of space-based architecture that differentiates it from other architecture styles?
#### 3.  Name the four components that make up the virtualized middleware within a space-based architecture.
#### 4.  What is the role of the messaging grid?
#### 5.  What is the role of a data writer in space-based architecture?
#### 6.  Under what conditions would a service need to access data through the data reader?
#### 7.  Does a small cache size increase or decrease the chances for a data collision?
#### 8.  What is the difference between a replicated cache and a distributed cache? Which one is typically used in space-based architecture?
#### 9.  List three of the most strongly supported architecture characteristics in space-based architecture.
#### 10. Why does testability rate so low for space-based architecture?
## Chapter 16: Orchestration-Driven Service-Oriented Architecture
#### 1. What was the main driving force behind service-oriented architecture?
#### 2. What are the four primary service types within a service-oriented architecture?
#### 3. List some of the factors that led to the downfall of service-oriented architecture.
#### 4. Is service-oriented architecture technically partitioned or domain partitioned?
#### 5. How is domain reuse addressed in SOA? How is operational reuse addressed?
## Chapter 17: Microservices Architecture
#### 1.  Why is the bounded context concept so critical for microservices architecture?
#### 2.  What are three ways of determining if you have the right level of granularity in a microservice?
#### 3.  What functionality might be contained within a sidecar?
#### 4.  What is the difference between orchestration and choreography? Which does microservices support? Is one communication style easier in microservices?
#### 5.  What is a saga in microservices?
#### 6.  Why are agility, testability, and deployability so well supported in microservices?
#### 7.  What are two reasons performance is usually an issue in microservices?
#### 8.  Is microservices a domain-partitioned architecture or a technically partitioned one?
#### 9.  Describe a topology where a microservices ecosystem might be only a single quantum.
#### 10. How was domain reuse addressed in microservices? How was operational reuse addressed?
## Chapter 18: Choosing the Appropriate Architecture Style
#### 1. In what way does the data architecture (structure of the logical and physical data models) influence the choice of architecture style?
#### 2. How does it influence your choice of architecture style to use?
#### 3. Delineate the steps an architect uses to determine style of architecture, data partitioning, and communication styles.
#### 4. What factor leads an architect toward a distributed architecture?
## Chapter 19: Architecture Decisions
#### 1. What is the covering your assets anti-pattern?
#### 2. What are some techniques for avoiding the email-driven architecture anti-pattern?
#### 3. What are the five factors Michael Nygard defines for identifying something as architecturally significant?
#### 4. What are the five basic sections of an architecture decision record?
#### 5. In which section of an ADR do you typically add the justification for an architecture decision?
#### 6. Assuming you don’t need a separate Alternatives section, in which section of an ADR would you list the alternatives to your proposed solution?
#### 7. What are three basic criteria in which you would mark the status of an ADR as Proposed?
## Chapter 20: Analyzing Architecture Risk
#### 1. What are the two dimensions of the risk assessment matrix?
#### 2. What are some ways to show direction of particular risk within a risk assessment? Can you think of other ways to indicate whether risk is getting better or worse?
#### 3. Why is it necessary for risk storming to be a collaborative exercise?
#### 4. Why is it necessary for the identification activity within risk storming to be an individual activity and not a collaborative one?
#### 5. What would you do if three participants identified risk as high (6) for a particular area of the architecture, but another participant identified it as only medium (3)?
#### 6. What risk rating (1-9) would you assign to unproven or unknown technologies?
## Chapter 21: Diagramming and Presenting Architecture
#### 1. What is irrational artifact attachment, and why is it significant with respect to documenting and diagramming architecture?
#### 2. What do the 4 C’s refer to in the C4 modeling technique?
#### 3. When diagramming architecture, what do dotted lines between components mean?
#### 4. What is the bullet-riddled corpse anti-pattern? How can you avoid this anti-pattern when creating presentations?
#### 5. What are the two primary information channels a presenter has when giving a presentation?
## Chapter 22: Making Teams Effective
#### 1. What are three types of architecture personalities? What type of boundary does each personality create?
#### 2. What are the five factors that go into determining the level of control you should exhibit on the team?
#### 3. What are three warning signs you can look at to determine if your team is getting too big?
#### 4. List three basic checklists that would be good for a development team.
## Chapter 23: Negotiation and Leadership Skills
#### 1. Why is negotiation so important as an architect?
#### 2. Name some negotiation techniques when a business stakeholder insists on five nines of availability, but only three nines are really needed.
#### 3. What can you derive from a business stakeholder telling you “I needed it yesterday”?
#### 4. Why is it important to save a discussion about time and cost for last in a negotiation?
#### 5. What is the divide-and-conquer rule? How can it be applied when negotiating architecture characteristics with a business stakeholder? Provide an example.
#### 6. List the 4 C’s of architecture.
#### 7. Explain why it is important for an architect to be both pragmatic and visionary.
#### 8. What are some techniques for managing and reducing the number of meetings you are invited to?
## Chapter 24: Developing a Career Path
#### 1. What is the 20-minute rule, and when is it best to apply it?
#### 2. What are the four rings in the ThoughtWorks technology radar, and what do they mean? How can they be applied to your radar?
#### 3. Describe the difference between depth and breadth of knowledge as it applies to software architects. Which should architects aspire to maximise?







