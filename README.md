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
This only works with Mac and Linux operating systems <br>
Make sure that you are located in the same folder as your `.pem` file

```
ssh -i [.pem file name] ec2-user@[Public IPv4 address associated with EC2 Instance] | SSHing into EC2 Instance
```
