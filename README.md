# udacity-highavailability-app
This is a high availability app using IaaC (cloudformation) in AWS

```export AWS_DEFAULT_PROFILE=udacity-admin```

```
aws cloudformation create-stack --stack-name udacity-project-network --template-body file://stacks/network/network.yml --parameters file://stacks/network/network.json --region=us-east-1
```

```
aws cloudformation create-stack --stack-name udacity-project-servers --template-body file://stacks/servers/servers.yml --parameters file://stacks/servers/servers.json --region=us-east-1 --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM"
```

```
aws configure
```

```
aws configure set aws_session_token ""
```