## What is a Jenkins Pipeline?

Suite of Jenkins features, installed as plugins, which enable implementation of 
continuos delivery pipelines, which are automated processes for getting software from 
source control through deployment to end users. 


## Jenkins at its core?

Supports building Continuos Delivery Pipelines through either a Web UI or a scripted 
Jenkinsfile. These are coded in the Groovy DSL. 

## 2 Ways of Coding Jenkins Pipeline: 

1. Scripted Groovy DSL
2. Declarative : Declarative is a recent feature and is very powerful.  

## Key Features of Jenkins Pipeline: 

- Code Your Pipeline & maintain it on git 
- Handles user input
- Parrallel job execution 
- Complex pipelines possible (Use conditional when and iterative for loops)


## Declarative vs Scripted 

1. 
- D:Recent features in jenkins & uses a simpler groovy syntax 
- S:Traditional way of writing Jenkins Pipeline with a stricter groovy syntax. 

2.
- D:Code ie written locally in a file & is checked in to the SCM. 
- S:Code is written directly on the Jenkins instance

3.
- D:Code is written within a pipeline block
- S:Code is written within a node block