Terraform AWS Infrastructure Project 🚀
Project Description
This project demonstrates the use of Terraform to automate the provisioning of AWS infrastructure. The setup includes the creation of an EC2 instance, automated web server deployment, and the secure storage of the Terraform state file in an S3 bucket. The infrastructure is fully scalable, modular, and emphasizes best practices for Infrastructure as Code (IaC).

Features
🚀 Infrastructure as Code (IaC): Automated infrastructure setup using Terraform.
🌐 EC2 Instance Creation: Deploys an Amazon EC2 instance with required configurations.
🖥️ Web Server Provisioning: Automatically provisions and configures a web server on the EC2 instance.
🔒 State Management: Stores the Terraform statefile in an encrypted S3 bucket for enhanced collaboration and disaster recovery.
📦 Reusable Modules: Ensures scalability and modularity in the code for reusability.
Prerequisites
Before running this project, ensure the following tools are installed on your system:

Terraform (v1.x or later)
AWS CLI (Configured with appropriate credentials)
A valid AWS account with the necessary permissions.
Usage
1. Clone the repository
bash
Copy code
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
2. Initialize Terraform
bash
Copy code
terraform init
3. Review the Terraform Plan
bash
Copy code
terraform plan
4. Apply the Configuration
bash
Copy code
terraform apply
5. Access the Web Server
Once the setup is complete, you can access the web server using the Public IP of the provisioned EC2 instance.
File Structure
bash
Copy code
.
├── main.tf            # Main Terraform configuration file
├── variables.tf       # Input variables
├── outputs.tf         # Output definitions
├── statefile.tf       # Backend configuration for storing state in S3
├── README.md          # Project documentation
Key Highlights
EC2 Instance Setup: The EC2 instance is launched using a custom AMI and security group configurations for enhanced performance and security.
Web Server Automation: The provisioning script automatically installs and configures a web server (e.g., Apache/NGINX).
S3 Backend: Terraform state is securely stored in an S3 bucket, ensuring team collaboration and disaster recovery.
AWS Services Used
EC2: Compute instance to host the web server.
S3: Secure backend storage for Terraform state files.
IAM: Roles and policies for secure access management.
How to Customize
To customize the infrastructure:

Modify the variables in the variables.tf file.
Adjust the security group rules in the main.tf file.
Update the web server provisioning script as needed.
License
This project is licensed under the MIT License.

Author
Pepsh

LinkedIn: Your LinkedIn
GitHub: Pepuhove
Feel free to contribute or raise issues in this repository!

