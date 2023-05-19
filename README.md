# AWS python pipline design

## Introduction

This project generates weekly data job to use python move and process raw data in Xetra S3 Bucket to Target S3 Bucket.

## Overview
- Set up a virtual environment and AWS
- Understanding the source data, quick and dirty solution using Jupyter Notebook
- Functional approach with the quick and dirty solution
- OOP Design principles and further requirements - Configuration, Logging, Meta Data
- OOP Code Design
- Impliment class frame and Logging
- Coding (Clean Code, fucntionality, linting, unit tests, integration tests)
- Performance tuning with profiling and timing
- Create Dockerfile + push docker image to Docker Hub
- Run application in production using a Minikube and Argo Workflows


 ### Set up a virtual environment
 use pipenv to create and active a virtual environment of python 3.9
 
 ### quick and dirty source data
 use Jupyter Notebook to read multipule files, transformations and save to s3 Bucket in AWS.
 
 ### Functional approach
 create function in Adapter layer, Application Layer and create main function entrypoint.
 
 ### OOP Code Design and Impliment
 add logging(using pyyaml) and Meta data
 create s3BucketConnector(), MetaProcess(), XetraETL(), XetraSourceConfig(NamedTuple), XetraTargetConfig(NamedTuple), S3FileTypes(), MetaProcessFormat() to edit methods.

 ### Coding
 add Linters (pylint) to clean code and use unit tests(moto package) and integration tests to test each unit and framework.
 
 ### Performance tuning with profiling and timing
 using memory_profiler to improve performance 
