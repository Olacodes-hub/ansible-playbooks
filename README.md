# Hosting an EC2 Website with Ansible Playbooks

This repository contains Ansible playbooks to automate the process of hosting a website on an EC2 instance. By following these steps, you can quickly set up and deploy a website on AWS.

## Getting Started

### Prerequisites

1. **AWS Account:** You will need an AWS account with appropriate permissions to create EC2 instances.

2. **Ansible:** Ensure Ansible is installed on your local machine. If not, you can download it from [Ansible's official website](https://www.ansible.com/).

3. **SSH Key Pair:** Create an SSH key pair to access your EC2 instances securely. Make note of the private key file.

### Repository Setup

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/ansible-ec2-website.git
   
Navigate to the repository directory: 
cd ansible-ec2-website
Configure AWS Credentials:

Open the aws_config.yml file and provide your AWS access key, secret key, and the desired AWS region.

Customize Website Configuration
Edit the website.yml playbook:

Specify the domain name, web server, and database type in the playbook. You can adjust other variables as needed.
Save the changes.

Deploy Your Website
Run the Ansible playbook to create and configure the EC2 instance:

Directory Structure
ansible.cfg: Ansible configuration file.
hosts.ini: Inventory file containing the EC2 instance details.
aws_config.yml: Configuration file for AWS credentials.
website.yml: Main playbook for deploying the website.
roles/: Directory containing Ansible roles for web server and database setup.
templates/: Contains templates for web server and database configuration.
