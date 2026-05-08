# Static Website Hosting with S3 and CloudFront

## Overview
This project demonstrates how to deploy a static website using AWS services. The website is hosted on Amazon S3 and distributed globally using CloudFront as a Content Delivery Network (CDN).

---

## Architecture
User → CloudFront → S3 (static website)

---

## Services Used
- Amazon S3 (static website hosting)
- CloudFront (content delivery and caching)

---

## Implementation Steps

### 1. Website Creation
- Created a simple HTML page (`index.html`)

### 2. S3 Bucket Setup
- Created an S3 bucket
- Disabled block public access
- Enabled static website hosting
- Uploaded website files

### 3. Bucket Policy
- Configured a policy to allow public read access

### 4. CloudFront Distribution
- Created a CloudFront distribution
- Configured S3 as the origin
- Set default root object to `index.html`
- Enabled HTTP to HTTPS redirection

---

## Features
- Static website hosting
- Global content delivery via CDN
- Reduced latency through caching
- Secure access using HTTPS

---

## Screenshots

### S3 Static Hosting
![S3](screenshots/s3-static-hosting.png)

### Bucket Policy
![Policy](screenshots/s3-policy.png)

### Website via S3
![S3 Website](screenshots/s3-website.png)

### CloudFront Distribution
![CloudFront](screenshots/cloudfront-created.png)

### Website via CloudFront
![Website](screenshots/cloudfront-website.png)

---

## Key Learnings
- Difference between S3 static hosting and traditional web servers
- Basics of CDN and caching
- How CloudFront improves performance and availability
- Managing public access securely in AWS

---

## Author
Jelena
