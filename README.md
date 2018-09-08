# quickstep
An Ultra Agile framework to shorten the path from User Stories to working software

# Contents

1. [RADiQL Overview](#radiql-overview)
2. [About RADiQL QuickStep](#about-radiql-quickstep)
   * [Prior art: RAD and JAD tooling](#prior-art-rad-and-jad-tooling)
   * [Focus on productivity: User Stories as components](#focus-on-productivity-user-stories-as-components)
   * [User Stories and Use Cases](#user-stories-and-use-cases)
   * [RADiQL QuickStep and Ultra Agile](#radiql-quickstep-and-ultra-agile)
   * [Design principles](#design-principles)
3. [Motivation for RADiQL QuickStep](#motivation-for-radiql-quickstep)

# RADiQL Overview

The founding core principles of RADiQL are to provide superlative and unparalleled developer productivity and a joyful, accessible and playful development experience that drives innovation and entrepreneurialism at unmatched rates of product and service evolution. It's only through this approach will we be capable of meeting the demand for new software products and services in the future.

# About RADiQL QuickStep

RADiQL QuickSteps are designed to be composed using Flow Based Programming (FBE) and are a key elements in designing and building RADiQL applications. QuickSteps are designed according to Clean Architecture principles, the most important of which being that each QuickStep encapsulates and implements a re-usuable and re-composable User Story. Key elements of Hexagonal Architecture have also been incorporated, namely that application logic is pure and separate from persistence mechanisms or user interace technology and that ports and adapters are a fundamental characteristic of each QuickStep component.

## Prior art: RAD and JAD tooling

RADiQL QuickStep components are analagous to Borland's Visual Component Library (VCL) for Delphi in that they do the same for Flow Based Programming as the VCL did for structured programs written in ObjectPascal. Delphi pioneered Rapid Application Development (RAD) and Joint Application Development (JAD) for Client/Server enterprise software using "lowcode" and "nocode" technology, heavily supporting re-use through drag and drop visual components or module/application templates, multiple languages (ObjectPascal with assembly language optimisation within an Object Pascal source file) and support for multiple component technologies (VCL, OCX, VBX, COM, DCOM and CORBA/IIOP). The Visual Component Library contained both GUI components (text fields, buttons, menus, etc.) but also data components (SQL Tables, SQL Queries, SOAP Calls, SQL Stored Procedures, report generators, datasource components for master/slave relationships and so forth). Visual network components (HTTP, FTP, TCPIP client socket, TCPIP server socket and UDP components, for example) were also provided. Creating low-level TCP/IP or UDP applications required no coding, as did applications using FTP file transfers.

In its day, Delphi was (and still is) an outstanding tool, though a very expensive one, for developer productivity. The reason for this was that the VCL was so well designed that it was possible to build most of an application without the need to resort to coding by hand. And furthermore the compiled software that was produced (the compiler being shared with C++ products from the same company) was of enterprise quality. Delphi Entprise made it possible to build robust production-quality data-driven multi-tier pplications with the ease of Visual Basic, with less code than VB yet with the performance, maintainability and flexibility of C++. 

After a decade of cheap or free software development tooling, Delphi still retails for over $5,000 per developer seat in its more expensive version and remains one of the best kept secrets in the software development world.

## Focus on productivity: User Stories as components

Though very different to Delphi, RADiQL is inspired by Delphi's focus on developer productivity and producing high quality results virtually instantly, with the design-time environment able to work with live data from real APIs even before the compile, build and deployment steps.

RADiQL QuickSteps are concrete implementations of User Stories that can be linked together as a network of data flows to rapidly build most or all of a new application (or microservice or suite of microservices or a combination thereof) using a drag and drop visual tool. Like Delphi's VCL components, RADiQL QuickStep components allow business analysts and designers to work with live data (be it from a test or production environment) whilst building complex enterprise-class distributed applications, leaving custom coding to development teams only where necessary.

## User Stories and Use Cases

User Stories are created and implemented by development teams using a traditional Agile development methodology. At this point in time, most developers, technical managers and business analysts are fully conversant with the now very familiar concept of User Stories. In this day and age, the development of computer applications is now almost always planned, tracked and controlled using User Stories and supporting tools such as Atlassian JIRA.

User Stories are, in effect, lightweight Use Cases. The main difference between the two is that 

1. Use Cases are usually designed in detail up front with inputs, outputs and various application flows (primary success flow and alternative and error flows) expressed as a series of related steps that need to be implemented.
2. User Stories are usually expressed as a single sentence outline specification of behaviour and subsequently elaborated by creating new User Stories and sub-tasks that need to be implemented one by one.

## RADiQL QuickStep and Ultra Agile

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
- QuickSteps are compatible with a Polyglot environment. QuickSteps can be implemented in any language and with any technology. The default supported languages are JavaScript, CoffeeScript and TypeScript for single-threaded processes based upon the web browser and NodeJS and Go (Golang) for compiled and robust multi-threaded compute-intensive highly concurrent and parallelized processess. 
- QuickSteps are compatible with GitHub. It's easy to find existing QuickStep components as well as to store new QuickStep components in GitHub.

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


