# DVOP320 Personal Website

Personal portfolio website showcasing cloud and DevOps projects.

## 🌐 Live Demo

**GitHub Pages**: https://ruskoloma.github.io/DVOP320-Personal-Website/

## 🚀 Purpose

This repository contains a responsive portfolio website built as part of DVOP320 course requirements. It features:
- Professional landing page with bio and skills
- Three project showcases with detailed descriptions
- Clean, modern UI with gradient design system
- Fully responsive layout

## 🔄 Continuous Deployment with GitHub Actions

This repository uses GitHub Actions for automated deployment to GitHub Pages. Every push to the `main` branch automatically triggers the deployment workflow.

### Workflow Overview

The deployment pipeline is defined in `.github/workflows/deploy.yml` and includes the following steps:

1. **Checkout** - Clones the repository code
2. **Setup Pages** - Configures the GitHub Pages environment
3. **Upload Artifact** - Packages the website files for deployment
4. **Deploy to GitHub Pages** - Deploys the site to the live URL

### How to Trigger Deployment

#### Automatic Deployment
The workflow runs automatically when you push changes to the `main` branch:
```bash
git add .
git commit -m "Your commit message"
git push origin main
```

#### Manual Deployment
You can also trigger the workflow manually from the GitHub Actions tab:
1. Go to your repository on GitHub
2. Click on the **Actions** tab
3. Select **Deploy static content to Pages**
4. Click **Run workflow** > **Run workflow**

### Configuration Details

- **Workflow file**: `.github/workflows/deploy.yml`
- **Trigger**: Push to `main` branch + manual trigger (`workflow_dispatch`)
- **Permissions**: contents: read, pages: write, id-token: write
- **Concurrency**: Single deployment at a time to prevent conflicts

## 📋 Git Setup Workflow

### 1. Initialize Repository
```bash
git init
git config user.name "Ruslan Kolomiyets"
git config user.email "moltbot@ruslan.one"
```

### 2. Add & Commit Files
```bash
git add .
git commit -m "Initial commit of portfolio website"
```

### 3. Link to GitHub & Push
```bash
git remote add origin git@github.com:ruskoloma/DVOP320-Personal-Website.git
git branch -M main
git push -u origin main
```

## 🛠️ Technologies Used

- **HTML5** - Semantic structure
- **CSS3** - Custom properties, flexbox, gradients
- **JavaScript** - Intersection Observer for scroll animations
- **Google Fonts** - Inter typeface
- **GitHub Actions** - CI/CD for automated deployment

## 📁 File Structure

```
.
├── .github/
│   └── workflows/
│       └── deploy.yml    # GitHub Actions workflow
├── index.html            # Main landing page
├── project1.html         # Smart Home Automation project
├── project2.html         # Cloud Migration project
├── project3.html         # CI/CD Pipeline project
└── README.md             # This file
```

## 🎯 Assessment Requirements

- ✅ Repository correctly initialized and pushed to GitHub
- ✅ Clean, well-organized HTML/CSS code
- ✅ README documentation with workflow explanation
- ✅ Meaningful commit messages
- ✅ GitHub Pages deployment configured via GitHub Actions

## 🤝 Author

**Ruslan Kolomiyets**  
Cloud / DevOps Engineer  
DVOP320 - Winter 2026

---

*Repository URL*: https://github.com/ruskoloma/DVOP320-Personal-Website
