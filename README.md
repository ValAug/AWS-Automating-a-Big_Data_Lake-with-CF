# AWS-Automating-a-Big_Data_Lake-with-CF

## These set of templates will intent to create and deploy secure Data Lake stackset using Cloudformation.  This Stackset use a default VPC for POC presentation.

### Instalation 

1. pip install awscli
2. pip install --upgrade awscli
3. aws configure
4. aws configure --profile <profile-name> # choose profile of preference
5. export AWS_ACCESS_KEY_ID=<access-key-id>
6. export AWS_SECRET_ACCESS_KEY=<secret-access-key>

*Usefull CLI Commands*:
aws --region <region-name> cloudformation validate-template --template-body file://<file-name.yaml>

aws --region <region-name> cloudformation create-stack --stack-name <name> --template-body file://<file-name.yaml>

aws --region <region-name> cloudformation describe-stacks --stack-name <name> --profile <profile-name>

aws --region <region-name> cloudformation update-stack --stack-name <name> --template-body file://<file-name.yaml>

aws --region <region-name> cloudformation delete-stack --stack-name <name> --profile <profile-name>

aws --region <region-name> cloudformation create-stack --stack-name <name> --template-body file://<file-name.yaml> --capabilities CAPABILITY_NAMED_IAM --profile <profile-name>

aws cloudformation estimate-template-cost --template-body file://<file-name.yaml>

# install cfn-lint
pip3 install cfn-lint 
