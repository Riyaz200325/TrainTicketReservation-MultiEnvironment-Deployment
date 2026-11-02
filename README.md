
# Train Ticket Reservation – Multi-Environment CI/CD Deployment

## 📌 Project Overview

This project demonstrates a Continuous Integration and Continuous Deployment (CI/CD) pipeline for a Train Ticket Reservation web application using GitHub Actions, Maven, Apache Tomcat, and AWS EC2.

The pipeline automates the application build and deployment process across multiple environments through a manual GitHub Actions workflow.

## 🛠️ Technologies Used

- AWS EC2
- Ubuntu
- Git & GitHub
- GitHub Actions
- Apache Maven
- Apache Tomcat 9
- Java
- CI/CD

## 🏗️ Architecture

Developer
   |
   v
GitHub Repository
   |
   v
GitHub Actions
   |
   v
Maven Build
   |
   v
WAR Artifact
   |
   v
AWS EC2 (Ubuntu)
   |
   v
Apache Tomcat
   |
   v
Train Ticket Reservation Application

## ⚙️ CI/CD Workflow

1. The application source code is stored in GitHub.
2. GitHub Actions workflow is triggered manually.
3. Maven builds the application and packages it into a WAR file.
4. The generated WAR artifact is transferred to the deployment job.
5. GitHub Actions deploys the WAR file to Apache Tomcat on AWS EC2.
6. The deployed application is verified using its application URL.

## 🌍 Deployment Environments

The workflow supports the following environments:

- DEV
- TEST
- PRE-PROD
- PROD

The target environment is selected when manually triggering the GitHub Actions workflow.

## 🚀 How to Run the Pipeline

1. Open the **Actions** tab in this repository.
2. Select the CI/CD workflow.
3. Click **Run workflow**.
4. Select the desired deployment environment.
5. Click **Run workflow** to start the pipeline.
6. Monitor the build and deployment jobs.
7. Verify the deployed application.

## 🔐 Security

Deployment credentials are stored securely using GitHub Actions Secrets.

Secrets used by the workflow:

- `TOMCAT_URL`
- `TOMCAT_USERNAME`
- `TOMCAT_PASSWORD`

Sensitive credentials are not included in the source code.

## 🎯 Project Objectives

- Automate application build and deployment.
- Implement a CI/CD pipeline using GitHub Actions.
- Deploy a Java web application to Apache Tomcat.
- Demonstrate environment-based deployment.
- Improve deployment consistency and reduce manual effort.

## 👨‍💻 Author

**Riyaz Shaik**

GitHub: [Riyaz200325](https://github.com/Riyaz200325)

## 📸 Project Screenshots

### Application Login Page
![Application Login](screenshots/application-login.png)

### Tomcat Manager
![Tomcat Manager](screenshots/tomcat-manager.png)

### Application Deployed on Tomcat
![Application Deployed](screenshots/application-deployed.png)

### GitHub Actions CI/CD Pipeline
![GitHub Actions Success](screenshots/github-actions-success.png)
