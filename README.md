Food Delivery App
Individual Project for Gradaute Software Engineering course Enterprise Distributed Systems.

Goal
The goal is to build a distributed enterprise web application which allows the user to order their food online. There are 2 actors in the system:
Restaurant Owner - Can add new restaurant, menu items, change status of orders.
Customers - Can search for different restaurants, dishes, place their order and view order status.
We were tasked with this project requirement so that we can learn to build enterprise MERN stack applications using various distributed technologies such as Apache Kafka as message queues, Redis for caching, etc.
System Design
Technology stack



Area	Technology
Front-End	React, React Router, Bootstrap, HTML5, CSS3, Javascript ( ES6 )
Message Queue (Middleware)	Apache Kafka
Authentication Middleware	Passport.js
Back-End	Express, Node.js
In-Memory Caching / Datastore	Redis
API Testing	Mocha, Chai, Postman
Performance Testing	JMeter
Database	MySQL (Amazon RDS), MongoDB (Mongo Atlas on AWS)
Deployment	Amazon Web Services

Database Design trade-offs
Used MongoDB (NoSQL) to store large amounts of read heavy data which doesn't require transaction support such as Restaurant details, their menu items, etc.

Used MySQL to store data which requires transaction support such as user profile information, order details, etc.

Used database pl stored procedure for our booking and payment functionality so that we can provide transaction support and if anything goes wrong in between then we can roll back to a point where the database is in a consistent state.
---

## 📞 Support
For any issues, feel free to open an issue on GitHub or contact me. 😊  

