# Dishant Bariya — Portfolio Website

A professional portfolio website created for **Dishant Bariya**, a B.Tech Computer Science graduate and creative visual content creator.

The website has been customized to showcase work and services related to video editing, motion graphics, short-form content, photo editing, visual storytelling, and social media content.

## 🌐 Live Website

[Visit Live Website](https://d2891h3l9ase71.cloudfront.net)

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript
- Bootstrap
- Bootstrap Icons
- Git
- GitHub
- Amazon S3
- Amazon CloudFront
- GitHub Actions
- AWS IAM
- AWS OIDC

## ✨ Website Sections

- Home
- About
- Services
- Portfolio
- Contact
- Resume

## 🎨 Creative Services

The portfolio focuses on:

- Video Editing
- Motion Graphics
- Short-Form Content
- Photo Editing
- Visual Storytelling
- Social Media Content

Tools used include:

- Adobe Premiere Pro
- Adobe After Effects
- Adobe Photoshop
- Adobe Illustrator

## ☁️ AWS Deployment

The static website is hosted using **Amazon S3** and delivered through **Amazon CloudFront**.

Deployment architecture:

```text
Static Website
      ↓
Amazon S3
      ↓
Amazon CloudFront
      ↓
Live HTTPS Website
```

The CloudFront distribution is configured with `index.html` as the default root object and HTTPS redirection.

## 🚀 CI/CD Pipeline

A GitHub Actions CI/CD pipeline has been implemented for automated website deployment.

Pipeline architecture:

```text
Developer
   ↓
Git commit
   ↓
GitHub repository (main)
   ↓
GitHub Actions
   ↓
AWS OIDC Authentication
   ↓
IAM Deployment Role
   ↓
Amazon S3 sync
   ↓
CloudFront cache invalidation
   ↓
Updated live website
```

### 🔐 Secure AWS Authentication

The GitHub Actions workflow uses **OpenID Connect (OIDC)** to authenticate with AWS.

No long-lived AWS access keys or secret access keys are stored in the GitHub repository for deployment.

The IAM deployment role is restricted to the project's GitHub repository and `main` branch.

### 📦 Automated Deployment

On every push to the `main` branch, GitHub Actions:

1. Checks out the repository.
2. Authenticates to AWS using OIDC.
3. Verifies the AWS identity.
4. Synchronizes website files to Amazon S3.
5. Creates a CloudFront cache invalidation.

This automates the path from a GitHub code change to the live AWS deployment.

## ✅ CI/CD Validation

The pipeline was validated with an actual website content change.

A text capitalization change was committed and pushed to the `main` branch. The GitHub Actions workflow completed successfully, and the updated text was visible on the live CloudFront website.

```text
GitHub push
     ↓
GitHub Actions ✅
     ↓
AWS OIDC authentication ✅
     ↓
S3 deployment ✅
     ↓
CloudFront invalidation ✅
     ↓
Updated live website ✅
```

This confirms the deployment workflow is working end-to-end.

## 📁 Repository

[GitHub Repository](https://github.com/CloudEng1/dishant-portfolio-aws-cicd)

## 🎨 Original Template

The website was started from the **FolioOne Bootstrap portfolio template** by BootstrapMade.

Template:
https://bootstrapmade.com/folioone-bootstrap-portfolio-websites-template/

The template has been customized for Dishant Bariya, including the content, services, portfolio information, profile image, and website sections.

## 📌 Project Status

**Completed**

- Static portfolio website customized
- Website deployed to Amazon S3
- CloudFront distribution configured
- HTTPS live deployment working
- GitHub repository created and populated
- GitHub Actions CI/CD implemented
- AWS OIDC authentication configured
- IAM deployment role configured with deployment permissions
- Automated S3 deployment implemented
- Automated CloudFront cache invalidation implemented
- End-to-end deployment tested successfully

## 👤 About Dishant

Dishant Bariya is a B.Tech Computer Science graduate and creative visual content creator focused on video editing, photo editing, motion graphics, short-form content, and visual storytelling.
