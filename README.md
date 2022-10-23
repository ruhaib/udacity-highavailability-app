# udacity-highavailability-app
This is a high availability app using IaaC (cloudformation) in AWS

Cloud Architecture Chart:
- [Lucidchart shareable Link](https://lucid.app/lucidchart/5ae6888d-632e-47aa-aec7-520d74aa5e2c/edit?viewport_loc=-864%2C-99%2C4195%2C2094%2C0_0&invitationId=inv_c458067b-9820-49e9-a4f1-258a67a4d70b)
- [image](Cloud%20Architecture%20Chart.png)


### Some helpful commands related to this project and udacity aws account:

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