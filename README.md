# AWS-Lift-and-Shift-Java-Application-Stack-Manually

 <h1 align="fill" >
 <img src="Cloud Architecture.jpeg"/>
</h1>

# 📒 Project Title: Java Application Deployment on AWS with MySQL, RabbitMQ, and Memcached Integration

# Project Description:
This project involves the deployment of a Java application on Amazon Web Services (AWS) utilizing individual EC2 instances for various components such as MySQL database, RabbitMQ message broker, Memcached caching system, and the application itself. The setup also includes configuring an Application Load Balancer (ALB) for handling incoming requests and ensuring secure communication through HTTPS connections.

# Components:
1. Java Application: The core application logic developed in Java.
2. MySQL Database (db01): Backend database storage for the application.
3. RabbitMQ (rmq01): Message broker for handling asynchronous communication between components.
4. Memcached (mc01): Caching mechanism to optimize data retrieval and storage.
5. EC2 Instances: Each component is hosted on individual EC2 instances for scalability and isolation.
   - db01: Hosts MySQL database.
   - rmq01: Hosts RabbitMQ message broker.
   - mc01: Hosts Memcached caching system.
   - app01: Hosts the Java application.
6. Application Load Balancer (ALB): Routes incoming requests to the app01 instance.
7. Security Groups: Ensures controlled access to each EC2 instance and the ALB.
8. Private Hosted Zones: Facilitates secure communication between components and HTTPS site connections.

# Deployment Process:
1. Provision EC2 instances for db01, rmq01, mc01, and app01.
2. Install and configure MySQL, RabbitMQ, Memcached, and Java runtime environment on respective instances Using scripts in userdata section 
3. Set up security groups to restrict access to each component with ports allowed in inbound Ttraffic mentioned in application.property file under src/
4. Configure ALB to distribute incoming requests to the app01 instance. 
5. Establish private hosted zones for secure communication.
6. Deploy the Java application code to app01.



This project aims to provide a comprehensive guide for deploying a Java application on AWS infrastructure, integrating essential components for efficient operation and scalability.
