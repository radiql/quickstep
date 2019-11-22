# quickstep
An Ultra Agile framework to shorten the path from User Stories to working software

# Contents

1. [RADiQL Overview](#radiql-overview)
2. [Motivation for RADiQL QuickStep](#motivation-for-radiql-quickstep)
3. [About RADiQL QuickStep](#about-radiql-quickstep)
   * [Prior art: RAD and JAD tooling](#prior-art-rad-and-jad-tooling)
   * [Focus on productivity: User Stories as components](#focus-on-productivity-user-stories-as-components)
   * [User Stories and Use Cases](#user-stories-and-use-cases)
   * [User Stories, Use Cases and Events](#user-stories-use-cases-and-events)
   * [Event Sourcing for data](#event-sourcing-for-data)
   * [Event Sourcing and scalability](#event-sourcing-and-scalability)
   * [RADiQL QuickStep and Ultra Agile](#radiql-quickstep-and-ultra-agile)
4. [Design principles](#design-principles)
 

# RADiQL Overview

The founding core principles of RADiQL are to provide superlative and unparalleled software development productivity and a joyful, accessible and playful development experience that drives innovation and entrepreneurialism at unmatched rates of product and service evolution. It's only through this approach will we be capable of meeting the demand for new software products and services in the future.

RADiQL QuickStep permits User Stories to be created from QuickStep templates or selected from QuickStep components and linked together by events and data flows. This graph of User Stories is then directly converted into working software and deployed as a monolithic application or a set of collaborating microservices or a hybrid of the two. 


# Motivation for RADiQL QuickStep

In traditional old-fashioned Agile development, User Stories are implemented one by one with a collection of classes, functions, objects, schemas, APIs and a plethora of frameworks, libraries and technology decisions. The development team frames its thoughts in terms of the implementation technologies, available APIs and architecture already selected first and foremost rather than the pure functionality described by the User Stories and the flow of data that joins these User Stories together.

This approach has many drawbacks. Click on the links below for more details.

1. [The cost of User Story reimplementation](./docs/motivations.md#the-cost-of-user-story-reimplementation)
2. [Suboptimal risk management with no prototyping](./docs/motivations.md#suboptimal-risk-management-with-no-prototyping)
3. [Too much code and excessive test impact](./docs/motivations.md#too-much-code-and-excessive-test-impact)
4. [Data Monitoring and Separation of Concerns](./docs/motivations.md#data-monitoring-and-separation-of-concerns)
5. [Slow time to market](./docs/motivations.md#slow-time-to-market)
6. [Problems of User Story portability](./docs/motivations.md#problems-of-user-story-portability)
7. [Problems of poor documenation](./docs/motivations.md#problems-of-poor-documentation)
8. [Knowledge loss and high cost of maintenance](./docs/motivations.md#knowledge-loss-and-high-cost-of-maintenance)
9. [Wrong and inflexible granularity of deployment](./docs/motivations.md#wrong-and-inflexible-granularity-of-deployment)


# About RADiQL QuickStep

RADiQL QuickSteps are designed to be composed using the principles of Flow Based Programming (FBP) and are a key elements in designing and building RADiQL applications. QuickSteps are designed according to Clean Architecture principles, the most important of which being that each QuickStep encapsulates and implements a re-usuable and re-composable User Story. Key elements of Hexagonal Architecture have also been incorporated, namely that application logic is pure and separate from persistence mechanisms or user interace technology and that ports and adapters are a fundamental characteristic of each QuickStep component. Finally, Event Sourcing is used as a technique for passing data between QuickStep components and for persistence of data.

## Prior art: RAD and JAD tooling

RADiQL QuickStep components are analagous to Borland's Visual Component Library (VCL) for Delphi in that they do the same for Flow Based Programming as the VCL did for structured programs written in ObjectPascal. Delphi pioneered Rapid Application Development (RAD) and Joint Application Development (JAD) for Client/Server enterprise software using "lowcode" and "nocode" technology, heavily supporting re-use through drag and drop visual components or module/application templates, multiple languages (ObjectPascal with assembly language optimisation within an Object Pascal source file) and support for multiple component technologies (VCL, OCX, VBX, COM, DCOM and CORBA/IIOP). The Visual Component Library contained both GUI components (text fields, buttons, menus, etc.) but also data components (SQL Tables, SQL Queries, SOAP Calls, SQL Stored Procedures, report generators, datasource components for master/slave relationships and so forth). Visual network components (HTTP, FTP, TCPIP client socket, TCPIP server socket and UDP components, for example) were also provided. Creating low-level TCP/IP or UDP applications required no coding, as did applications using FTP file transfers.

In its day, Delphi was (and still is) an outstanding tool, though a very expensive one, for developer productivity. The reason for this was that the VCL was so well designed that it was possible to build most of an application without the need to resort to coding by hand. And furthermore the compiled software that was produced (the compiler being shared with C++ products from the same company) was of enterprise quality. Delphi Enterprise made it possible to build robust production-quality data-driven multi-tier pplications with the ease of Visual Basic, with less code than VB yet with the performance, maintainability and flexibility of C++. 

At the time of writing, even after a nearly two decades of cheap or free software development tooling, Delphi still retails for over $5,000 per developer seat in its more expensive version and remains one of the best kept secrets in the software development world. This shows that even at that price point, really good tools still have a market, albeit more limited due to the steep pricing. Users of Delphi, however, still appear to believe that there's a competitive advantage to be had from using an expensive niche product of this sort.

Please note that that we've cited Delphi and the VCL as tools that possesses many of the qualities and characteristics that we're striving for with RADiQL and and RADiQL Quickstep. There have been many innovative tools over the years (such as Microsoft VisualBasic, IBM's VisualAge and many more) but we've described Delphi here because in our view it was more successful in combining the characteristics and qualities that the RADiQL toolset is built upon. Delphi has been one of our inspirations, though not the only one. And RADiQL takes a very different and far more complete approach to componentry, application assembly, deployment and maintenance. 

## Focus on productivity: User Stories as components

Though very different to Delphi, RADiQL is inspired by Delphi's focus on developer productivity and producing high quality results virtually instantly, with the design-time environment able to work with live data from real APIs even before the compile, build and deployment steps.

RADiQL QuickSteps are concrete implementations of User Stories that can be linked together as a network of data flows to rapidly build most or all of a new application (or microservice or suite of microservices or a combination thereof) using a drag and drop visual tool. Like Delphi's VCL components, RADiQL QuickStep components allow business analysts and designers to work with live data (be it from a test or production environment) whilst building complex enterprise-class distributed applications, leaving custom coding to development teams only where necessary.

## User Stories and Use Cases

User Stories are created and implemented by development teams using a traditional Agile development methodology. At this point in time, most developers, technical managers and business analysts are fully conversant with the now very familiar concept of User Stories. In this day and age, the development of computer applications is now almost always planned, tracked and controlled using User Stories and supporting tools such as Atlassian JIRA.

User Stories are, in effect, lightweight Use Cases that serve as initial outlines of the desired behaviour. Use Cases describe the successul outcome of a story as well as the altenative means of reaching that outcome and the various failure modes that may occur. The conceptual difference between the two is that: 

1. Use Cases are usually designed in detail up front with inputs, outputs and various application flows (primary success flow and alternative and error flows) expressed as a series of related steps that need to be implemented.
2. User Stories are usually expressed as a single sentence outline specification of behaviour and subsequently elaborated by creating new User Stories and sub-tasks that need to be implemented one by one.

## User Stories, Use Cases and events

It's important to understand that each step in a User Story or Use Case is, in itself, an event. The sequence of these events produce a change in state of some sort, either in terms of what's shown on a display screen, the data stored in a database, a physical change to the world that's been either been completed or that is still ongoing on-going or some combination of these.

By describing themselves in steps, User Stories and Use Cases document how these changes of state occur through a sequence of events. Viewed in this lights, User Stories and Use Cases are descriptions of event processors. Each event can be described in natural language but can also be modelled as a data structure. User Stories and Use Cases can be thought of as being linked together by a stream of event data structures passing between them. RADiQL QuickSteps that implement User Stories:

1. accept streams of event data structures as inputs
2. process events and the associated data from these inputs 
3. optionally create or pass through event data structures to their outputs

QuickStep components can have multiple inputs and multiple outputs. QuickStep components can process multiple different types of event data structures. And this is natural because this process is exactly what Use Cases and User Stories really describe. 

## Event Sourcing for data

The principle of Event Sourcing is about persisting state as a sequence of state-changing events. Events are persisted in an event store of some sort which behaves as a database of events. The state of an entity can therefore be reconstructed from the events that describe interactions with that entity. While this may sound strange at first (and somewhat risky compared with using ACID transactions using a relation database such as Oracle) you should note that this is exactly how data replication and commit logs work in databases like Oracle. So in a way Event Sourcing underpins the technology that we've used for decades.

What relational databases such as Oracle do is to reconstruct state from events into tables. An in practive Event Sourcing systems do much the same sort of thing, periodically creating snapshots of state in order to improve performance. Each snapshot can be thought of as a savepoint (or bookmark of state) in the stream of events. Rather than reconstruct state from the dawn of time, therefore, it's possible just to reference the last and most recent snapshot and reconstruct state using the events that have occurred since that snapshot was taken.

The benefits of Event Sourcing are as follows:

1. Event Sourcing is a natural fit for event-driven architectures, which are in themselves extremely scalable.
2. There is no object/relational mismatch that is so common in conventional enterprise applications. We deal with snapshots of raw data and events that desribe mutations to that raw data. So we don't need to translate between relational SQL and data structures (such as objects) in languages like Java, Scala or C#. That problem simply goes away.
3. Event Sourcing inherently creates an audit log of mutations in the form of events that are persisted in the event store.
4. It's possible to "time travel" backwards and forwards in the event stream to reconstruct state at an earlier point in time.
5. Applications built with Event Sourcing can be assembled from components that are loosely-coupled (being coupled only by the pure data that logically connects them) rather than any particular API or transport mechanism. This means that it's much easier to build applications based upon microservices and serverless platforms, bringing cost-benefits and flexible scalability.
6. Event sourcing is a natural fit for concurrent and parallel processing using multi-core CPU architectures.

## Event Sourcing and scalability

Event data structures are very easy to pass between loosely coupled components running on separate threads within a modern multi-core computer. This means that Event Sourcing is a natural fit for parallel processing on massively multi-core CPU machines.

Since the physical limits have just about been reached for improving the speed of an individual CPU core, the only viable alternative to improve utilitisation and performance of computers is to massively expand the number of CPU cores themselves and improve upon the hardware built into the CPU itself that is used to inteconnect them. Because of this, CPUs are now being produced with many more than the 2 or 4 cores that have been available to date. 

Intel's Core i9 CPUs with 18 cores (and 36 threads) are already available at the time of writing. AMD has announced CPUs with 32 cores and 64 threads in its Threadripper 2 CPU line. It's not difficult to foresee 64, 128, 256, 512 or 1024 core CPUs being produced over the next decade, with coresponding increases in the number of threads available for concurrent and parallel processing. 

Exploiting all of this power with conventional programming techniques will be difficult and expensive, however. Conventional programming languages (and the software developers that work with these) are not cut out for productive development of massively parallel processing. Indeed using these legacy programming languages its difficult to visualise how such computer programs would work. And if its difficult to visualise then it's going to be expensive to maintain, because people will struggle to understand what's going on. 


## RADiQL QuickStep and Ultra Agile

The RADiQL QuickStep Framework represents a revolutionary step forward in Agile development capability that we call Ultra Agile (UA). It builds upon the work of Ivar Jacobson, Alistair Cockburn, Robert C Martin, Paul Morrison, Henri Bergius and Eric Evans. So although the RADiQL Quickstep Framework is marks a revolutionary step forward, as with almost all progress, it's built on the shoulders of giants, and the solid foundations, hard work and wisdom of others after many years of practical experience and discovering good practice from the failures and difficulties that have encountered.

The RADiQL combines Use Cases (Jacobson), Flow Based Programming (Morrison/Bergius), Clean Architecture (Martin), Hexagonal Architecture (Cockburn), Domain Driven Design and Event Sourcing (Eric Evans) in an intuitive, highly visual data-driven framework that takes advantage of the latest advances in cloud technology, microservice technology, serverless technology, multi-core CPUs and crypto technologies such as Blockchain and Hashgraphs. What marks RADiQL as different is its ease of us, conceptual simplicity and low bar for entry. What makes it powerful is that its completely oriented to the direction that technology, government and commerce are taking in a way that other development tools are not. RADiQL is a next generation development tool suite.

QuickSteps are used to enable ultra-agile development using visual tools and "lowcode" or "nocode" techniques. Using RADiQL QuickSteps, a business analyst, entrepreneur or application designer assembles an application as a network of User Stories rather than classes, functions, libraries and microservices. QuickSteps can be thought of as re-usable User Story lightweight nanoservices that can easily be combined, composed and chained together into a one or more data flows.

RADiQL QuickStep has been created specifically to deal with the complexity of massively parallel processing and to fully exploit the computing power of next-generation multi-core CPU architectures. And to do so using Ultra Agile RAD and JAD nocode/lowcode techniques that permit organisations to exploit the power of these new platforms to achieve successful business outcomes. The business-centric nature of QuickSteps (since these actually implement and correspond to business-oriented User Stories and Use Cases) means that it's possible to understand and perform the necessary steps for Digital Transformation of an organisation in record time. And by this we mean not just the underpinning technology but the oranisational changes that need to come about to fully exploit the symbiosis beween that technology and a more effective organisation that this technology serves. That's what Digital Transformation is all about. 

RADiQL Composer and RADiQL QuickStep technologies help organsations to explore and research the possibilities through prototyping (at minimal risk and maximum speed). But at the same time RADiQL Composer using RADiQL QuickSteps can be used to implement the technology within an organisation to enable and empower Digital Transformation.

RADiQL is an Ultra Agile toolset because it brings **D**on't **R**epeat **Y**ourself (DRY) to a new level. QuickSteps are reusuable and relevant User Story or Use Case implementation that are wired together (much like your hifi system or your TV and DVD player and amplifier or any other sort of electronic components) to build "business-centric circuits". These are analogous to electronic circuits except that instead of electronic components, there are User Stories and Use Cases. Since many User Stories are common to many organisations (User Management, Purchase Orders, Inventories, Sales, Invoices, Receipts, Sorting, Mailing, Deliveries, CRM, Shopping Carts, Tax, Calculations, Social Security, Authentication, Authorisation, Analytics, Fraud Detection, Customer Service, Geolocation, Image Processing, Monitoring, Telemetry, etc.), generic User Stories can be customised, parameterised, tailored, assembled, and packaged as QuickStep components to provide the bulk of a the business needs or a particular organisation **without** involvment of a software development team.

# Design principles

The design principles of the QuickStep Framework are that:

- QuickSteps encapsulate simple User Stories. There is a one to one correspondence. 
- Quickstep component inputs and outputs are defined as streamable data structures (Information Packets).
- Information Packets contain Events which are used for Event Sourcing.
- User interface technologies are treated as plugins. React and React Native are the default user interface technologies but are by no means the only technologies that will be supported. User interface frameworks may be substituted or combined as new frameworks and technologies are introduced.
- Databases and data stores are treated as plugins. There is no direct dependence on SQL and NoSQL databases. User Stories are implemented entirely as QuickStep components or combinations therefore and there is therefore no need to use supporting features of the database other than those provided by boundary interface components implemented as QuickStep components.
- QuickSteps are reusable. QuickSteps can be reused many times within an application or across multiple applications.
- QuickSteps are searchable. QuickSteps can be be published individually or together in a GitHub respository to be searched and indexed for use in visual tools.
- QuickSteps can be strongly typed. The input and output ports of QuickSteps can be strongly typed to support automatic wiring together of QuickStep components or automated support for matching of QuickStep outputs and inputs for autocompletion of wiring within a visual tool.
- QuickSteps are composable. QuickSteps can be built from and orchestrate other QuickSteps
- QuickSteps are peers. QuickSteps can be chained together in a network to build functionality without any coding.
- QuickSteps are self-documenting. QuickSteps are manipulated in a visual editor that explains their functionality, how they're used and the particular usage of a QuickStep component in the context of the current usage scenario.
- QuickSteps are compatible with a Polyglot environment. QuickSteps can be implemented in any language and with any technology. The default supported languages are JavaScript, CoffeeScript and TypeScript for single-threaded processes based upon the web browser and NodeJS and Go (Golang) for compiled and robust multi-threaded compute-intensive highly concurrent and parallelized processess. 
- QuickSteps are compatible with GitHub. It's easy to find existing QuickStep components as well as to store new QuickStep components in GitHub.



