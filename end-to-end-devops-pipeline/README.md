# End-to-End DevOps Pipeline (Azure DevOps + ACR + AKS)

**Combination of Multiple DevOps Tasks**

This is a **combination of multiple key DevOps tasks** that cover the entire pipeline, from code analysis to deployment:

### 1. **CI Pipeline Setup**: 
   - **Builds and tests** a sample **.NET** application in Azure DevOps.
   - **Unit tests** are run as part of the CI process, ensuring that the code quality is maintained.

### 2. **Dockerization & Push to ACR**:
   - **Dockerfile** is used to containerize the application, creating a Docker image.
   - The image is pushed to **Azure Container Registry (ACR)** (`rachana.azurecr.io`).

### 3. **Multi-Stage CD**:
   - This pipeline includes a **multi-stage deployment** process for multiple environments:
     - **Dev**: Automatic deployment.
     - **Staging**: Automatic deployment with environment-specific configuration.
     - **Prod**: Requires **manual approval** for deployment. Please find the screenshot of gating below:

### 4. **Kubernetes Deployment**:
   - **Deployment** and **Service** are defined in a `manifest.yaml` file, which includes **liveness** and **readiness probes** for container health monitoring.

Note: Due to some limitations with my free azure subscription, I was unable to create aks cluster. However, the 

### 5. **Code Quality & Security**:
   - **SonarQube** integration for static code analysis, ensuring code quality and detecting potential bugs or vulnerabilities.
   - **Trivy** integration to perform a **security scan** of the Docker image for any vulnerabilities, ensuring the images are secure before being deployed.

### 6. **Approval Gates for Production**:
   - Deployment to **Prod** requires a **gated approval** in Azure DevOps, ensuring that only validated code and images make it to the production environment.




