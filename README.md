# zenwebapi11

My test app

## 🏗️ Setup Instructions

This repository contains deployment infrastructure and CI/CD pipelines for your .NET application. 

**⚠️ Next Steps:**
1. Add your .NET solution and project files to this repository
2. Remove the `SETUP-DOTNET-PROJECTS.md` file after reading the setup instructions  
3. Update this README with your application-specific information
4. Push your changes to trigger the CI/CD pipeline

## 📋 Configuration Summary

### Features

- **Cloud Provider**: GCP
- **Deployment Type**: Gke
- **Region**: asia-south1
- **GKE Cluster**: zenhotel-cluster
- **Namespace**: default

## Getting Started

1. Clone this repository
2. Add your .NET application code to this repository
3. Push to the `main` branch to trigger the deployment pipeline

## Deployment

### Application Deployment
Your application will be deployed to **Google Kubernetes Engine (GKE)** cluster:
- **Cluster**: zenhotel-cluster
- **Namespace**: default
- **Region**: asia-south1

## CI/CD Pipeline

The repository includes GitHub Actions workflows for:
2. **Application Deployment** (`deploy.yml`) - Runs on every push to main branch

## Prerequisites

Make sure the following GitHub secrets are configured in your repository:

- `GCP_PROJECT_ID`: Your Google Cloud Project ID
- `GCP_REGION`: Your Google Cloud Region
- `GCP_SA_KEY`: Base64 encoded service account key with necessary permissions

## Development

Add your .NET application code and push to trigger the deployment pipeline. The template supports both:

- **ASP.NET Web API** (Backend)
- **ASP.NET Web App** (Frontend)

The Dockerfile and deployment scripts are generic and will work with both application types.
