# Jenkins on ECS

CloudFormation stack for creating an ECS service for Jenkins.

## Launching Stack

Make sure you are logged into the AWS Console and have permissions then click:

[![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/template?stackName=ecs-jenkins-stack&templateURL=https://sumu-stacks.s3.us-east-1.amazonaws.com/jenkins/production/cloudformation/jenkins/top.yaml)

Fill out the parameters and launch!

---

Creates:

- ALB
- DNS Records (optional)
- ECS Service
- ECS Task

Requires:

- ECS Cluster
- VPC Id
- ACM Certificate
- Subnet Ids
