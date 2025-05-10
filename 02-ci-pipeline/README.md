# Task 2 - Azure DevOps CI Pipeline for .NET Application

This repository demonstrates a complete CI pipeline setup using Azure DevOps for a sample `.NET` application (`HelloWorldApi`). The pipeline includes build, test, and artifact publishing stages.

---

## 📁 Files Included

- `azure-pipelines.yml` – Azure DevOps pipeline definition
- `build-logs.zip` – Downloaded build logs from Azure DevOps
- `test-results` – Test execution report screenshot
![Image](https://github.com/user-attachments/assets/35441b7e-6b0c-41a8-ae9a-221880af6836)

🧪 Test Summary

| Metric          | Value     |
|-----------------|-----------|
| Total Tests     | 1         |
| Passed          | 1         |
| Failed          | 0         |
| Pass Percentage | 100%      |
| Test Duration   | ~2m 29s   |


---

## ⚙️ Pipeline Features

### ✅ Trigger
- Automatically runs on commits to the `main` branch.

### ✅ Stages
1. **Build Stage**  
   - Restores and publishes the .NET solution using `dotnet publish`.

2. **Test Stage**  
   - Executes unit tests using `dotnet test` 
   
3. **Publish Stage**  
   - Publishes compiled artifacts to the Azure DevOps artifact container.

---
