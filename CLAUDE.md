# CLAUDE.md

This file provides guidance for AI assistants working with this repository.

## Repository Overview

**hello-world** is a personal learning repository created by M. Sekido (GitHub: sekstore) in November 2020 to practice Git and GitHub fundamentals. It is not a software project — it contains no source code or build system. Its purpose is documentation and experimentation with Git workflows.

## Repository Structure

```
hello-world/
├── README.md                  # Repository introduction (English)
├── text_ver1.0                # Sample text file used in early Git exercises
├── How_to_Use_Git+GitHub.txt  # Step-by-step Git/GitHub reference guide (Japanese)
└── CLAUDE.md                  # This file
```

### File Descriptions

- **README.md**: Brief introduction written in English. States this is the owner's first GitHub repository, with a note added by M. Sekido.
- **text_ver1.0**: A short plain-text file used as a versioned artifact during early Git commit practice. Content: "This is the first Edit. Added 1. to 10. Last Line. Fin."
- **How_to_Use_Git+GitHub.txt**: A personal Git reference guide written in Japanese. Covers: account config, cloning, branch creation/checkout, editing files, staging (`git add`), committing, viewing logs, merging, and pushing to remote.

## Git Conventions

- **Default branch**: `master`
- **Feature branches**: Created from `master`, named descriptively (e.g., `new-cool-function`, `new-cool-function2`)
- **Commit messages**: Short, descriptive English messages (e.g., `"Changed by me."`, `"v1.0 text_ver1.0 に First Versionと記載"`)
- **Merging**: Feature branches are merged into `master` via pull requests on GitHub

### Typical Workflow (from How_to_Use_Git+GitHub.txt)

1. Configure git identity: `git config --global user.email / user.name`
2. Clone: `git clone https://github.com/sekstore/hello-world.git`
3. Create a branch: `git branch <branch-name>`
4. Checkout the branch: `git checkout <branch-name>`
5. Edit files
6. Stage new files: `git add <filename>`
7. Commit: `git commit -m "<message>"`
8. Review log: `git log --pretty=oneline`
9. Merge into master: `git checkout master` → `git merge <branch-name>`
10. Push: `git push origin master`

## Development Guidelines for AI Assistants

- **No build system**: There are no build scripts, test suites, package managers, or CI/CD pipelines. Do not attempt to run builds or tests.
- **No programming language**: All files are plain text. Do not introduce source code files unless explicitly requested.
- **Language**: Commit messages and new documentation may be in English. Existing Japanese content should be preserved as-is.
- **Minimal changes**: This is a simple learning repo. Keep any changes focused and small.
- **File additions**: If asked to add files, use plain text unless otherwise specified.
- **Branch discipline**: Always develop on a feature branch and open a pull request; do not commit directly to `master`.
