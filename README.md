# DevOps Engineer Challenge (Azure)

## Objective:
Set up a basic CI/CD pipeline for a simple web application, deploy it to Azure, and implement essential monitoring, security, and scalability, all within the constraints of the Azure free tier.

## Tasks

### Infrastructure Setup
1. **Provision Azure Infrastructure**:
   - Use Azure Resource Manager (ARM) templates, Bicep, or Terraform to provision:
     - An Azure App Service to host a simple web application (e.g., Node.js or .NET Core) using the free tier.
     - An Azure SQL Database or Azure Cosmos DB as the backend, utilizing the free tier options. 
   - Ensure the web app is accessible via a public URL.

### CI/CD Pipeline
2. **Set Up Basic CI/CD Pipeline using GitHub Actions**:
   - Trigger the pipeline on every `git push`.
   - Run unit tests.
   - Build and package the application.
   - Deploy the application to the Azure App Service.

### Monitoring
3. **Implement Basic Monitoring**:
   - Use Azure Monitor to set up alerts for CPU usage and HTTP error rates.
   - Ensure logs are collected using Azure Log Analytics, keeping within the 5 GB free tier limit.

### Security
4. **Secure the Setup**:
   - Use Azure Key Vault to securely manage and access database credentials.
   - Set up SSL/TLS for the web application using the free App Service Managed Certificate.

### Scalability
5. **Manual Scalability Configuration**:
   - Describe how to scale the Azure App Service manually using the Azure portal.
   - Provide a theoretical explanation of auto-scaling, even though it’s not available in the free tier.

### Documentation
6. **Provide Documentation**:
   - Include step-by-step instructions for setting up the infrastructure and CI/CD pipeline.
   - Briefly explain the monitoring and logging setup.
   - Document the security measures.

### Bonus (Optional)
- Implement a rollback mechanism for failed deployments.
- Describe a disaster recovery plan for the web application.

## Submission Guidelines

### 1. Project Repository
**GitHub Repository Link**: 
Provide a link to the public GitHub repository containing all the code, configuration files, and scripts used in the challenge.
The repository should include the following:
- Source Code: The web application code (e.g., Node.js, .NET Core) used for the deployment.
- CI/CD Pipeline Configuration: GitHub Actions workflows (.github/workflows/ directory) with detailed YAML files.
- Infrastructure as Code (IaC) Files: ARM templates, Bicep files, or Terraform scripts used for provisioning Azure resources.
- Scripts and Commands: Any scripts or commands used for setup, deployment, or testing.

### 2. Documentation
**README.md**:
- **Overview**: Provide a brief description of the project, including the purpose of the web application and the CI/CD pipeline.
- **Setup Instructions**: Step-by-step instructions on how to:
   - Clone the repository.
   - Set up the Azure infrastructure.
   - Configure the CI/CD pipeline.
   - Deploy the application.
- **Monitoring & Logging**: Explanation of how monitoring and logging were implemented using Azure Monitor and Log Analytics, including what metrics and alerts are set up.
- **Security Measures**: Detailed description of the security configurations, including the use of Azure Key Vault and SSL/TLS setup.
- **Scalability Considerations**: Explanation of manual scaling configuration and theoretical discussion on auto-scaling.
- **Testing Instructions**: Guidance on how to test the setup, including any simulated traffic tests for scalability.
- **Rollback Mechanism**: (Optional) Describe the rollback mechanism if implemented.
- **Disaster Recovery Plan**: (Optional) A brief description of a disaster recovery strategy.

### 3. Video Demonstration (Optional)
A short video (5-10 minutes) demonstrating:
- The CI/CD pipeline in action (e.g., triggering a deployment with a git push).
- Monitoring alerts and logging in Azure.
- Manual scaling of the Azure App Service.
The video should be hosted on a platform like YouTube (unlisted) or shared as a downloadable file.

### 4. Testing & Verification
Ensure that the entire setup works from end to end. The CI/CD pipeline should successfully deploy the application to Azure, and the monitoring, security, and scalability features should be demonstrable.

### 5. Submission Format
- All files and documentation should be committed and pushed to the GitHub repository.
- Provide a summary in the repository's README.md of any known issues or limitations.
- Email the submission details (GitHub repository link and optional video link) to the provided contact address.

