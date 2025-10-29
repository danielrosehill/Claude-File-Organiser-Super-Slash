# Filesystem Cleaner Agent - Super Slash Command

[![Claude Code](https://img.shields.io/badge/Claude%20Code-Project-8A2BE2?style=for-the-badge&logo=anthropic)](https://github.com/anthropics/claude-code)
[![Claude Code Projects Index](https://img.shields.io/badge/Claude%20Code-Projects%20Index-blue?style=flat-square)](https://github.com/danielrosehill/Claude-Code-Repos-Index)
[![Master Index](https://img.shields.io/badge/GitHub-Master%20Index-green?style=flat-square)](https://github.com/danielrosehill/Github-Master-Index)

A comprehensive, deterministic slash command for Claude Code that transforms chaotic file and folder structures into well-organized, maintainable systems across any operating system.

## Overview

This repository contains a sophisticated AI agent prompt designed as a slash command for Claude Code CLI. The agent specializes in filesystem organization with minimal user intervention, applying intelligent rules and pattern recognition to create clean, consistent directory structures.

## Key Features

### Core Capabilities

- **Machine-Readable Naming**: Enforces `snake_case` conventions and removes special characters
- **Automatic Typo Remediation**: Fixes obvious typos without consultation
- **Smart Timestamp Integration**: Applies consistent date formats (DD-MM-YYYY, YYMMDD)
- **Optimal Recursion Depth**: Creates balanced folder hierarchies (avoiding both flat chaos and excessive nesting)
- **Orphan File Management**: Identifies and relocates files not contained in any folder
- **Intelligent Disambiguation**: Resolves naming conflicts with descriptive suffixes
- **Pattern Recognition**: Automatically detects and applies domain-specific organizational strategies

### Technical Features

- **Vision-Based Analysis**: Uses image analysis to intelligently rename photos and videos
- **Duplicate Detection**: Identifies and consolidates duplicate files
- **Cross-Platform Compatibility**: Ensures naming works across Windows, Linux, and macOS
- **Archive Management**: Organizes outdated files with year/month hierarchies
- **Metadata Preservation**: Maintains file extensions and important attributes

### Personality

The agent features a unique, theatrical communication style:
- **Beginning**: Inspirational announcements about the "monumental quest" ahead
- **Completion**: Celebratory victory messages emphasizing the transformative impact

## Domain-Specific Patterns

The agent recognizes and applies specialized rules for:

### Pattern A: Image Galleries
- Content-based renaming using vision analysis
- Resolution-based organization (thumbnails vs full resolution)
- Semantic grouping (portraits, landscapes, etc.)

### Pattern B: Video Collections
- Resolution hierarchy (4K → 1080p → 720p)
- Aspect ratio separation (portrait/landscape)
- Content type classification

### Pattern C: Mixed Media Folders
- Media type segregation (images, videos, documents, audio)
- Technical attribute sorting (resolution → aspect ratio)

### Pattern D: Code Repositories
- Separation of concerns (code vs non-code)
- Standard directory structures (`src/`, `assets/`, `docs/`, `tests/`)

### Pattern E: Document Collections
- Type and status organization (active, drafts, archive)
- Year/month hierarchies for invoices and time-sensitive docs

### Pattern F: Download Folders
- File type grouping
- Installer identification and versioning
- Archive consolidation

## Organizational Principles

### Naming Conventions
- Default format: `snake_case`
- Avoid special characters (except `_` and `-`)
- Lowercase preferred (capitals only when critical for readability)
- Concise but descriptive (<50 characters)
- No redundancy with parent folder names

### Date Formats
- **General naming**: `DD-MM-YYYY` or `YYMMDD`
- **File prefixes**: `YYMMDD` for chronological sorting
- **Hierarchical folders**: `year/month/day/` structure

### Hierarchy Guidelines
- **1-3 items**: No subfolder needed (unless semantically distinct)
- **4-9 items**: Evaluate natural groupings
- **10+ items**: Subfolders likely beneficial
- **Maximum depth**: Rarely exceed 5 levels

## Decision Framework

### Autonomous Actions (No Consultation Required)
- Fixing obvious typos
- Applying machine-readable naming
- Moving files to clearly appropriate folders
- Creating obvious organizational structures
- Removing duplicate temp/system files

### User Consultation Required
- Deleting files (except obvious temp files)
- Major restructuring (>30% of hierarchy)
- Ambiguous file purposes
- Multiple valid organization strategies

### Uncertainty Handling
When unsure, the agent creates a `/bin` folder and moves questionable items there for user review.

## Execution Workflow

1. **Analysis**: Scan structure, identify patterns, detect issues
2. **Planning**: Determine strategy, plan structure and renaming
3. **Execution**: Create folders, fix typos, move files, resolve conflicts
4. **Verification**: Confirm completeness, validate consistency, document changes

## Version History

This repository maintains multiple versions of the slash command:

- **`prompt.md`**: Current version with comprehensive features
- **`archive/v1/`**: Earlier iteration
- **`archive/v2/`**: Second iteration
- **`archive/mine/`**: Original user-created versions

### Development Philosophy

**Rule**: Always iterate by creating new versions. Never overwrite existing versions.

## Usage

1. Add the slash command to your Claude Code CLI configuration
2. Navigate to the directory you want to organize
3. Execute the slash command
4. The agent will analyze, plan, and execute the organization
5. Review any items placed in `/bin` for uncertain cases

## Technical Requirements

- Claude Code CLI
- File system access permissions
- (Optional) Vision API access for image/video content analysis

## Project Structure

```
Claude-File-Organiser-Super-Slash/
├── README.md                           # This file
├── CLAUDE.md                          # Project instructions for AI
├── prompt.md                          # Current slash command prompt
├── archive/                           # Previous versions
│   ├── v1/
│   │   └── prompt.md
│   ├── v2/
│   └── mine/
│       └── my-v1.md
└── breakdown/                         # Analysis documentation
    └── full.md
```

## Best Practices

### File Extensions
- Always preserve original extensions
- Use lowercase (`.jpg` not `.JPG`)
- Avoid multiple extensions unless necessary
- Remove redundant extensions

### Versioning
- Use semantic versioning: `v1`, `v2`, `v1.1`
- Place before extension: `proposal_v2.pdf`
- Prefer descriptive states: `draft`, `review`, `final`

### Special Directories
- `src/` - Source code
- `assets/` - Static resources
- `docs/` - Documentation
- `archive/` - Outdated but useful files
- `temp/` - Temporary working files
- `bin/` - Uncertain items for review

## Cross-Platform Compatibility

The agent ensures compatibility by:
- Avoiding Windows reserved names (`CON`, `PRN`, `AUX`, etc.)
- No trailing spaces or periods
- No leading hyphens
- Path length <260 characters (Windows MAX_PATH)

## Contributing

When contributing new versions:
1. Create a new version directory
2. Never overwrite existing versions
3. Document changes and improvements
4. Follow the established organizational principles

## License

[Add license information]

## Author

Daniel Rosehill
- Website: [danielrosehill.com](https://danielrosehill.com)
- Business: [DSR Holdings](https://dsrholdings.cloud)
- Email: public@danielrosehill.com

## Acknowledgments

Built for use with Claude Code CLI by Anthropic.

---

*"Order is the shape upon which beauty depends."*
