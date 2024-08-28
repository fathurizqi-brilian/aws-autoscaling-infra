# aws-autoscaling-infra
Create AWS EC2 Autoscaling infrastructure using CloudFormation

You need to deploy each file sequencially using command "aws deploy ..."

Here is the command to deploy resources in ap-southeast-1

1. aws cloudformation deploy --template-file 1_IAC-network.yml --stack-name IAC-Networking --region ap-southeast-1

2. aws cloudformation deploy --template-file 2_IAC-instance.yml --stack-name IAC-Instance --region ap-southeast-1

3. aws cloudformation deploy --template-file 3_IAC-autoscaling.yml --stack-name IAC-Autoscaling --region ap-southeast-1