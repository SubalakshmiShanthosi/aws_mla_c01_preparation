# AWS Machine Learning Engineer - Associate Certification Preparation Track


AWS From Start to Certified - AWS MLA-C01 Exam Guide overview

This certification has new question types in addition to Multiple Choice and Multiple response
    New question types - Ordering, Matching and Case Study questions 

Case Studies - Architecting ML type questions

Domains for the examination:

```rb
Domain 1: Data Preparation for Machine Learning (28% of scored content)

Domain 2: ML Model Development (26% of scored content)

Domain 3: Deployement and Orchestration of ML Workflows (22% of scored content)

Domain 4: ML Solutioning Monitoring and Security (24% of scored content)
```

Domain 1 - 
```rb  
    * Data Engineering lifecycle
    * Process to data - to ensure high quality, no missing data, no errorous data.
    * 1.1 Ingest and Store data 

            How to ingest data
            How to store data
            AWS storage services
            How to store based on access pattern
            How to store based on formats
            How to structured cost
            How to store based on performance
            How to troubleshoot and debug storage related issues

    * 1.2 Understand AWS tools and services and how to use them for feature engineering

            Understand different techniques of encoding
            Understand coding for feature engineering
            Understand data cleaning
            Understand different services for validation and labeling for data

    * 1.3 Ensure data integrity and prepare for modeling. 

            Understand classification 
            Masking the data
            Anonymization 
            Data encryption 
            Data integrity and validating data quality
            Identifying and reducing data biases


```

Domain 2 - Model Development

```rb
    * 2.1 Choosing modelling approach 
             Types of models - classification, regression/forcasting for prediction of categories
             Managed AI Services - Pre-trained models for different usecases
             How to use model based on requirements
    
    * 2.2 Train and Refine Models

            Hyperparameter tuning
            Factors affecting model accuracy and model size - Model tuning

    * 2.3 Analyze model performance

            In context of sagemaker model - In different ML environments what kind of model performane metrics are setup for evaluating the model accuracy. 
```

Domain 3 - Deployment ML models

```rb
    * 3.1 Select Deployment Infrastructure
            
            Understand deployment services
            Single deployment or batch deployment 
            Select resources - CPU,GPU,RAM,network
            Different types of giving model endpoints - Serverless, real-time, async, batch inference
            Versioning of deployment and rollback 
            Model Optimization on edge devices and deployment options
            Performance, Cost and Latency tradeoffs
            Airflow and Sagemaker Pipelines

     * 3.2 Create Scripts
            
            Difference between on-demand and provisioned resources
            Scaling policies
            Containerization for both training and inference 
    
     * 3.3 CI/CD and automation
            
            Setting up Code Pipeline 
            GitFlow 
            Code repository and pipeline wiring


Domain 4 - ML Solution Monitoring and Troubleshooting

      * Monitor model inference 
          
           Identify model drifts
           Model evaluation metrics
           A/B testing
     
      * 4.2 Monitor and Optimize Infrastructure
         
           Being aware of reducing the operational scale - Reducing carbon footprint - Reduced cost
           Picking right size of infrastructure
           Compute budget, Savings plan for sagemaker instances

       * 4.3 Securing AWS resources
         
            IAM Role Manager
            Sagemaker security and compliance features
            Security best practices for CI/CD
            
            
```

AWS Training Live - Episode 2

# Data Preparation for ML
How is Data Preparation different from Data Pre-processing?

Data Processing / Data Preparation - Data Collection , Data Pre-processing and Feature Engineering.


Question: Amazon Kinesis Datastream to ingest,store and pre-process data at the same time? 



SQS - Poll a message from queue - Kinesis Data stream will hold the data within the stream - 

Before Kinesis was made of Kinesis Data Firehouse , Kinesis Data Analytics

Throw Data Into Kinesis Data Stream ---> Send data to converging Apache Flink Managed Service --> Firehouse Data store the data can be sent to be stored on data store say example S3

Producers - Publishing data to data stream 

Apache Flink Managed Service - Consumers (Custom build or build on top of Apache Flink like an App) - Control the processing logic for data 

Data Firehouse - it's can be used to offload data to destination data store.

More concerned about reading data (S3) Write once read many

Card clash - Data Lake Data Ingest (TODO)

Task 1.2 Data Preparation and Data Processing

Amazon Glue, EMR, what types of data processing is done for ML workloads-? 

Sagemaker Data Wrangler - What type of data transformations and analysis is done for the ML task data. 
