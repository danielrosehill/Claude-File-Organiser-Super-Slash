# Repo Purpose

The purpose of this repository is to version control and work on a single and very detailed slash command for organising filesystems. 

The slash command should be versatile enough to work across a wide variety of systems and deterministic enough that it sorts based upon clearly defined logic obviating the need for frequent user input or any at all. 

# Latest Version

prompt.md

# Updating Workflow

Before any guided update:

1. Copy prompt.md to archive and give it the latest iterative version number
2. Create the improved version as prompt.md
3. Add or append a markdown badge (shields.io) with the new version number
4. **Document changes in CHANGELOG.md**:
   - Add a new version section under `## [Unreleased]`
   - List all changes in the appropriate categories:
     - **Added**: New features or capabilities
     - **Changed**: Modifications to existing functionality
     - **Deprecated**: Soon-to-be removed features
     - **Removed**: Deleted features
     - **Fixed**: Bug fixes
     - **Security**: Security-related changes
   - Include the date in YYYY-MM-DD format
   - Move the changes from `[Unreleased]` to the new version section
   - Describe what was changed between versions clearly and specifically

## Rules

- Always iterate by creating new versions. Never overwrite.
- Always document changes in CHANGELOG.md with clear descriptions of what changed between versions.
- Be specific about what was added, modified, or removed in each version.