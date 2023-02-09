# Piepeline description
I used pipeline consists of tow main jops as follow
* **Build** jop that build both frontend and backend 
* **Deploy** that deploy both frontend and backend

## My orbsa that pipeline depends on

*  for **node** I use circleci/node@5.0.2
*  for **aws-cli** I use circleci/aws-cli@1.3.1
*  for **eb** I use circleci/aws-elastic-beanstalk@1.0.0

## In build jop the workflow as follow
1- Install node versoin 14.15
2- Checkout the repo
3- Install Front-End Dependencies
4- Install API Dependencies
5- Build Front-End project
6- Build API project

## In deploy jop the workflow as follow
1- Install node versoin 14.15
2- Install eb
3- Install aws-cli
4- Checkout the repo
5- set project environment
6- Deploy both frontend and backend
