Git and GitHub
1. Introduction to Version Control
Version control is a system that records changes to files over time. It allows developers to inspect, compare, and recover previous versions of a project. It helps track modifications, identify who made changes and when, restore earlier versions, and support teamwork.
Benefits of Version Control
1. Tracks changes and maintains project history.
2. Helps recover from errors or accidental changes.
3. Supports parallel development through branches.
4. Improves collaboration and accountability.
5. Makes projects easier to maintain and reproduce.
2. Types of Version Control Systems
1. Local Version Control: Manages versions on one computer.
2. Centralized Version Control: Stores project history on a central server. Example: Subversion (SVN).
3. Distributed Version Control: Each clone contains repository history. Example: Git.
3. What are Git and GitHub?
- Git: A distributed version control system used to track file changes, maintain commit history, and support parallel development.
- GitHub: An online platform for hosting Git repositories and collaborating through pull requests, Issues, and code reviews.
Git works locally and can be used offline. GitHub provides remote hosting and online collaboration features.
4. Installing and Configuring Git
Download Git for Windows from git-scm.com/downloads. On Ubuntu/Debian, use sudo apt install git; on macOS, use brew install git.

Check the installation and configure the commit identity:
git --version
git config --global user.name "Student Name"
git config --global user.email "student@example.com"
git config --global --list
These configuration values identify the author of commits; they do not authenticate a user to GitHub.
5. Creating a Repository and Basic Workflow
A Git repository stores project files, metadata, branches, and commit history. Initialize one inside a project directory:
mkdir my-project
cd my-project
git init
Git has three main areas:
1. Working Directory: Files being edited.
2. Staging Area: Selected changes prepared for a commit.
3. Repository: Committed project history.
The basic workflow is edit, stage, commit, and then push when a remote is configured.
git status
git add .
git diff --staged
git commit -m "Add initial project"
git log --oneline
Use meaningful commit messages that describe the purpose of each change.
6. Important Git Commands
1. git diff – Shows unstaged changes.
2. git diff --staged – Shows staged changes.
3. git branch – Lists local branches.
4. git switch -c feature-name – Creates and switches to a branch.
5. git merge feature-name – Merges a branch into the current branch.
6. git clone REPOSITORY_URL – Copies a remote repository locally.
7. git fetch – Downloads remote updates without integrating them.
8. git pull – Fetches and integrates remote changes.
9. git push – Sends local commits to a remote repository.
10. git revert COMMIT_ID – Creates a new commit that reverses an earlier commit.
7. GitHub and Collaboration
Create a repository on GitHub, connect it to a local repository, and push commits:
git remote add origin REPOSITORY_URL
git branch -M main
git push -u origin main
A branch provides an independent line of development. A merge conflict occurs when Git cannot automatically combine competing changes; resolve it by editing the affected file, removing conflict markers, staging the result, and completing the merge.

A pull request (PR) proposes changes for review and integration. A fork creates a separate hosted copy of a repository, while clone creates a local copy.
8. GitHub Features and Best Practices
- README.md: Explains a project's purpose, features, installation, and usage.
- .gitignore: Lists files Git should ignore, such as caches, logs, and local environment files.
- Issues: Track bugs, questions, and tasks.
- Projects: Organize tasks and monitor progress.
- Tags and Releases: Mark important versions of a project.
Commit regularly, use descriptive branch names, review and test changes before merging, and keep commits focused. Never upload passwords, API keys, or private tokens. Review repository visibility and permissions.
9. Learning Outcomes
After learning Git and GitHub, students should be able to create and manage repositories, use essential Git commands, maintain project history, publish projects online, work with branches, resolve merge conflicts, and collaborate through pull requests.