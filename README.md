# cloudformation
Cloudformation documentation: https://docs.aws.amazon.com/cloudformation/

# commands for s3 stack
aws cloudformation create-stack --stack-name nk57xx-s3-bucket-stack --template-body file://s3-bucket.yaml

aws cloudformation describe-stacks --stack-name nk57xx-s3-bucket-stack

aws cloudformation update-stack --stack-name nk57xx-s3-bucket-stack --template-body file://s3-bucket.yaml

aws cloudformation delete-stack --stack-name nk57xx-s3-bucket-stack

# commands for vpc stack
aws cloudformation create-stack --stack-name vpc-stack --template-body file://vpc.yaml

aws cloudformation describe-stacks --stack-name vpc-stack

aws cloudformation update-stack --stack-name vpc-stack --template-body file://vpc.yaml

aws cloudformation delete-stack --stack-name vpc-stack

# commands for iam stack
aws cloudformation create-stack --stack-name iam-stack --template-body file://iam.yaml --capabilities CAPABILITY_NAMED_IAM

aws cloudformation update-stack --stack-name iam-stack --template-body file://iam.yaml --capabilities CAPABILITY_NAMED_IAM