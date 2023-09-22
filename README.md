# Github-SQL-Repo
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


