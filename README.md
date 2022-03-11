# AWS CodeDeploy Demo

## The required files for codedeploy to work - 
1. appspec.yml
2. Scripts folder
3. Your application code (html file here)
---

## You can refer to this blog on medium: 


---

## Steps : 

1. Create IAM Roles : CodeDeployRole & EC2DeployRole

2. Create EC2 instance with following categories

	a. Select the AMI as Amazon Linux 2 AMI

	b. Select the Instance type: t2.micro

	c. During configurion of the instance: Choose EC2CodeDeploy IAM role

	d. Tag the name with a name of your choice.

	e. Configure Security Group: 

		HTTP TCP 80 0.0.0.0/0

		HTTP TCP 80 ::/0

		SSH TCP 22 (YOUR IP ADDRESS)

		HTTPS TCP 443 0.0.0.0/0

		HTTPS TCP 443 ::/0

	f. click on launch instance

3. Login to EC2 instance and install the code deploy agent
4. Do the deployment
---
