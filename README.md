# n8n Workflow Backup Repository

Overview

This repository contains backups of n8n workflows organized in a structured folder hierarchy for version control and maintenance.

Each folder represents a workflow or a group of related workflows. Workflow files are stored in JSON format and can be imported directly into n8n when needed.

Structure Guidelines

- Each top-level folder represents a workflow project or automation group.
- Subfolders may be created when a workflow contains multiple related processes.
- Each JSON file represents an individual n8n workflow.
- Related workflows should be grouped together to improve organization and maintainability.

## Naming Convention

Folder Naming

```bash
01 - Workflow Name
02 - Workflow Name
03 - Workflow Name
```

Where:

- 01, 02, 03, etc. = Workflow version or sequence number.
- Workflow Name = Descriptive name of the automation.
