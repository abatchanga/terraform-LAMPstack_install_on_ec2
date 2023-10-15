# terraform-LAMPstack_install_on_ec22

Objective
After following this tutorial, you should be able to install a Lamp stack server automatically on an EC2 instance using Terraform.

Prerequisites
Terraform must be installed (installation steps here if you have not yet installed it)

aws cli must be installed (installation steps Here) and configured (link here if you have not yet configured AWS-CLI in your terminal)

Let’s follow the steps below to create an EC instance, then install the LAMP stacker server and WordPress on it.

Step 1: Creation of Terraform Configuration files
Creation of the project directory
Before creating the terraform files, let’s create a project directory that will store all those files by using the following steps:

cd into the directory for all your terraform projects created in previous labs



cd ~
cd terraform-projects
If the terraform-projects not yet created, use this command: mkdir terraform-projects

In this directory, create a folder called terraform-lamp-stack for this project and navigate to it:



mkdir terraform-lamp-stack
cd terraform-lamp-stack
Now, we can create terraform files for the project.
