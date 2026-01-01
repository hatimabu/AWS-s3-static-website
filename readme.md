# AWS S3 Static Website (Terraform)

This project deploys a simple static website to AWS S3 using Terraform.  
It demonstrates core Infrastructure-as-Code concepts and serves as a clean, minimal example of AWS provisioning.

## 🚀 Features

- S3 bucket created via Terraform
- Static website hosting enabled
- Public read access configured
- HTML file automatically uploaded
- Website URL output after deployment

## 📁 Project Structure

aws-s3-static-website/
│
├── main.tf
├── variables.tf
├── outputs.tf
└── index.html

## 🛠️ Requirements

- Terraform ≥ 1.0
- AWS CLI configured (`aws configure`)
- An AWS account
- A globally unique S3 bucket name

## 🔧 Deployment

### 1. Initialize Terraform

terraform init

### 2. Apply the configuration

Replace the bucket name with your own unique name:

terraform apply -var="bucket_name=your-unique-bucket-name"

Type `yes` when prompted.

## 🌐 Access Your Website

After deployment, Terraform outputs:

website_url = http://your-bucket-name.s3-website-us-east-1.amazonaws.com

Open the URL in your browser — your website is live.

## 🧹 Cleanup

To remove all resources:

terraform destroy

## 📚 What This Project Demonstrates

- AWS S3 static hosting
- Terraform resource creation
- Bucket policies
- File uploads via Terraform
- Clean IaC project structure

This project is ideal for cloud/DevOps portfolios and interview discussions.

## ✨ Author

Built by Hatim — Cloud & DevOps Engineer in progress.