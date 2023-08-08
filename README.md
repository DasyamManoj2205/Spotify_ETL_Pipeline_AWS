# Spotify_ETL_Pipeline_AWS

## Introduction
  We have built ans ETL pipleline using AWS services from spotify API. The extracted data from API will be transformed in required format and then load in to AWS data store.

## Datasource
  We got the data of the artists,albumns and songs from the [spotify API] - [developer.spotify.com](https://developer.spotify.com/)

## AWS Services

### 1.Cloud Watch - 
  Amazon CloudWatch is a monitoring and management service that provides data and actionable insights for AWS, on-premises, hybrid, and other cloud applications and       infrastructure resources.
### 2.S3 -
  Amazon Simple Storage Service (Amazon S3) is an object storage service offering industry-leading scalability, data availability, security, and performance.
### 3.AWS Lambda - 
  AWS Lambda is a serverless compute service that runs your code in response to events and automatically manages the underlying compute resources for you.
### 4.Glue Crawler - 
  AWS Glue crawlers are scheduled or on-demand jobs that can query any given data store to extract scheme information and store the metadata in the AWS Glue Data Catalog
### 5.Data Catalog -
  The AWS Glue Data Catalog is a centralized metadata repository for all your data assets across various data sources.
### 6.AWS Athena - 
  Athena helps you analyze unstructured, semi-structured, and structured data stored in Amazon S3. 

## Flow

Lambda Trigger ( every 1 hour ) -> Trigger Extract function -> Store raw data in S3  -> Trigger Transform Function -> Transform data and load it in S3 -> Query from Athena


  

  
