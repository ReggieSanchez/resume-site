# 🌐 Cloud Resume Project – Reggie Sanchez

[![Live Website](https://img.shields.io/badge/Live%20Site-View%20Resume-39FF14?style=for-the-badge&logo=amazon-aws&logoColor=black)](https://resume.whoisreggiesanchez.com)

🚀 **Overview**

This project showcases a fully serverless, cloud-hosted resume built on AWS with modern DevOps practices:

- **Infrastructure as Code:** Terraform provisions and manages all resources.
- **CI/CD Pipeline:** GitHub Actions automatically deploys updates to S3 and CloudFront.
- **Dynamic Features:**
  - Visitor counter using Lambda + API Gateway + DynamoDB
  - Dark mode with rotating themes
  - Custom circuit board SVG background
  - Downloadable PDF resume
  - Verified GitHub and LinkedIn links
- **Custom Domain:** `resume.whoisreggiesanchez.com` served via CloudFront CDN.
- **Security:** CSP headers and HTTPS enforced.

---

## 🛠️ **Tech Stack**

| Category              | Service / Tool                       |
|-----------------------|--------------------------------------|
| Infrastructure        | Terraform                            |
| Cloud Provider        | AWS                                  |
| Storage               | S3 Static Website Hosting            |
| CDN & HTTPS           | CloudFront + ACM                     |
| Serverless Functions  | Lambda (Visitor Counter)             |
| API Gateway           | REST API for Lambda Invocation       |
| Database              | DynamoDB (Visit Tracking)            |
| Notifications         | SNS/SQS (Planned)                    |
| CI/CD                 | GitHub Actions                       |
| Frontend              | HTML, CSS, JavaScript                |
| Design                | Font Awesome Icons, Custom CSS       |
| Domain Registrar      | Namecheap / Route53                  |

---

## ✨ **Features**

✅ **Serverless Visitor Counter**

Every page load increments a DynamoDB counter via Lambda triggered by API Gateway.

✅ **Dark Mode with Multiple Themes**

Click the toggle to switch between 5 neon-inspired color palettes.

✅ **Downloadable Resume**

Hosted PDF for recruiters to download instantly.

✅ **Verified Links**

GitHub & LinkedIn profiles with hover effects and accessibility labels.

✅ **Custom Background**

SVG circuit board overlay with smooth fade between light and dark mode.

✅ **Infrastructure as Code**

Terraform scripts manage:
- S3 bucket policies
- CloudFront distribution
- IAM roles
- Lambda deployment

✅ **CI/CD Pipeline**

GitHub Actions:
- Runs on `push` to `main`
- Syncs files to S3
- Invalidates CloudFront cache for near-instant updates

✅ **Security Headers**

Enforced Content Security Policy (CSP), HSTS, and other best practices.

---

## 🏗️ **Infrastructure Overview**

This project uses the following AWS resources:

- **S3 Bucket:** Hosts the static site
- **CloudFront Distribution:** Serves content securely over HTTPS
- **Lambda Function:** Counts visits and returns totals
- **API Gateway:** Public endpoint to trigger Lambda
- **DynamoDB Table:** Stores visitor counts
- **IAM Roles:** Securely grant least-privilege access
- **SES:** Planned for download notifications

---

## 🚀 **Deploy**

**All infrastructure is deployed via Terraform.**
Updates are pushed automatically via GitHub Actions.

---

## 📄 **Live Demo**

[🔗 Visit the live site](https://resume.whoisreggiesanchez.com)

---

## 💡 **Purpose**

This project demonstrates end-to-end cloud engineering skills, infrastructure as code, and modern web development.

---

## 🏆 **Next Steps**

- SNS/SQS email notifications
- Publish Terraform modules
- Enhance performance and accessibility further

---

