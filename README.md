# AWS Command Line
A list of helpful AWS Command Line commands

## aws configure
Used to enter your access key id and password along with setting up the region.

Common regions include: <br>
us-east-1, US East (N. Virginia) <br>	
us-east-2, US East (Ohio)	<br>
us-west-1, US West (N. California) <br>	
us-west-2, US West (Oregon)	<br>

```
aws configure | Starts you through configuration
```

## aws iam list-policies
Lists all the IAM policies in JSON format

```
aws iam list-policies | Lists the policies that exist on computer
```

## ssh ec2-user
Used to connect to an EC2 instance <br>
Note: This only works with Mac and Linux operating systems <br>
Note: Make sure that you are located in the same folder as your `.pem` file <br>
Note: If you get a '[.pem file name]: bad permissions' error type `chmod 0400 [.pem file name]` to give it permissions

```
ssh -i [.pem file name] ec2-user@[Public IPv4 address associated with EC2 Instance] | SSHing into EC2 Instance
```
