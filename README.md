# quickstep
Ultra Agile User Stories

# RADiQL Core Principles

The founding core principles of RADiQL are to provide superlative and unparalleled developer productivity and a joyful, accessible and playful development experience that drives innovation and entrepreneurialism at unmatched rates of product and service evolution. It's only through this approach will we be capable of meeting the demand for new software products and services in the future.

# About RADiQL QuickStep

RADiQL QuickSteps are designed to be composed using Flow Based Programming (FBE) and are a key elements in designing and building RADiQL applications. QuickSteps are designed according to Clean Architecture principles, the most important of which being that each QuickStep encapsulates and implements a re-usuable and re-composable User Story. Key elements of Hexagonal Architecture have also been incorporated, namely that application logic is pure and separate from persistence mechanisms or user interace technology and that ports and adapters are a fundamental characteristic of each QuickStep component.

RADiQL QuickStep components are analagous to Borlands Visual Component Library (VCL) for Delphi in that they do the same for Flow Based Programming as the VCL did for structured programs written in ObjectPascal. Delphi pioneered Rapid Application Development (RAD) and Joint Application Development (JAD) for Client/Server enterprise software using "lowcode" and "nocode" technology, heavily supporting re-use through drag and drop visual components or module/application templates, multiple languages (ObjectPascal with assembly language optimisation within an Object Pascal source file) and support for multiple component technologies (VCL, OCX, VBX, COM, DCOM and CORBA/IIOP). The Visual Component Library contained both GUI components (text fields, buttons, menus, etc.) but also data components (SQL Tables, SQL Queries, SOAP Calls, SQL Stored Procedures, report generators, datasource components for master/slave relationships and so forth). Visual network components (HTTP, FTP, TCPIP client socket, TCPIP server socket and UDP components, for example) were also provided. Creating low-level TCP/IP or UDP applications required no coding, as did applications using FTP file transfers.

In its day, Delphi was (and still is) an outstanding tool, though a very expensive one, for developer productivity. The reason for this was that the VCL was so well designed that it was possible to build most of an application without the need to resort to coding by hand. And furthermore the compiled software that was produced (the compiler being shared with C++ products from the same company) was of enterprise quality. Delphi Entprise made it possible to build robust production-quality data-driven multi-tier pplications with the ease of Visual Basic, with less code than VB yet with the performance, maintainability and flexibility of C++. 

After a decade of cheap or free software development tooling, Delphi still retails for over $5,000 per developer seat in its more expensive version and remains one of the best kept secrets in the software development world.

Though very different to Delphi, RADiQL is inspired by Delphi's focus on developer productivity and producing high quality results virtually instantly, with the design-time environment able to work with live data from real APIs even before the compile, build and deployment steps.

RADiQL QuickSteps are concrete implementations of User Stories that can be linked together as a network of data flows to rapidly build most or all of a new application (or microservice or suite of microservices or a combination thereof) using a drag and drop visual tool. Like Delphi's VCL components, RADiQL QuickStep components allow business analysts and designers to work with live data (be it from a test or production environment) whilst building complex enterprise-class distributed applications, leaving custom coding to development teams only where necessary.

## User Stories and Use Cases

User Stories are created and implemented by development teams using a traditional Agile development methodology. At this point in time, most developers, technical managers and business analysts are fully conversant with the now very familiar concept of User Stories. In this day and age, the development of computer applications is now almost always planned, tracked and controlled using User Stories and supporting tools such as Atlassian JIRA.

User Stories are, in effect, lightweight Use Cases. The main difference between the two is that 

1. Use Cases are usually designed in detail up front with inputs, outputs and various application flows (primary success flow and alternative and error flows) expressed as a series of related steps that need to be implemented.
2. User Stories are usually expressed as a single sentence outline specification of behaviour and subsequently elaborated by creating new User Stories and sub-tasks that need to be implemented one by one.

## Where RADiQL QuickStep fits in

The RADiQL QuickStep Framework represents a revolutionary step forward in Agile development capability that we call Ultra Agile (UA). It builds upon the work of Ivar Jacobson, Alistair Cockburn, Robert C Martin, Paul Morrison and Henri Bergius.

