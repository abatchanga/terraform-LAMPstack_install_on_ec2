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
cd ~
cd terraform-projects

mkdir terraform-lamp-stack
cd terraform-lamp-stack


Creation of the Terraform files
code main.tf
code var.tf
code provider.tf
code output.tf
code install_lamp.sh



Step 2: Launch the EC2 instance
Let’s initialize our infrastructure using the following command in the terminal:

terraform init

Now, let's run the following command to get a plan of resources that will be created for our infrastructure:

terraform plan

Run this command to launch an EC2 instance and all resources needed:

terraform apply --auto-approve
Once completed, you will get the output below:


Step 3: WordPress Configuration
Copy the URL of the lamp stack server and paste it into the browser, you will get the result as in the following image:

For the WordPress installation, choose the language English and continue:

Now, fill out the form as in the following image and click on Install WordPress

Username: student

Password: school1

You can now log in with the user student and its password school1.

The dashboard will open: this is the backend of the website. If you click on the name of the site, you will have a default preview

We can change the theme of the site by going back to the dashboard

Click on Appearance then Themes and Activate one

Choose one theme and click on Activate to enable it.

Preview the site once more

This is how some websites are easily set up with Wordpress!

You will get the final result:

You successfully installed LAMP stack and WordPress on an EC2 instance :grinning: 


Step 4: Destroy the infrastructure
Once you have done, you can use the following command to destroy all resources created in AWS:

terraform destroy --auto-approve
