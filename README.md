# Scalable Static Website Deployment using AWS S3, Cloudflare & GitHub Actions

## Project Overview :

This project demonstrates how to deploy a **scalable static website** using **AWS S3**, automate deployment with **GitHub Actions**, and deliver the website globally through **Cloudflare CDN with HTTPS**.

The setup provides a **CI/CD pipeline** where every push to GitHub automatically updates the live website.


## Live Website :

https://portfolio-site.amarnathraki.workers.dev


## Technologies Used :

* AWS S3 – Static website hosting
* GitHub – Source code repository
* GitHub Actions – CI/CD automation
* Cloudflare – CDN and HTTPS
* HTML / CSS / JavaScript


## Architecture :

Developer
↓
GitHub Repository
↓
GitHub Actions CI/CD
↓
AWS S3 Static Hosting
↓
Cloudflare CDN + HTTPS
↓
End User


## Project Structure :

├── index.html
├── style.css
├── script.js
└── .github/workflows/deploy.yml


## CI/CD Workflow :

Whenever code is pushed to the **main branch**, the GitHub Actions pipeline automatically:

1. Checks out the repository.
2. Loads AWS credentials securely from GitHub Secrets.
3. Syncs website files to the S3 bucket.
4. Updates the live website.

Deployment command used:

aws s3 sync . s3://amarnath-static-website --delete


## Cloudflare Integration :

Cloudflare is used for:

* Global CDN caching
* HTTPS encryption
* Faster content delivery
* Security protection

The site is accessible through a Cloudflare Workers subdomain.


## Key Features :

* Automated CI/CD deployment
* Static website hosting on AWS
* Global CDN delivery
* Secure HTTPS access
* Simple and scalable architecture


## Deliverables :

* GitHub Actions CI/CD workflow
* AWS S3 static website hosting
* Cloudflare CDN integration
* Live deployed website


## Author :

Amarnath K

DevOps & Cloud Enthusiast

GitHub:
https://github.com/amar2220