QuickSteps are used to enable ultra-agile development using visual tools and "lowcode" or "nocode" techniques. Using RADiQL QuickSteps, a business analyst, entrepreneur or application designer assembles an application as a network of User Stories rather than classes, functions, libraries and microservices. QuickSteps can be thought of as re-usable User Story lightweight nanoservices that can easily be combined, composed and chained together into a one or more data flows.

QuickSteps can be deployed into web browsers, monolithic applications, microservices, serverless infrastructure or a combinaton thereof.

## Design principles

The design principles of the QuickStep Framework are that:

- QuickSteps encapsulate simple User Stories. There is a one to one correspondence. 
- Quickstep component inputs and outputs are defined as streamable data structures (Information Packets).
- User interface technologies are treated as plugins. React and React Native are the default user interface technologies but are by no means the only technologies that will be supported. User interface frameworks may be substituted or combined as new frameworks and technologies are introduced.
- Databases and data stores are treated as plugins. There is no direct dependence on SQL and NoSQL databases. User Stories are implemented entirely as QuickStep components or combinations therefore and there is therefore no need to use supporting features of the database other than those provided by boundary interface components implemented as QuickStep components.
- QuickSteps are reusable. QuickSteps can be reused many times within an application or across multiple applications.
- QuickSteps are searchable. QuickSteps can be be published individually or together in a GitHub respository to be searched and indexed for use in visual tools.
- QuickSteps can be strongly typed. The input and output ports of QuickSteps can be strongly typed to support automatic wiring together of QuickStep components or automated support for matching of QuickStep outputs and inputs for autocompletion of wiring within a visual tool.
- QuickSteps are composable. QuickSteps can be built from and orchestrate other QuickSteps
- QuickSteps are peers. QuickSteps can be chained together in a network to build functionality without any coding.
- QuickSteps are self-documenting. QuickSteps are manipulated in a visual editor that explains their functionality, how they're used and the particular usage of a QuickStep component in the context of the current usage scenario.
- QuickSteps are compatible with a Polyglot environment. QuickSteps can be implemented in any language and with any technology. The default supported languages are JavaScript, CoffeeScript, TypeScript, Java and Scala.
- QuickSteps are compatible with GitHub. It's easy to find existing QuickStep components as well as to store new QuickStep components in GitHub.

# Motivation for RADiQL QuickStep

In traditional old-fashioned Agile development, User Stories are implemented one by one with a collection of classes, functions, objects, schemas, APIs and a plethora of frameworks, libraries and technology decisions. The development team frames its thoughts in terms of the implementation technologies, available APIs and architecture already selected first and foremost rather than the pure functionality described by the User Stories and the flow of data that joins these User Stories together.

## The cost of User Story reimplementation

An application is treated as a set of custom User Stories the like of which have never been seen before and that need to be developed from scratch within the context of some runtime environment or process (such as a microservice). A characteristic of this approach is that there is virtually no re-use of User Stories from application to application, nor from microservice to microservice. 

## Suboptimal risk management with no prototyping

An important principle of Agile methodologies is development of an application through many small incremental steps and short development cycles that are often referred to as "sprints", as they're referred to when adopting Scrum. Sprints typically last for between one and three weeks though shorter sprints and longer sprints are possible. The golden rule is that there must be working software at the end of each sprint. During each sprint a number of User Stories will be identified as within scope of the sprint then converted into tasks for coding and testing.

