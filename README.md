# AWS_EC2_with_Terraform

In this project, as a very basic IaC, I will provision an AWS EC2 instance using Terraform. 

## Connect to AWS and configuration directory

First I connect to my AWS account via the AWS CLI. 

![Screenshot (274)](https://github.com/user-attachments/assets/587b1d0d-8a43-4b6b-98d0-f2b6afb67069)

Then I create the working directory for my configuration and I change into it.

![Screenshot (276)](https://github.com/user-attachments/assets/db8cc92b-5842-45ed-b775-6e1d7867489e)

## Create the infrastructure and launch the instance

After that I create the file to define my infrastructure and I enter the following configuration.

![Screenshot (277)](https://github.com/user-attachments/assets/304a0c9c-d06d-4397-9586-830e226585e0)
![Screenshot (281)](https://github.com/user-attachments/assets/36d96dbe-b77f-46fd-8a98-cfccb1da1fe4)

I save the file and initialize the directory.

![Screenshot (279)](https://github.com/user-attachments/assets/7f740275-5342-4a4e-9161-bbbcbf07c988)

Then I use the command terraform apply to apply the configuration. It prints out the execution plan and I accept it.

![Screenshot (282)](https://github.com/user-attachments/assets/462fd7cd-3a0e-4707-b25f-9d487a96f4a4)
![Screenshot (283)](https://github.com/user-attachments/assets/b70e0aac-04b6-4f86-858c-56b553ced2a4)

## Inspect the outcome on the console

In order to verify the launch of my EC2 instance, I log in to the AWS Management Console, in the EC2 instances section, where I see my newly created instance.

![Screenshot (284)](https://github.com/user-attachments/assets/6147a6b0-b7ec-4d27-b888-d965d90d4817)

## Clean up resources and verify

Finally I use the command terraform destroy to terminate the EC2 instance.

![Screenshot (285)](https://github.com/user-attachments/assets/61d279f2-ef8e-4406-80af-cacedd642c10)
![Screenshot (286)](https://github.com/user-attachments/assets/9305a7ad-d39b-4fe2-b790-6982aab4fe92)
![Screenshot (287)](https://github.com/user-attachments/assets/6b85da07-509d-4b9d-aff4-6fde7736e1c2)

As a last step, I head again to the AWS Management Console to verify the termination of the instance.

![Screenshot (288)](https://github.com/user-attachments/assets/4905d893-a653-4b83-95d0-cbf010b78db9)

It was successfully terminated.
