# Hyper-V_setup
This article shows you how to create a complete Windows environment and supporting resources with Terraform. Those resources include a virtual network, subnet, public IP address, and more.

Terraform enables the definition, preview, and deployment of cloud infrastructure. Using Terraform, you create configuration files using HCL syntax. The HCL syntax allows you to specify the cloud provider - such as Azure - and the elements that make up your cloud infrastructure. After you create your configuration files, you create an execution plan that allows you to preview your infrastructure changes before they're deployed. Once you verify the changes, you apply the execution plan to deploy the infrastructure.

In this article, you learn how to:

Create a virtual network
Create a subnet
Create a public IP address
Create a network security group and SSH inbound rule
Create a virtual network interface card
Connect the network security group to the network interface
Create a storage account for boot diagnostics
Create a virtual machine with an IIS web server
View the web server page

# Implement the Terraform code

Create a directory in which to test the sample Terraform code and make it the current directory.

Create a file named providers.tf and insert the following code:Create a file named main.tf and insert the following code:
Create a file named main.tf and insert the following code:


# Initialize Terraform
Run terraform init to initialize the Terraform deployment. This command downloads the Azure provider required to manage your Azure resources.

# Create a Terraform execution plan
Run terraform plan to create an execution plan.

# Apply a Terraform execution plan
Run terraform apply to apply the execution plan to your cloud infrastructure.

# Clean up resources
When you no longer need the resources created via Terraform, do the following steps:

Run terraform plan and specify the destroy flag