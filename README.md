# Data-pipeline-with-Airflow
automate solution to run task on AWS

## Introduction

The music streaming company Sparkify decide to automate their data warehouse ETL pipelines. Our goal is to create our  own custom operators to perform tasks such as staging the data, filling the data warehouse, and running checks on the data as the final step.

Before choose the tool to achieve that, we considered to run cron, which is a simple and effective way to execute the jobs. However, the limitation of cron is appeared over time as data and the demand for more reports increased. It became difficult to estimate the time a particular job would take.  It often run into lock wait timeouts and deadlocks. Thus, we need a dedicated tool can overcome it. The Apache airflow provides below functions: 
  - Handle complex relationships between jobs.
  - Handle all the jobs centrally with a well defined user interface.
  - Error reporting and alerting.
  - Viewing and analyzing job run times.
  - Security (protecting credentials of databases).

has decided that it is time to introduce more automation and monitoring to their data warehouse ETL pipelines and come to the conclusion that the best tool to achieve this is Apache Airflow.

The source data resides in Amazon S3 and needs to be processed in data warehouse in Amazon Redshift. The source datasets consist of two kind of JSON logs. One is user activity in the application. The other is the songs information.

![Airflow DAG](images/dag.png)

