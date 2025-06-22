# 📺 VideoSharingCLD

A scalable *Video Sharing Web App* built with *React* and hosted on *AWS Cloud*. Users can upload, view, and share videos seamlessly. The app is designed to demonstrate cloud-native architecture using modern front-end frameworks.


## 🛠 Tech Stack

- *Frontend:* React (with Hooks & Context API)
- *Cloud Hosting:* AWS S3, CloudFront
- *Backend/Storage (Optional):* AWS Lambda, API Gateway, DynamoDB, S3
- *CI/CD:* GitHub Actions (optional)
---

## 📁 Features

- 🎥 Upload and stream video content
- 🔗 Shareable video links
- 📱 Responsive design (Mobile & Desktop)
- 🌐 CDN-backed performance with AWS CloudFront
- ☁ Serverless and cost-efficient architecture

---

## 🏗 Architecture Overview

```text
                +---------------------+
                |   React Frontend    |
                | (Hosted on S3/CF)   |
                +---------+-----------+
                          |
                    HTTPS Request
                          ↓
          +-------------------------------+
          |     AWS API Gateway (Optional)|
          +-------------------------------+
                          ↓
             +-------------------------+
             |   AWS Lambda (Optional) |
             +-------------------------+
                          ↓
               +-------------------+
               |  AWS S3 (Videos)  |
               +-------------------+
