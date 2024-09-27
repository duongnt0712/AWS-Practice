# AWS-Practice
This repo will aggregate the use cases for studying purpose.

## Prerequisite
### AWS CLI

### AWS Credentials
To check if AWS Credentials is associated with ACCESS_KEY and SECRET_KEY in your workspace:
```aws configure```

To check if the AWS CLI is configured:
```aws configure list```

#### AWS CloudFormation 
To create AWS CloudFormation stack:
```
aws cloudformation create-stack \
    --stack-name your-stack-name \
    --template-body file://template.yaml \
    --parameters ParameterKey=ProjectName,ParameterValue=main-project ParameterKey=EnvironmentName,ParameterValue=dev
```