The problem here is that Agile teams focus on "building stuff" with a production implementation of the User Stories. Little or no time is given to prototyping the functionality since this is impractical given the Agile team skill set and the mix of technologies typically used in traditional Agile development. These technologies are typicially a textual programming langage (such as C, C++, JavaScript, Scala, Java, C#, Ruby, Clojure or whatever), a runtime environment (Node, JVM, .NET, etcetera.) and a database (Oracle, Neo4J, Cassandra, MySQL, MongoDB, etcetera). Using Test Driven Development (TDD) or a similar approach, unit tests are written by hand, functionality implemented and the functionality tested in a QA environment using an automated test framework such as Selenium or similar. 

Because development cycles are short it's thought that there is no point performing prototyping. However, keeping development cycles short reduces the risk but doesn't minimize it nor eliminate it. The principle is that the financial risk is restricted to one to three weeks worth of Agile team costs. If the requirements are proved to be wrong or insufficiently demanding or have been incorrectly implemented at the end of the sprint, then User Stories are created for defects or rework.

Prototyping is about reducing exposure to risk to days, hours or minutes rather than weeks or months. The ideal solution is where prototyping produces a production quality solution with little or no need to code by hand. Manual coding, unit testing and QA testing aren't eliminated entirely, but when new functionaltiy is required and needs to be implemented this way it should be made available within a repository and reusable for any future iteration of rapid prototyping that involves similar functionality. Development, testing and documention costs are thus largely eliminated for future reuse of the User Story implementation. This time can instead be spent developing new functionality only where this is needed and/or reducing time to market and project costs.

## Too much code and excessive test impact

Test driven development is an important tool in the Agile developer's armoury. When writing code by hand, writing the test for the code first and ensuring that from the outset the test fails is a pre-requisite. When the test passes, the code is complete. Done properly, TDD should achieve almost 100% code coverage.

The real issue here is not with TDD at all. It's the fact that human beings make mistakes when writing new code. TDD keeps them honest and overall more productive than if no unit tests are written. But the underlying problem (and often the almost invisible elephant in the room) is that developers simply write too much code and new code that's written by humans always has to be tested.

A further problem is that TDD is often applied in the wrong place. The unit is assumed to be a class or a function rather than an encapsulating interface, boudary object, package or module. The problem of testing at the wrong level is that should code need to be refactored, the unit test often needs to be rewritten. This destroys the theoretical value of the test to ensure functional equivalence of the old and new implementations of the functional code. In other words, if you have to write the unit test again then you really haven't done any regression testing. The test shouldn't have changed at all. So it's important to put it in the right place.

What would be better for most of the time is if human beings were not involved in writing new code. Currently human beings are difficult to eliminate from the loop. But the key point to make here is that by driving up component reuse based upon entire User Stories (rather than low level functions and classes) we can achieve this to a much higher degree and minimise or eliminiate the impedance mismatch between the User Story requirement and the correctness of the functional implementation of this in code. 

Furthermore, by reducing our testing to inputs and outputs of the User Story implementation as pure data, we greatly simplify the testing process and make the test portable across languages and environments. This means that even if the code is reimplemented in a different language, the test implementation can stay language neutral. This means that one test implementation can be used to test implementations of code in many languages (JavaScript, Java, Scala, C#, etcetera). 

## Data Monitoring and Separation of Concerns

Introducing data monitoring often requires dedicated tooling that's relatively non-portable. For this reason, many data monitoring solutions monitor HTTP requests and responses and the interface of a microservice or API gateway. The problem is that it's difficult to inject the monitoring solution into compiled code.

The inputs and outputs of a User Story are, however, possible to define with great precision in order to define portable test cases. And if User Story implementations are self-contained and plugable, it's possible to intercept streams of data between User Story implementations and tap the data stream for monitoring purposes. It then becomes easy to integrate monitoring from various data streams since all are carrying Information Packets (IPs) that follow a particular structure and obey the same conventions. The data in the data stream is pure, in other words. It isn't encumbered by the implementation details and calling conventions of any particular language. 

## Slow time to market

With re-implementation of common User Stories comes slower time to market and less complete Minimum Viable Products (MVPs). User Stories are typically implemented and re-implemented from scratch, burning time during both development and testing. Existing User Story implementations cannot easily be refactored. Where a User Story has been implemented in another language or technology, this often cannot be easily integrated into a new microservice of application due to imcompatibilities in the technologies.

## Problems of User Story portability

Switching from a monolithic application to a suite of microservices (or back again) becomes very complex because the implementations of User Stories are now no longer portable. Invocation of remotely hosted functionality (via HTTP web service calls protected by invasive circuit breaker implementation code such as Hystrix) looks very different to a local method call on another class running in the same process.

This lack of portability is due to the very hard dependencies that have been built on languages, frameworks and database technologies as well as method and function signatures. It's also due to the interweaving of User Story implementations in the code. User Story implementations rapidly become interdependent and are woven together over time. In other words there is very high coupling between User Stories and, as a result, the code becomes brittle when trying to extract or refactor User Story functionality at a later date. 

## Problems of poor documenation

Agile is typically characterised by focussing on a low ceremony approach that minimises documentation during developement and where the code itself becomes the documentation. The theory goes that expert product-focussed teams will retain intimate knowledge of the code and retain an agile edge when being required to make changes. When microservice approaches are adopted, the theory goes that the smaller finer-grained microservices will be easier to understand (as well as more flexible to redeploy and upgrade). In practice though, things rarely work out quite like this and this is expecially true when measure over years.

The result is that functionality, which was originally driven by documented user stories, is now all mixed up and baked into an application or microservice. The relationship between microservices and the multiple applications that may use them is not well understood either. And virtually none of these interdependencies will be documented. And even if they are at the outset, it's unlikely that this will be true in the long term.

With regard to self-documented code, the very directory structure of an application or microservice will be dominated by directories or folders with names like "controller", "view", "model", "helpers", "services", "persistance" and so on and so forth. A glance through the directory structure, package names or module names rarely, if ever, tells the story of what the application or microservice is actually doing (and how). 

Each User Story is broken up and distributed into artificial technical constructs dictated by convention (for a particular, language, technology or framework) or by design pattern. The User Story is no longer documented effectively in the code because the story has been sliced and diced and distributed across multiple files and possibly translated into several programming languages. The User Story itself and the correctness of its implementation is therefore very difficult to follow by reading the code. The code may document itself by telling us what its doing and how. But it rarely, if ever, tells us why its doing this, why its organised in that way and what interdepencies exist with other functionality in the same process and with other functionality in remote processes.

In a world where distributed systems are becoming the norm, relying on the code alone to document the implementation of User Stories (that may span multiple processes) is completely inadequate. 

## Knowledge loss and high cost of maintenance

It's the lack of User Story portability that makes long term maintenance of applications and microservices expensive. Developers and technology managers eventually fear making changes to applications and microservices due to the high risk of introducing new defects through lack of understanding of how User Story implementations have been interwoven and due to the interdependencies that are now no-longer understood. JIRA and Git provide a degree of traceability, but the complexity of re-tracing the original development team's steps using using JIRA and Git makes separating User Story implementations effectively impossible. Furthermore the test impact is typically quite considerable.

Staff turnover due to the modern reality of flexible resourcing and the wide variety of opportunities in the areas where development centres tend to be located (such as London, New York or the San Francisco area), along with the low-ceremony, low documentation of most Agile shops means that risk of introducing changes into an application or microservice 3 or 4 years down the line becomes very a very daunting prospect.

## Wrong and inflexible granularity of deployment

In addition to User Story implementations being split up into a number of components and services that may themselves be combined with other User Stories and therefore providing limited business agility, components and services are often deployed grouped together into a runtime process from the outset of development. Typically an Agile team will be responsible for one or more microservices in a microservice architecture and will therefore implement a User Story within the context of a particular microservice. As we've already discussed, this knock on effects of this for other consumers of the microservice is that remote and local code looks very different and therefore portability of the functionality (both from the client and the server perspectives) is badly compromised.

However, this is a wider problem. Because the User Story implementions (that are distributed across multiple files in different application layers and possibly even different processes entirely in a distributed environment) collectively describe the business rules. This means that business rules cannot be easily and conveniently made available to third parties or third party products. The implications for government, for example, are that government business rules (such as tax calculations or complex data validation) need to be re-implemented by third party software vendors and organisations. Re-implementation implies a significant test impact and the necessity of some sort of government-provided test environment with which the correctness of the third party implementation can be tested. This incurs additonal cost for both parties both in terms of money and time.

This is a wasteful use of resources and represents higher costs for the taxpayer and the consumer of the third party software. Furthermore, it restricts how much the state can offload the burden of software development onto the private sector. A knock-on effect is that it restricts competition and innovation in the private sector for this market.



