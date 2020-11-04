# Tech Stack Rationale

This document will lay out an overview of the proposed tech stack for the Plant Health Data Solutions project and provide a supporting rationale for each element chosen.

Proposed tech stack: **MERN** (**M**ongoDB, **E**xpress, **R**eact, **N**ode.js)

The MERN stack leverages javascript based open-source technologies to provide a simple, flexible, and fast framework for building web applications.


# Plant Health Data Solutions Rationale

A number of criteria specific to the Plant Health Data Solutions project were considered in the decision to use the MERN stack proposed above.
*   Lots of data formats – specialists have many datasets in a wide array of formats
*   Maintenance – the project places a high value on sustainability and extensibility
*   Fast development – the project has an accelerated timeline requiring quick development
*   Flexibility – a large number of use cases, requires a flexible application structure


## Lots of data formats

**Supporting technologies: MongoDB**

Crop specialists — the primary end-users of the product — collect and utilize large amounts of data spread over many different data formats and structures. One of the identified needs is to compare data across these disparate datasets.

MongoDB allows for the necessary flexibility to allow specialists to upload data in many different formats and structures to a centralised database, thereby supporting the need for comparison across datasets. MongoDB also makes it easy to store and share multimedia data (video, audio, images) which was identified by specialists during user research as an important aspect of their work.



## Maintenance

**Supporting technologies: MongoDB, Node.js**

Project criteria included the sustainability of this project and the ability to extend product features to meet future needs. A focus was put on technologies that required fewer adjustments over time and systems that were easy to maintain.

MongoDB makes it easy to design a system with flexible data structures to address future needs. This allows a product to adapt to changing needs without requiring a database architect or software developer to constantly make updates to the allowed data types and formats.

Node.js has a large library of open source packages, developers can quickly identify and implement solutions to problems that the community has already addressed. This ability to implement existing code means that the cost of solving challenges is often drastically reduced.


## Fast Development

**Supporting technologies: MongoDB, Express, React**

This project has an accelerated timeline that covers many more concerns than a typical software development project. It is critical that the project team be able to move quickly and build momentum by delivering key development milestones in a short timeframe.

MongoDB and Express are both optimized to allow developers to quickly set up application frameworks and begin working quickly. React allows developers to easily reuse code for front-end components and therefore reduces the time it takes to add or extend features.


## Flexibility

**Supporting technologies: MongoDB, React**

The Plant Health Data Solutions project has a large number of potential use-cases due to the large number of datasets and the varied applications of this data. The primary end-users of the product – OMAFRA crop specialists – have many shared needs but also have a number of unique requirements based on the nature of their work and the needs of their clients.

MongoDB allows for flexibility in data structures to ensure that specialists' data needs are easily accommodated. React allows for a powerful and diverse front-end design that will allow for flexibility in the interfaces that specialists and other users interact with.


# Benefits of using MERN



*   Fast development, easy maintenance
*   Flexible architecture and data structures
*   Open source technologies


## Fast development, easy maintenance

One of the main benefits of the MERN stack is that developers only need to be proficient in JavaScript. Because only **one programming language** is used for both server and client-side code as well as the database shell, context switching is much easier. This means applications are developed faster and maintenance is simpler. This single programming language requirement also makes it **easier to hire developers** that can develop and maintain your application.


## Flexible architecture and data structures

The technologies leveraged in the MERN stack are **un-opinionated** and provide flexibility at every level of the application. The MongoDB database allows for a fast and flexible approach to data which can increase the lifetime of a product and decrease the need for regular maintenance. The front-end React application allows for a **flexible approach to architecture** that makes adding features and extending functionality simpler.


## Open source technologies

All of the technologies included in the MERN stack are backed by large and stable **open source communities** and receive regular security updates and performance improvements. These communities also mean that there is a wealth of **learning and support resources** available. The open source nature of the MERN stack also allows for a robust ecosystem of **pre-built solutions** for many common application features and functionalities.


# MERN stack components


## MongoDB: Database

MongoDB is a NoSQL database where each record is a document of key-value pairs. MongoDB allows for a flexible data structure and gives developers a JavaScript shell to interact with the application database.



*   Scalable – Large and non-standard data can be handled easily
*   Flexible – A schemaless database can store any type of data
*   JSON – Simple syntax, easy sharing of many data types (including multimedia)


## Express: Back-end Framework

Express is a minimalist framework for Node.js. This makes it simpler and easier to write backend JavaScript code, Express is used to build powerful web applications and APIs.



*   Asynchronous and Single-threaded
*   Efficient, fast & scalable
*   Large community of support


## React: Front-end Framework

React is a JavaScript library for building front-end UI. React is not a true framework, allowing for much more flexibility in how applications handle concerns. Used for complex UI, React can handle complex and rapidly changing data.



*   Component-based – promotes code reusability, application is easy to understand
*   High performance – highly optimized for high performance with virtual DOM, JSX, etc.
*   Mobile apps – can be used to develop Android and iOS apps as well as web applications


## Node.js: Runtime Environment

Node.js allows developers to run JavaScript code on the server. NPM (Node Package Manager) gives developers access to thousands of free packages to address common problems.



*   Open source
*   Fast
*   Highly scalable

