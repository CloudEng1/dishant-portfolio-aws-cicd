# Dishant Bariya — Portfolio Website

A professional portfolio website created for **Dishant Bariya**, a B.Tech Computer Science graduate and creative visual content creator.

## 🌐 Deployment

The website is currently deployed using:

- Amazon S3
- Amazon CloudFront

Current flow:

```text
Local Website → Amazon S3 → Amazon CloudFront → Live Website
```

CloudFront is configured with HTTPS and `index.html` as the default root object.

## 🛠️ Technologies

- HTML5
- CSS3
- JavaScript
- Bootstrap
- Bootstrap Icons
- Git
- GitHub
- Amazon S3
- Amazon CloudFront

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

## 📦 GitHub

The project source code is maintained in Git and pushed to the `main` branch on GitHub.

## 🚀 CI/CD — Next Phase

The next step is to implement automated deployment using GitHub Actions.

Planned flow:

```text
Code Change
    ↓
GitHub
    ↓
GitHub Actions
    ↓
AWS S3
    ↓
CloudFront Cache Invalidation
    ↓
Updated Live Website
```

**Note:** CI/CD is the next phase of the project and is not being claimed as completed yet.

## 🎨 Original Template

The website was started from the **FolioOne Bootstrap portfolio template** by BootstrapMade.

Template:
https://bootstrapmade.com/folioone-bootstrap-portfolio-websites-template/

The template has been customized for Dishant Bariya's portfolio, including the content, services, portfolio information, profile image, and website sections.

## 👤 About Dishant

Dishant Bariya is a B.Tech Computer Science graduate with a focus on video editing, photo editing, motion graphics, short-form content, and visual storytelling.

Tools include:

- Adobe Premiere Pro
- Adobe After Effects
- Adobe Photoshop
- Adobe Illustrator

---

## 📌 Project Status

**Completed:**
- Static portfolio website customized
- Website deployed to Amazon S3
- CloudFront distribution created
- HTTPS live deployment working
- Source code pushed to GitHub

**Next:**
- GitHub Actions CI/CD
- Secure AWS authentication using OIDC
- Automatic S3 deployment
- Automatic CloudFront cache invalidation
