# AWS Services

## Technologies used:

- AWS, Docker, Linux, Jenkins, Git, Java, Maven, Docker Hub

## Job 1: Deploy Web Application on EC2 Instance (manually)
#### Job description:

- Create and configure an EC2 Instance on AWS
- Install Docker on remote EC2 Instance
- Deploy Docker image from private Docker repository on EC2 Instance

## Job 2: CD - Deploy Application from Jenkins Pipeline to EC2 Instance (automatically with docker)
#### Job description:

- Prepare AWS EC2 Instance for deployment (Install Docker)
- Create ssh key credentials for EC2 server on Jenkins
- Extend the previous CI pipeline with deploy step to ssh into the remote EC2 instance and deploy newly built image from Jenkins server
- Configure security group on EC2 Instance to allow access to our web application

## Job 3: CD - Deploy Application from Jenkins Pipeline on EC2 Instance (automatically with docker-compose)
#### Job description:

- Install Docker Compose on AWS EC2 Instance
- Create docker-compose.yml file that deploys the web application image
- Configure Jenkins pipeline to deploy newly built image using Docker Compose on EC2 server
- Improvement: Extract multiple Linux commands thatvare executed on remote server into a separate shell script and execute the script from Jenkinsfile

## Job 4: Complete the CI/CD Pipeline (Docker-Compose, Dynamic versioning)
#### Job description:

- CI step: Increment version
- CI step: Build artifact for Java Maven application
- CI step: Build and push Docker image to Docker Hub
- CD step: Deploy new application version with Docker Compose
- CD step: Commit the version update

## Job 5: Interacting with AWS CLI
#### Job description:

- Install and configure AWS CLI tool to connect to our AWS account
- Create EC2 Instance using the AWS CLI with all necessary configurations like Security Group
- Create SSH key pair
- Create IAM resources like User, Group, Policy using the AWS CLI
- List and browse AWS resources using the AWS CLI
