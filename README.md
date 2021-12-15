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

### Steps required to solve the given task !!
#### Step 1: Pull code from GitHub. Install and start docker at base OS. Create Dockerfile, run the file and build image using docker file. 

![GitHub Repo](https://user-images.githubusercontent.com/68737245/146204620-6150d3cf-0384-410f-a393-3464c043887e.png)

![Create EC2 Instance](https://user-images.githubusercontent.com/68737245/146205092-6c090f87-0dcd-412b-9644-60c2f81720d5.png)

![Pull Code from GitHub](https://user-images.githubusercontent.com/68737245/146205280-2e58bd8b-c993-45d2-b08c-a6637468bf2f.png)

![Create Docker File](https://user-images.githubusercontent.com/68737245/146205484-f4423212-c2e2-4ad0-8ee6-2a9b014ebbc5.png)

#### Step 2: Push that Image into ECR 

![Create Repo](https://user-images.githubusercontent.com/68737245/146205782-fc4846b8-d67a-42d1-9989-1881671a5172.png)

![Create Repo](https://user-images.githubusercontent.com/68737245/146205947-d2c13874-6f20-49cc-ab96-9970d914cac9.png)

![Push Image into Repo](https://user-images.githubusercontent.com/68737245/146206128-65971b19-a305-4d26-881f-ee35ca7cf14f.png)

![Push Image into Repo](https://user-images.githubusercontent.com/68737245/146206249-6bd8711f-d110-4f16-ab94-baa1b722c446.png)




