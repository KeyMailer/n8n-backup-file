# n8n Workflow Backup Repository

## Overview

This repository contains backups of n8n workflows organized in a structured folder hierarchy for version control and maintenance.

Each folder represents a workflow or a group of related workflows. Workflow files are stored in JSON format and can be imported directly into n8n when needed.

## Structure Guidelines

- Each top-level folder represents a workflow project or automation group.
- Subfolders may be created when a workflow contains multiple related processes.
- Each JSON file represents an individual n8n workflow.
- Related workflows should be grouped together to improve organization and maintainability.

## Naming Convention

### Folder Naming

```bash
01 - Workflow Name
02 - Workflow Name
03 - Workflow Name
```

Where:

- `01`, `02`, `03`, etc. = Workflow version or sequence number.
- `Workflow Name` = Descriptive name of the automation.

## Pushing Changes to Git

After exporting or updating a workflow JSON file, follow these steps to push it to the repository.

### 1. Check what changed

```bash
git status
```

### 2. Stage the changes

```bash
git add .
```

To stage a single folder or file instead:

```bash
git add "01 - Workflow Name/"
```

### 3. Commit the changes

```bash
git commit -m "Update 01 - Workflow Name: describe what changed"
```

### 4. Push to the remote repository

```bash
git push origin main
```

> Replace `main` with your branch name if it's different (e.g. `master`).

### Quick Reference (all in one)

```bash
git add .
git commit -m "Backup n8n workflows - YYYY-MM-DD"
git push origin main
```

### Commit Message Examples

```bash
git commit -m "Add 04 - Lead Notification workflow"
git commit -m "Update 02 - Invoice Automation: fix webhook node"
git commit -m "Backup all workflows - 2026-10-07"
```

### Tips

- Run `git pull origin main` before pushing to avoid conflicts if others also update the repo.
- Use clear commit messages so changes are easy to trace later.
- Make sure no credentials or API keys are in the exported JSON before pushing.
