# Proxy in Apigee

In Apigee, proxies are a fundamental component of the platform and play a crucial role in API management. Proxies act as intermediaries between client applications and backend services. They receive incoming API requests, apply various policies and transformations, and route the requests to the appropriate backend services.

## Deploy proxies in Apigee using Jenkins

This repository contains Jenkinsfile which has script for deploying proxies in Apigee environments.

For using this template we have to update our Apigee organisation name and credentials in jenkinsfile for parameter:

`def orgList = ['APIGEE_ORGANISATION_NAME']`

`credentialsId: '<gcp_service_account>'`


Create a Jenkins pipeline using this repository and build that pipeline by passing parameters to it. You can select multiple envs at the same time in parameter.


![jenkins_pipeline](https://i.postimg.cc/tRwxn8w9/Screenshot-from-2023-07-15-16-49-29.png)


Build the pipeline and it will deploy proxies in Apigee envs.

To verify this move to:

Apigee > Develop > API Proxies
