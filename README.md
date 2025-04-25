How to install Terraform on Windows and run your first project
This post is helpful for installing the Terraform on windows and running your first Terraform module.
Module: Creating the EC2 instance with the help of Terraform
Requirements: AWS, Vs code and Terraform.

Follow the below steps:-

Install the latest version of Terraform from there official documentation and AWS CLI
Terraform: https://developer.hashicorp.com/terraform/install
AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

Terraform is not like other executable .exe we just need to download it and check by opening CMD in the same folder and run the below command

terraform -v
If You see the below output then congratulation its installed.

Terraform v1.11.4
3.Now open the same folder in VS-Code and try to check there as well in the new terminal.

4.Install the 2 extension now AWS Toolkit and Terraform

AWS toolkit: click on the extension after installing it then click on View from the top bar then click on command pallette then type AWS:create credentials profile it will ask for key and secrets give them one by one done.( you will get key from your aws ac)
Terraform: just install this extension no need to do the configuration.
Create the new file main.tf and paste the data over there which we are going to use to run the terraform this data is in HCL language you can refer below documentation for that
https://registry.terraform.io/providers/hashicorp/aws/latest/docs

Below I am providing the my Github repository link where I have store my code just replace access key, secret key and the AMI according to the AWS region and add this code to you main.tf

https://github.com/I-am-nk/Terraform

7.After adding code to the main.tf run the below sets of command
a.

terraform init

b.

terraform plan
( after running this command it will ask for pem file name give the name according to you)
c.

terraform apply
d.

terraform destroy
(run it only you want to destroy the script)
