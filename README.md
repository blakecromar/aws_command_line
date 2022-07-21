# AWS Command Line
A list of helpful AWS Command Line commands

## How to configure your AWS
Used to enter your access key id and password along with setting up the region.

Common regions include: <br>
us-east-1, US East (N. Virginia) <br>	
us-east-2, US East (Ohio)	<br>
us-west-1, US West (N. California) <br>	
us-west-2, US West (Oregon)	<br>

```
aws configure | Starts you through configuration
```

## List all policies
Lists all the IAM policies in JSON format

```
aws iam list-policies | Lists the policies that exist on computer
```

## How to SSH with the correct command
Used to connect to an EC2 instance <br><br>
Note: This only works with Mac and Linux operating systems <br>
Note: Make sure that you are located in the same folder as your `.pem` file <br>
Note: If you get a '[.pem file name]: bad permissions' error type `chmod 0400 [.pem file name]` to give it permissions

```
ssh -i [.pem file name] ec2-user@[Public IPv4 address associated with EC2 Instance] | SSHing into EC2 Instance
```

## exit or control+d
Use this command to exit out of an instance user session.

```
exit (or control+d) | Used to exit out of instance.
```
## How to get your AWS version

```
aws --version | Finding the aws version number
```

## How to stress an AWS EC2 Instance

If you haven't already use these commands if you haven't already
```
sudo amazon-linux-extras install epel -y
sudo yum install stress -y
```
Run this command
```
stress -c [NUMBER OF CPUS] | This is often 4, but could be more
```
