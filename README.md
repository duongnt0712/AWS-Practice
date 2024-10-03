# AWS-Practice
This repo will aggregate the use cases for studying purpose.

## Prerequisite
### AWS CLI

### AWS Credentials
To check if AWS Credentials is associated with ACCESS_KEY and SECRET_KEY in your workspace:
```
aws configure
```

To check if the AWS CLI is configured:
```
aws configure list
```

#### AWS CloudFormation 
##### To create stack:
```
aws cloudformation create-stack \
    --stack-name demo-main \
    --template-body file://main.yaml \
    --parameters ParameterKey=ProjectName,ParameterValue=cloudformation-project ParameterKey=EnvironmentName,ParameterValue=Development
    --capabilities CAPABILITY_IAM CAPABILITY_NAMED_IAM CAPABILITY_AUTO_EXPAND
```
##### To update stack:
```
aws cloudformation create-stack \
    --stack-name demo-main \
    --template-body file://main.yaml \
    --parameters ParameterKey=ProjectName,ParameterValue=cloudformation-project ParameterKey=EnvironmentName,ParameterValue=Development \
    --capabilities CAPABILITY_IAM CAPABILITY_NAMED_IAM CAPABILITY_AUTO_EXPAND
```
- CAPABILITY_IAM: Allows CloudFormation to create IAM roles and policies.
- CAPABILITY_NAMED_IAM: Allows CloudFormation to create IAM resources with specified names.
- CAPABILITY_AUTO_EXPAND: Allows CloudFormation to perform actions that automatically expand macros in your template.
