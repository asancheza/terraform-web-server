# Terraform Web Server Template

This repository provides a Terraform template for deploying a basic web server on AWS. The template is designed to simplify the process of setting up a web server by using Terraform's infrastructure as code capabilities.

## Project Overview

The Terraform configuration in this repository allows users to easily deploy a web server on AWS with a few commands. It leverages AWS resources to ensure scalability and reliability.

## Prerequisites

To use this template, you will need:

- [Terraform](https://www.terraform.io/) installed on your local machine.
- An AWS account with the necessary permissions to create resources such as EC2 instances.
- AWS credentials set up on your machine as environment variables.

## Installation and Usage

Follow these steps to set up and deploy the web server:

1. **Install Terraform**: 
   Ensure that Terraform is installed by following the instructions on [Terraform's website](https://www.terraform.io/downloads.html).

2. **Configure AWS Credentials**: 
   Set your AWS credentials as environment variables on your machine:
   
   ```bash
   export AWS_ACCESS_KEY_ID="your_access_key_id"
   export AWS_SECRET_ACCESS_KEY="your_secret_access_key"
   ```

3. **Initialize Terraform**: 
   Run the following command to initialize the directory containing the Terraform configuration files. This step downloads the necessary provider plugins:
   
   ```bash
   terraform init
   ```

4. **Plan the Deployment**: 
   Execute the plan command to see what changes Terraform will make:
   
   ```bash
   terraform plan
   ```
   Review the plan output to ensure everything looks good.

5. **Apply the Terraform Plan**: 
   If the plan looks good, apply it to deploy the resources:
   
   ```bash
   terraform apply
   ```
   Confirm the action when prompted.

## File Overview

- **main.tf**: Contains the Terraform configuration for setting up the web server resources on AWS.
- **outputs.tf**: Defines the outputs of the Terraform deployment, such as server IP addresses.
- **vars.tf**: Contains variable definitions that can be customized to modify the Terraform deployment.

## Author

This project is maintained by [Alejandro Acosta](https://github.com/asancheza).

## License

No license information is provided. Please contact the author for more details on usage.

## Contributions

Contributions to this project are welcome. Please fork the repository and submit a pull request for review.