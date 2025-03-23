# Day 3: 30 Day DevOps Challenge

## Project: Creating a Data Lake on AWS for NBA Sports Analytics

This project is an exercise from the 30 Day DevOps Challenge. It demonstrates the creation of a data lake on AWS while showcasing how to programmatically set up and tear down AWS resources using Python and the AWS SDK (boto3).

## Project Overview

The project consists of two main Python scripts:

1. `data_lake_setup.py`: Creates and configures AWS resources for the data lake
2. `delete_aws_resources.py`: Cleans up and removes all created AWS resources

## Features

### Data Lake Setup (`data_lake_setup.py`)

- Creates an S3 bucket for storing NBA data
- Sets up an AWS Glue database and table for data cataloging
- Fetches NBA player data from sportsdata.io API
- Converts and uploads data to S3 in line-delimited JSON format
- Configures Athena for querying the data

### Resource Cleanup (`delete_aws_resources.py`)

- Deletes all objects in the S3 bucket
- Removes the S3 bucket itself
- Deletes the Glue database and associated tables
- Cleans up Athena query results

## AWS Services Used

- Amazon S3: For data storage
- AWS Glue: For data cataloging and schema management
- Amazon Athena: For querying the data
- AWS SDK (boto3): For AWS service interaction

## Cleanup

The project includes a cleanup script to remove all created resources, helping to manage AWS costs and maintain a clean environment.
