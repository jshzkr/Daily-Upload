Custom bootcamp
 
NIKHIL KUMAR PATRA SH7B23237 
Day 1 (IDA 29/08/23)

Topics covered:-
1) Data - A piece of any information

2) Database - Organized collection of data usually controlled by a management system.

3) ER Model - Used to identify entities to be represented in the database

4) Normalization - Minimizing redundancy from a relation
(i) 1NF
(ii) 2NF
(iii) 3NF
(iv) 3.5NF

5) De-normalization

6) Case study of ER

7) Case study of normalization

8) Dimension modelling - 

9) Slowly changing dimension - Enable the historical aspect of data in an analytical system
(i) SCD 1
(ii) SCD 2
(iii) SCD 3


Day 2 (30/08/23)

Topics covered:-
1) Data (Structured, semi-structured, unstructured)

2) Big Data

3) Batch Processing

4) Stream Processing

5) Parallel and distributed processing

6) Data Warehouse

7) Data Lake

8) Data Lakehouse

9) Difference between Authorization and Authentication

10) Cloud Computing (Private, Public, Hybrid) and its benefits

11) CapEx and OpEx

12) Serverless computing

13) Azure Fundamentals (Azure Subscription, ARM, Resource Groups)

Day 3 (31/08/23)

Topics covered
1) Single Database, elastic pool

2) DDL (Create table, create schema, alter, drop)

3) DML (Update, insert, delete)

4) DCL (Grant/Revoke)

5) Schema

6) Examples and practices for DDL, DML and DCL commands

Day 4 (01/09/23)

1) Joins (Inner, Left, Right, Self, Outer, Cross)

2) Union

3) Stored procedures

4) Functions

5) Scalar and table view

6) Indexing (Cluster, Non-Clustering, Columnar) 

Day 5 (04/09/23)

1) Azure Storage

2) Data Lake

3) Data Warehouse

4) Data Lakehouse

5) Blob Storage

6) Data lake gen 2 storage

7) Storage account

Day 6 (05/09/23)

1) Data Lake

2) Azure blob storage

3) Azure Data Lake

4)File Share

5) Containers

6) Uploading the file to the blob service

Day 7 (06/09/23)

Azure Data Factory
Access
Authentication
Creation of container in Data Lake
Uploading a file into ADLS Gen2

Day 8 (07/09/23)

Azure Data Factory
Source Transformation
Sink Transformation
API Integration
CDC

Day 9 (08/09/23)

Real-time data synchronization
Azure error handling
Azure monitoring

Day 10 (12/09/23)

Azure Synapse Analytics
Creation of Azure Synapse Account
Synapse Studio
Pipeline
SQL Pool

Day 11 (13/09/23)

Intro to Power BI
Data loading
Different types of data transformations – Removing duplicates, merge queries, slicers
Parameters
DAX, Calculated columns, measures
Simple analysis charts

Day 12 (14/09/23)

Connection with Azure SQL
Univariate and Bivariate analysis
Exploring various analysis charts
Reports and dashboard

Day 13 (15/09/23)

Intro to Python
Different data types and their syntaxes with examples
Different operators in python

Day 14 (19/09/23)

args and kwargs
Classes
Lists
Lambda function

Day 15 (20/09/23)

PANDAS,NumPy
Tuples, Dictionaries
User-defined functions
If-Else statements
Zip functions, Enumerate, Counter

Day 16 (21/09/23)

Big Data
Introduction to Spark
Architecture of Spark
Pyspark
Spark Session
Read File Using Spark
RDD

Day 17 (22/09/23)

RDD to dataframe
Data Transformation
SQL Query in PySpark
Parquet

Day 18 (25/09/23)

Data cleaning
Filtering data
Drop

Day 19 (26/09/23)

Azure Data Bricks
Mounting and why mounting
Parameterization
Widgets
Utility table
Streaming data

Day 20 (27/09/23)

Cluster
Caching
Persist and Unpersist
Data Cleaning
Azure Data Bricks Connection with other Services
Delta Table
Scheduling
Connection to Azure SQL DB through JDBC Connection

Day 21 ( 28/09/23)

Docker
Steps to containerize a flask app

app.py
Add requirements.txt file which contains all the libraries . 
Add dockerfile without any extension and add instructions in it . 
Create an image using the command docker build -t app-name  . 
To check it use the command docker images .

Steps to push to Azure Container Registry

Install Azure CLI using command  curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash .
Login in Azure using the command az login -u userName -p password .
Create a Resource Group in Azure using the command az group create --name RG_Shell_IDA --location eastus .
Create an Azure Container Registry using the command az acr create --name cridashell --resource-group RG_Shell_IDA --sku Standard --admin-enabled true .
Login in the Azure Container Registry using the command az acr login --name acrName .
Then enter the username and password (from Azure Container Registry) .
name the container using the command docker tag cridashell/flask-app:latest cridashell.azurecr.io/flask-app:latest .
push the image into ACR using the command docker push cridashell.azurecr.io/flask-app:latest .

Kubernetes

Steps to deploy image using Kubernetes

Create a folder name kubernetes and add two files service.yaml and deployment.yaml .
Add necessary code in both the file .
Run the command kubectl apply -f deployment.yaml and kubectl apply -f service.yaml . 
Run the command az aks get-credentials --resource-group RG_Shell_IDA --name K8S_Cluster .
Run the command az aks update -n K8S_Cluster -g RG_Shell_IDA --attach-acr cridashell . 
Attach the container port to localhost port using command kubectl port-forward flask-app-deployment-658d6f6d66-djvm5 8000:8000 .

Day 22 (29/09/23)

Intro to Azure DevOps
Azure Board
Epic, Feature, User Story, Tasks
Creating a simple project with proper naming
Creating Repos
Creating Pipelines
CI/CD

Day 23 (03/10/23)

Machine Learning
Azure ML Service
ML Workspace
Pipeline
Dataset
Filter Data

Day 24 (04/10/23)

Azure ML Service
Pipeline
Split Data
Train Model
ML Algorithm
Score
Evaluate Model
