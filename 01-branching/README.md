## Branching Strategy

Below is the Git Feature Branch Workflow with a structured release flow across environments. The main branches used are:

- **`main`** – Production-ready code. 
- **`staging`** – Pre-production validation. 
- **`qa`** – Internal testing (QA environment).
- **`develop`** – Active integration of all feature branches.
- **`feature/*`** – Task-specific branches for new features or fixes.

### Typical Workflow:

1. Start feature from `develop`:
   ```bash
   git checkout -b feature/task-1-branching develop

2. After feature completion, raise a PR to develop

3. After integration testing, merge develop to qa

3. Once QA passes, promote code from qa to staging

4. Finally, merge staging to main for production release


- feature/* → develop → qa → staging → main

### Git Branching and Workflow Demonstration

This pull request demonstrates a standard Git workflow as part of the DevOps assessment.

**Includes:**
- Created a feature branch: `feature/task-1-branching`
- Added sample file `hello.txt`
- Branching strategy is mentioned in first section of this file.
- Below screenshots for:
  - Pull request creation:
    
   ![Image](https://github.com/user-attachments/assets/5274fa13-ff84-4147-a31c-138b56dad098)

  - Code review comment:
    
   ![Image](https://github.com/user-attachments/assets/96ca8101-37f4-4a29-94cb-62b6cb9762d4)

  - Merge confirmation:
    
   ![Image](https://github.com/user-attachments/assets/1ecb53e6-9322-4d04-9db8-84a7fd5a1354)


