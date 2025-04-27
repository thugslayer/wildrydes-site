# AWS Project

Wild Rides is a fully serverless ride-sharing web application built using AWS services. Instead of managing traditional servers, the app uses AWS Amplify for hosting the frontend, Amazon Cognito for user authentication, API Gateway to expose secure APIs, AWS Lambda for backend processing, and DynamoDB for storing ride details. Users register and log in via Cognito, click on a map to request a unicorn ride, and the system processes their request entirely through serverless functions. The project demonstrates how to create a scalable, cost-effective, and low-maintenance cloud-native app, offering hands-on experience with modern serverless architecture and CI/CD deployment through GitHub and Amplify.

## Services used:

- **AWS Amplify**: A platform to build, host, and deploy full-stack web and mobile applications easily.
- **Amazon Cognito**: A service for adding user sign-up, login, and authentication to your applications securely.
- **Amazon API Gateway**: A fully managed service to create, publish, maintain, and secure APIs at any scale.
- **AWS Lambda**: A compute service that lets you run code in response to events without provisioning or managing servers.
- **Amazon DynamoDB**: A fast and flexible NoSQL database service for storing and retrieving any amount of data with low latency.
- **AWS IAM (Identity and Access Management)**: A service to securely manage access to AWS resources by creating users, groups, roles, and permission policies.

## Implementation:

### Step 1: Set Up GitHub Repository
- Create a GitHub repo and upload frontend code.
### Step 2: Deploy Frontend with AWS Amplify
- Connect GitHub repo to Amplify for hosting and automatic deployment.
### Step 3: Set Up User Authentication with Amazon Cognito
- Create a Cognito User Pool, configure password policies, and create an App Client.
- Update the frontend `config.js` file with the User Pool ID and App Client ID.
### Step 4: Create DynamoDB Table
- Create a table called `Rides` with `rideID` as the partition key.
### Step 5: Set Up IAM Role for Lambda
- Create a Lambda execution role with DynamoDB write permissions.
### Step 6: Create AWS Lambda Function
- Code Lambda to handle ride requests, select a unicorn, and save data to DynamoDB.
### Step 7: Set Up API Gateway
- Create a REST API linked to Lambda.
- Add Cognito authentication and enable CORS.
### Step 8: Connect Frontend to Backend
- Update frontend to call API Gateway using authenticated user tokens.
### Step 9: Test the Application
- Register a user, log in, request a ride, and verify data in DynamoDB..

