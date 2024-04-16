# aws-cicd-cross-account-deployment
Cross Account Deployment using Blue/Green strategy with AWS CloudFormation Templates

Deploying Docker images on Amazon Elastic Container Service (ECS) across multiple AWS accounts can be a complex yet essential task for organizations seeking secure and scalable solutions. This guide aims to support AWS customers in achieving this goal by employing a comprehensive approach—leveraging a single CodePipeline, Blue/Green deployment strategy with AWS CodeDeploy, and CloudFormation templates.

The primary purpose of this guide is to facilitate the seamless deployment of Docker images on ECS within three AWS accounts. This is accomplished through the orchestration of resources such as ECS clusters, Amazon Elastic Container Registry (ECR), Virtual Private Clouds (VPC), Security Groups (SG), and CodePipeline using CloudFormation templates. The deployment strategy employed is the robust Blue/Green approach, offering a controlled transition between environments.

Key Features:

Single CodePipeline: Streamlining the deployment process, this guide demonstrates the use of a single CodePipeline to manage the deployment workflow across multiple AWS accounts.

Blue/Green Deployment: The Blue/Green deployment strategy with AWS CodeDeploy ensures minimal downtime and allows for careful validation before transitioning to the new environment.

CloudFormation Templates: Infrastructure as Code (IaC) is implemented through CloudFormation templates, simplifying the creation and management of required resources consistently.

IAM Roles Across Accounts: Secure deployment is achieved by creating and managing IAM roles across all AWS accounts involved in the deployment process.

Automatic and Manual Approvals: The deployment pipeline incorporates both automatic and manual approvals, providing a balance between automation and human validation.

SNS Integration: Notifications are streamlined through Simple Notification Service (SNS), allowing for efficient communication during the deployment process.

![AB2 Arch Diagram](https://github.com/PrachiTembhekar/aws-cicd-cross-account-deployment/assets/60718974/ef5b4142-10c3-4a6b-8d1f-09583c6be5b7)
