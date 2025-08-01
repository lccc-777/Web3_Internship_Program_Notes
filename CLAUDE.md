# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Web3 Internship Program documentation repository (Web3残酷共学) that serves as a personal learning tracker and task management system. It's deployed as a GitHub Pages site where users can track their progress through various Web3 learning tasks and submit proof of completion.

## Repository Structure

```
├── docs/                           # GitHub Pages source directory
│   ├── _config.yml                 # Jekyll configuration for GitHub Pages
│   ├── todo.md                     # Main task tracking page (deployed as website)
│   └── StudyNotes/                 # Daily learning notes
│       ├── day0.md to day30.md     # 31 daily study note templates
├── ProofForChallenges/             # Storage for task completion proofs
├── Resume/                         # Resume templates
├── Tasks/                          # Additional task directories
└── readme.md                       # Project setup instructions
```

## Key Architecture Concepts

### GitHub Pages Deployment
- The `docs/` folder is configured as the GitHub Pages source
- Jekyll processes the markdown files with front matter variables
- The site is accessible at `https://<username>.github.io/Web3_Internship_Program_Notes/todo`

### Task Tracking System
- `docs/todo.md` contains Jekyll front matter with variables:
  - `githubID`: User's GitHub username for form submissions
  - `path_proofForChallenges`: Path to proof storage
  - `timeStamp`: Unix timestamp for tracking
- Tasks link to external Tally forms with URL parameters for automatic submission
- Task completion uses checkboxes in markdown format

### Daily Study Notes Template
- Each `dayX.md` file follows a consistent structure:
  - Date header in Chinese format (YYYY年MM月DD日)
  - Structured sections: 学习目标, 学习内容, 学习笔记, 问题与思考, 总结
  - Footer with formatted date

## Common Operations

### Setting Up for New Users
1. Fork the repository
2. Change `githubID` variable in `docs/todo.md` front matter
3. Enable GitHub Pages in repository settings, source: `/docs`
4. Wait for deployment (a few minutes)
5. Access at `https://<username>.github.io/Web3_Internship_Program_Notes/todo`

### Modifying Task Progress
- Edit checkboxes in `docs/todo.md` to mark tasks as complete: `- [x]`
- Changes will be reflected on the live site after GitHub Pages rebuilds

### Adding New Daily Notes
- Use the template structure found in existing `dayX.md` files
- Maintain consistent Chinese date formatting
- Include all standard sections for learning organization

### Managing Proof Files
- Store task completion proofs in `ProofForChallenges/` directory
- Reference these files in task submissions or link them in todo.md

## Jekyll Configuration Notes

- `_config.yml` is configured to hide the site title link (`title: false`)
- Downloads are disabled (`show_downloads: false`) 
- The site uses GitHub Pages' default theme with minimal customization

## Important File Relationships

- `docs/todo.md` front matter variables are used in Tally form submission URLs
- The `{{page.githubID}}` liquid template variable gets replaced with the actual GitHub username
- Task submission links are pre-configured with scoring and task descriptions
- Daily notes are independent but follow the same template for consistency