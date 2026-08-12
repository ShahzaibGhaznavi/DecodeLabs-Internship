# DecodeLabs Project 3 - CI/CD Pipeline

## Description

This project demonstrates an automated CI/CD pipeline using GitHub Actions to build, test, package, and deploy a simple HTML application to an AWS EC2 server.

## Objective

- Understand Continuous Integration and Continuous Deployment
- Automate build and test steps
- Trigger the pipeline using Git push
- Use GitHub Actions workflows
- Create and manage build artifacts
- Store sensitive credentials securely using GitHub Secrets
- Deploy application files automatically to an AWS EC2 server using SSH/SCP

## Application

This project contains a simple HTML application used to demonstrate the complete CI/CD workflow.

## CI/CD Flow

Git Push → GitHub Actions → Runner → Build → Test / Quality Gate → Artifact → Download Artifact → SSH/SCP → AWS EC2

## Deployment

After successful build and testing:

1. The application files are packaged as an artifact.
2. The artifact is uploaded by GitHub Actions.
3. The artifact is downloaded for deployment.
4. GitHub Actions uses GitHub Secrets for secure EC2 authentication.
5. The application files are transferred to the AWS EC2 server using SSH/SCP.

## Deployed Files

The following files are deployed to the EC2 server:

- `index.html`
- `README.md`

Deployment directory:

`~/decodelabs-project-3`

## Technologies

- Git
- GitHub
- GitHub Actions
- YAML
- Linux
- AWS EC2
- SSH/SCP
- GitHub Secrets
