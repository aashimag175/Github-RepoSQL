# Step-by-Step Guide: Setting Up an AWS Database with Amazon RDS
Setting up an AWS database involves several steps,and there is a specific process on the type of database one needs to create.In this section,I'll elaborate on how to setup a relational database using Amazon RDS(Relational Database Service)

Prerequisites

Make sure you have the following:

a) An AWS account which can be signed up on https://aws.amazon.com/


Steps to be followed:

Step-1: Login to the AWS Console by signing into the AWS account and open the Amazon RDS console at https://console.aws.amazon.com/rds
Step-2: Create the RDS Database by creating the RDS instance and choosing the "Standard Create" option
Step-3: Choose the database engine you prefer using by selecting the appropriate version and configure the settings accordingly including the database instance class,storage,and database details
Step-4: Configure the "Advanced Settings" as needed by database name,port,DB instance identifier,backup,and maintenance.Once reviewed you may click the "Create Database" button.It may take a few minutes for the RDS instance to be provisioned and one can monitor the status in the RDS dashboard
Step-5: To connect to your RDS database typically,you'll need the endpoint(hostname) and port number along with username and password one has specified during the setup.

After setting up the AWS Database you can add a sample database to your AWS RDS instance assuming that you've selected MYSQL database.The following steps needs to be considered and can be followed as below:

Step-1: Connect to the AWS RDS Database by using the endpoint,port,username,and password to connect to your RDS instance using these credentials
Step-2: After logging,you may create a new database within your RDS instance using the "CREATE DATABASE (Database Name)". Once done,you can easily verify that the database was created successfully by listing the databases on the left-hand side.

That's it! You've successfully created a new database in MySQL. You can now use this database for storing tables and data as needed for your applications.