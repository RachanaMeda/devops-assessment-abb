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
  - Pull request creation

  - Code review comment

  - Merge confirmation


