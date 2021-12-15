# QuizAppTask
### Run the Web Application using AWS services !!!
#### What is AWS ??
##### The full form of AWS is Amazon Web Services. It is a platform that offers flexible, reliable, scalable, easy-to-use and, cost-effective cloud computing solutions. AWS is a comprehensive, easy to use computing platform offered Amazon. The platform is developed with a combination of infrastructure as a service (IaaS), platform as a service (PaaS) and packaged software as a service (SaaS) offerings.

#### What is ECR ??
##### Amazon Elastic Container Registry (Amazon ECR) is an AWS managed container image registry service that is secure, scalable, and reliable. Amazon ECR supports private repositories with resource-based permissions using AWS IAM. You can use your preferred CLI to push, pull, and manage Docker images, Open Container Initiative (OCI) images, and OCI compatible artifacts.

#### What is ECS ??
##### Amazon Elastic Container Service (Amazon ECS) is a highly scalable, fast container management service that makes it easy to run, stop, and manage containers on a cluster. Your containers are defined in a task definition that you use to run individual tasks or tasks within a service. Amazon ECS enables you to launch and stop your container-based applications by using simple API calls.

#### What is AWS Lambda ??
##### AWS Lambda is an event-driven, serverless computing platform provided by Amazon as a part of Amazon Web Services. Therefore you don’t need to worry about which AWS resources to launch, or how will you manage them. Instead, you need to put the code on Lambda, and it runs. In AWS Lambda the code is executed based on the response of events in AWS services such as add/delete files in S3 bucket, HTTP request from Amazon API gateway, etc. However, Amazon Lambda can only be used to execute background tasks.

#### What is AWS API Gateway ??
##### It’s a fully managed service that provides all the necessary tools for developers in order to create, publish, manage and secure your API regarding of scale. Amazon API Gateway will take care of all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management.

## Steps required to solve the given task !!
### Step 1: Pull code from GitHub. Install and start docker at base OS. Create Dockerfile, run the file and build image using docker file. 

![GitHub Repo](https://user-images.githubusercontent.com/68737245/146204620-6150d3cf-0384-410f-a393-3464c043887e.png)

![Create EC2 Instance](https://user-images.githubusercontent.com/68737245/146205092-6c090f87-0dcd-412b-9644-60c2f81720d5.png)

![Pull Code from GitHub](https://user-images.githubusercontent.com/68737245/146205280-2e58bd8b-c993-45d2-b08c-a6637468bf2f.png)

![Create Docker File](https://user-images.githubusercontent.com/68737245/146205484-f4423212-c2e2-4ad0-8ee6-2a9b014ebbc5.png)


### Step 2: Push that Image into ECR 


![Create Repo](https://user-images.githubusercontent.com/68737245/146205782-fc4846b8-d67a-42d1-9989-1881671a5172.png)

![Create Repo](https://user-images.githubusercontent.com/68737245/146205947-d2c13874-6f20-49cc-ab96-9970d914cac9.png)

![Push Image into Repo](https://user-images.githubusercontent.com/68737245/146206128-65971b19-a305-4d26-881f-ee35ca7cf14f.png)

![Push Image into Repo](https://user-images.githubusercontent.com/68737245/146206249-6bd8711f-d110-4f16-ab94-baa1b722c446.png)

![Details of Repo](https://user-images.githubusercontent.com/68737245/146213850-0620000f-7e7f-4566-8d53-d1715c4b639c.png)


### Step 3: Create ECS cluster for EC2 t2 micro, create a task in ECS for the service to start the app.

![Create ECS cluster](https://user-images.githubusercontent.com/68737245/146214416-ab89886c-10de-424e-8082-7fd299a49304.png)

![Create ECS cluster](https://user-images.githubusercontent.com/68737245/146214564-f8a7b3d8-d428-4e1d-9d46-a9b0b67f3184.png)

![Details of ECS Cluster](https://user-images.githubusercontent.com/68737245/146214755-50d98b52-9bb3-44c4-b1be-2d64c1b05e5a.png)

![Task Defination](https://user-images.githubusercontent.com/68737245/146214888-e0c32013-6dd1-4213-8db0-ab7bcb9f215d.png)

![Task Defination](https://user-images.githubusercontent.com/68737245/146215161-59617892-6bb8-4d86-8228-9283a02f3426.png)

![Output of the App](https://user-images.githubusercontent.com/68737245/146216464-3ce27703-9e2b-4c96-95c1-77a20a8da059.png)


### Step 4: Create API Gateway and AWS Lambda function to make an endpoint to start the app.

#### I have created QuizApp lambda function which hit the ECS cluster and run the task when I call the API and give the output "Output from ECS Task !!".

![Lambda Function](https://user-images.githubusercontent.com/68737245/146217092-82fa67fd-10ab-4510-8621-f81263282b7e.png)

![Lambda Function](https://user-images.githubusercontent.com/68737245/146217222-58c0ffd7-53bb-4bf0-a610-5925067965f0.png)

#### Creation of API using API Gateway.

![Creation of API using API Gateway](https://user-images.githubusercontent.com/68737245/146217436-641e1d9a-e1d9-4620-8563-a3af40925c6e.png)

#### Output of lambda function.

![Running the task](https://user-images.githubusercontent.com/68737245/146217824-c51a161c-cf30-4d8c-900b-7eca2769d29a.png)

![Console output](https://user-images.githubusercontent.com/68737245/146217930-c7b87f5d-5126-4c90-9168-7172387a04ce.png)

[Hit the url to see the output of lambda function](https://ryeel9tmsi.execute-api.ap-south-1.amazonaws.com/default/QuizApp)

## Thank You so for reading !!! 
