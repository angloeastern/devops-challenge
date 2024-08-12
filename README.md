# DevOps Engineer Challenge (Azure)

## Objective:
Set up a complete CI/CD pipeline for a simple web application, deploy it to Azure, implement monitoring, and ensure scalability and security.

## Tasks

### Infrastructure Setup
1. **Provision Infrastructure**:
   - Use Azure Resource Manager (ARM) templates, Bicep, or Terraform to provision the following:
     - An Azure Virtual Network (VNet) with appropriate subnets.
     - An Azure Application Gateway (or Azure Load Balancer) to route traffic to the web application.
     - Two Azure App Services running a simple web application (e.g., Node.js or .NET Core).
     - An Azure SQL Database or Azure Cosmos DB as the backend database.

### CI/CD Pipeline
2. **Set Up CI/CD Pipeline**:
   - Use GitHub Actions to set up a CI/CD pipeline with the following features:
     - Automatically trigger on a git push.
     - Run unit tests.
     - Build and package the application.
     - Deploy the application to the Azure App Service.
     - Perform a blue-green or canary deployment.

### Monitoring & Logging
3. **Implement Monitoring and Logging**:
   - Use Azure Monitor for monitoring:
     - Set up basic alerts for CPU usage, memory usage, and HTTP error rates using Azure Monitor alerts.
   - Implement centralized logging using Azure Log Analytics:
     - Ensure logs from all instances are aggregated in one place.

### Security
4. **Secure Azure Infrastructure**:
   - Set up Network Security Groups (NSGs) to restrict access to the VMs and database.
   - Implement Azure Role-Based Access Control (RBAC) to ensure least privilege access.
   - Set up SSL/TLS for the web application using Azure Key Vault to manage certificates.
   - Ensure sensitive information, such as database credentials, is managed securely using Azure Key Vault.

### Scalability
5. **Ensure Scalability**:
   - Configure Azure App Service Scale Sets to automatically scale the web application instances based on CPU or memory usage.
   - Ensure the Azure Application Gateway can handle increasing traffic and distribute it evenly across instances.
   - Test the scalability by simulating traffic and showing that the infrastructure scales up/down automatically.

## Documentation
6. **Provide Documentation**:
   - Include:
     - Step-by-step instructions on how to set up the infrastructure and CI/CD pipeline.
     - Explanation of the monitoring and logging setup using Azure services.
     - Security measures implemented.
     - How to trigger deployments and rollback in case of failures.

## Bonus (Optional)
- Implement a rollback mechanism in the CI/CD pipeline for failed deployments.
- Set up a disaster recovery plan.

## Submission Guidelines
1. Provide a Git repository with:
   - All ARM templates/Bicep files, CI/CD pipeline scripts, and application code.
2. Include a `README.md` file with:
   - Instructions on how to set up, deploy, and test the application on Azure.
3. (Optional) Record a short video demonstrating the setup and how everything works together.
4. Send the link to the Git repository and any other relevant files by the deadline.
