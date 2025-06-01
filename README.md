Terraform AWS S3 Project

This project demonstrates Infrastructure as Code (IaC) using Terraform to automate a private AWS S3 bucket in the us-east-1 region. It includes variables for reusability, ownership controls, and a private ACL, showcasing real-world DevOps skills for cloud infrastructure automation.

Features





Terraform configuration for an AWS S3 bucket.



Variables for region and bucket name for reusability.



Private bucket with ownership controls.



Automated setup and teardown (AWS free tier).



Professional GitHub repository.

Prerequisites





Terraform



AWS CLI (configured)



AWS account with IAM user (AmazonS3FullAccess)



Git



GitHub account

Setup Instructions





Clone the repository:

git clone https://github.com/your-username/terraform-s3.git
cd terraform-s3



Configure AWS CLI:

aws configure

Enter AWS Access Key ID, Secret Access Key, region (e.g., us-east-1), output (json).



Initialize Terraform:

terraform init



Plan the deployment:

terraform plan



Apply the configuration:

terraform apply

Type yes. Verify in AWS S3 console.



Destroy the infrastructure:

terraform destroy

Type yes.

Terraform Configuration





main.tf: AWS provider, S3 bucket, ownership controls, private ACL.



variables.tf: Defines reusable variables for region and bucket name.



.gitignore: Excludes Terraform state and .terraform/ directory.



Bucket name must be globally unique (e.g., yourname-bucket-2025-xyz).

Challenges Faced





Mastered Terraform syntax and AWS provider setup.



Configured AWS CLI and IAM on Windows.



Ensured bucket name uniqueness with random suffixes.



Added variables for reusable Terraform code.

Future Improvements





Add outputs to display bucket details.



Include more AWS resources (e.g., IAM, CloudFront).



Integrate CI/CD for automated Terraform deployments.

Author





Your Name (GitHub)



Connect on LinkedIn