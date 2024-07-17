# AWSNEW

1. API GATEWAY 
# IAM Role for API Gateway
apigateway.amazonaws.com

# IAM Policy for API Gateway
execute-api:Invoke

2. CLOUD WATCH
# IAM Role for cloud watch
logs.amazonaws.com

#IAM Policy for CloudWatch Logs
logs:CreateLogGroup",
logs:CreateLogStream
logs:PutLogEvents"

3. DYNAMODB
# IAM Role for Dynamodb
dynamodb.amazonaws.com

#IAM Policy for Dynamodb 
AllowAllPermissions

"NotAction": [
        "lightsail:*",
        "sagemaker:*"
      ],
      
#KMS KEY
      
      
      
4. EC2
# IAM Role for EC2
ec2.amazonaws.com

#IAM Policy for EC2
AllowAllPermissions

"NotAction": [
        "lightsail:*",
        "sagemaker:*"
      ],
#kms key
      
      
5. EC2 AMI

# IAM Role for EC2 AMI
ec2.amazonaws.com     

#IAM Policy for EC2 AMI

"ec2:CreateImage",
        "ec2:DescribeImages",
        "ssm:UpdateInstanceInformation",
        "ssmmessages:CreateControlChannel",
        "ssmmessages:CreateDataChannel",
        "ssmmessages:OpenControlChannel",
        "ssmmessages:OpenDataChannel",
        "ec2:RegisterImage",
        "ec2:RunInstances"  
      
#KMS KEY

6. ECR 
# IAM Role for ECR
ecr.amazonaws.com

# IAM Policy for ECR
          "ecr:GetDownloadUrlForLayer",
          "ecr:BatchGetImage",
          "ecr:BatchCheckLayerAvailability"
 
#KMS KEY

7. ECS CLUSTER
# # IAM Role for ECS CLUSTER
ecs.amazonaws.com

# IAM Policy for ECS CLUSTER
        "ecs:Describe*",
        "ecs:List*"
 
#KMS KEY        
        
8. ECS SERVICE 
# IAM Role for ECS SERVICE
ecs.amazonaws.com

# IAM Policy for ECS SERVICE
          "logs:CreateLogStream",
          "logs:PutLogEvents"
          
#KMS  KEY

9. EKS
# IAM Role for EKS
eks.amazonaws.com

# IAM Policy for EKS
        "eks:DescribeCluster",
        "eks:ListNodegroups",
        "eks:CreateNodegroup",
        "eks:DeleteNodegroup",
        "eks:UpdateNodegroupConfig",
        "eks:TagResource"
          
#KMS KEY          
        
 
