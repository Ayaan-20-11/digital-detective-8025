# Mission 0 — Create your GitHub Workspace

## 1. Task / Objective

The objective of this mission was to create a GitHub repository with the required naming convention and prepare an organised folder structure for all nine missions of the Digital Detective assignment.

## 2. Work Completed

- Selected the repository name: `digital-detective-8025`.
- Created the local project folder on the Desktop.
- Created all nine mission folders.
- Created a separate README.md inside every mission folder.
- Created the root README.md.
- Created the `number_converter.py` file inside Mission 5.
- Created the `evidence` folder.
- Prepared the root README with a project introduction, mission index and project workflow.

## 3. Commands / Tools Used

| Command / Tool | Purpose |
|---|---|
| `mkdir -p` | Created the mission folders and evidence folder. |
| `touch` | Created empty README and Python files. |
| `cd` | Changed the current directory to the project folder. |
| `pwd` | Displayed the current working directory. |
| `find . -print` | Listed the complete folder and file structure. |
| `code .` | Opened the project folder in Visual Studio Code. |
| `python3 --version` | Checked the installed Python version. |
| `git --version` | Checked the installed Git version. |
| Visual Studio Code | Used to edit the Markdown documentation. |

### Installed Tool Versions

- Python: 3.14.5
- Git: 2.54.0 (Apple Git-157)

## 4. My Understanding

A GitHub repository is a place where project files and their version history can be stored and managed. Git helps track changes made to files, while GitHub allows the repository to be hosted online and shared.

Organising the assignment into separate mission folders makes the project easier to navigate, maintain and review. Each mission has its own README so that its activities and learning can be documented independently.

## 5. Difficulties Faced

During the initial Git commit, Git automatically used the local Mac username and hostname as the commit identity. I wanted to avoid exposing local device information in the public repository.

## 6. How I Resolved Them

I configured a repository-specific Git username and GitHub-provided noreply email address. I then amended the initial commit using `git commit --amend --reset-author --no-edit` and verified the updated author and committer details before pushing.

## 7. Evidence / Files

- Root README.md
- Mission 0 to Mission 8 folders and their README.md files.
- Mission 5 number_converter.py
- evidence folder
- Verified folder structure using the Terminal.

## 8. Commit Details

- Commit message: `Set up Digital Detective mission structure`
- Initial commit hash: `e9f5c50`
- Branch: `main`
- Remote repository: https://github.com/Ayaan-20-11/digital-detective-8025
- Status: Successfully pushed to GitHub.