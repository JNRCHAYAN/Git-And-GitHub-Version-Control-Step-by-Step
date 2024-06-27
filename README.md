# Git and GitHub: Version Control Step-by-Step

## What is GitHub?

GitHub is a web-based platform used for version control and collaborative development of projects. It uses Git, an open-source version control system, to track changes in the code. GitHub provides a central repository where developers can store and manage their code, track issues, review code, and collaborate with other developers.

## What is Git?

Git is a distributed version control system designed to handle everything from small to very large projects with speed and efficiency. It allows multiple developers to work on a project simultaneously without interfering with each other's changes. Git tracks changes, allows for branching and merging, and provides a history of all changes made to the codebase.

## Differences Between Git, GitHub, and Google Drive

| Feature/Functionality | Git                          | GitHub                        | Google Drive                    |
|-----------------------|------------------------------|-------------------------------|---------------------------------|
| **Type**              | Version Control System       | Hosting service for Git repositories | Cloud Storage Service           |
| **Collaboration**     | Yes, through branching/merging | Yes, with additional features for collaboration and project management | Yes, but primarily for document sharing and collaboration |
| **Version Tracking**  | Yes                          | Yes                           | Limited                         |
| **Local Repository**  | Yes                          | No, but works with local Git repositories | No                              |
| **Code Review**       | No                           | Yes                           | No                              |
| **Issue Tracking**    | No                           | Yes                           | No                              |

## Installing Git Bash

### On Windows

1. Download Git for Windows from [git-scm.com](https://git-scm.com/download/win).
2. Run the downloaded installer.
3. Follow the instructions in the setup wizard. It is recommended to use the default settings.

### On Mac

1. Open Terminal.
2. Install Homebrew if not already installed:
   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
3. Install Git using Homebrew:
   ```sh
   brew install git
   ```
### On Linux
1. Open Terminal
2. Update the package list:
   ```sh
   sudo apt update
   ```
3. Install Git:
   ```sh
   sudo apt install git
   ```
### Setting Up Git After Installation
1. Open Git Bash (Windows) or Terminal (Mac/Linux).
2. Configure your Git username:
   ```sh
   git config --global user.name "Your Name"
   ```
3. Configure your Git Email:
   ```sh
   git config --global user.email "your.email@example.com"
   ```

### Using Git and GitHub
## Basic Git Commands
1. Initialize a Repository in your local machine:
   ```sh
   git init
   ```
2. Create a repository on GitHub and copy the link of the repository then add this to the local repository of your machine:
   ```sh
   git add origin https::github.com/your_github_user_name/your_repository_name
   ```
3. Check changes:
   ```sh
   git status
   ```
4. Moved untracked file to tracked file:
   1. Add a specific file
      ```sh
      git add "file name"
      ```
   2. Add all files:
      ```sh
      git add .
      ```
5. Moved tracked file to stage by commit or saved in local repository:
   ```sh
   git commit -m "comments"
   ```
6. Push the committed file to GitHub repository:
   ```sh
   git push -u origin branch_name
   ```
   No need to use "-u origin branch_name" if you are pushing into an existing branch of GitHub and it is the present branch of the local machine. But you need to use it when you want to push another branch.
7. Create a new branch:
   ```sh
   git checkout -b branch_name
   ```
8. To check the branches:
   ```sh
   git branch
   ```
9. Go to the existing branch
   ```sh
   git checkout branch_name
   ```
10. Clone the repository on local
    ```sh
    git clone repository_link
    ```
11. To pull something from branch:
    ```sh
    git pull origin branch_name
    ```
    No need to use "origin branch_name" if you are pulling from present branch.


Other my Commnd 

| Command                                            | Description                                                                 |
|----------------------------------------------------|-----------------------------------------------------------------------------|
| `git config --global user.name jnrchayan`          | Set global Git username                                                      |
| `git config --global user.email jnrchayan@gmail.com`| Set global Git email address                                                |
| `git init`                                         | Initialize a new Git repository in the current directory                     |
| `ls -lart`                                         | List all files and directories, including hidden ones                       |
| `git status`                                       | Check the current status of the repository                                   |
| `git add chayan.cpp`                               | Add `chayan.cpp` to the staging area                                         |
| `git commit`                                       | Commit changes in the staging area to the repository                        |
| `git commit -m "Initial commit"`                   | Commit with a message ("Initial commit")                                     |
| `git checkout -f`                                  | Force checkout to discard local changes and revert to the last commit        |
| `touch roy.cpp`                                    | Create a new file `roy.cpp`                                                  |
| `git add -A`                                       | Add all changes (including untracked files) to the staging area              |
| `git commit -m "Added more cpp"`                   | Commit all staged changes with a message                                     |
| `git checkout roy.cpp`                             | Restore `roy.cpp` from the last commit                                       |
| `git log`                                          | Display commit history                                                       |
| `git log -p -1`                                    | Show the last commit with changes                                            |
| `git diff`                                         | Show unstaged changes between working directory and staging area             |
| `git diff --staged`                                | Show staged changes between staging area and the last commit                 |
| `git commit -a -m "Skipped staging area and fixed"`| Commit all modified files, skipping the staging area with a message          |
| `git rm dele.cpp`                                  | Remove `dele.cpp` from both working directory and staging area               |
| `git restore --staged dele.cpp`                    | Unstage `dele.cpp` (restore from staging area)                               |
| `git rm --cached chayan.cpp`                       | Remove `chayan.cpp` from the tracking (unstage without deleting the file)    |
| `git commit -a -m "Removing waste"`                | Commit all changes (including deletions) with a message                     |
| `touch .gitignore`                                 | Create a `.gitignore` file to specify files to ignore                        |
| `git commit -a -m "ignored some files and added gitignore"` | Commit changes to `.gitignore` with a message                        |
| `git branch feature1`                              | Create a new branch named `feature1`                                         |
| `git branch`                                       | List all branches                                                            |
| `git checkout feature1`                            | Switch to branch `feature1`                                                  |
| `git checkout master`                              | Switch back to `master` branch                                               |
| `git merge feature1`                               | Merge `feature1` branch into the current branch (`master`)                   |
| `git checkout -b 'flaskfile'`                      | Create and switch to a new branch named `flaskfile`                          |
| `git remote add origin https://github.com/JNRCHAYAN/Git_Test.git` | Link local repository to a remote repository on GitHub         |
| `git remote`                                       | List remote repositories                                                    |
| `git remote -v`                                    | Show remote repositories with URLs                                          |
| `git push origin master`                           | Push `master` branch changes to remote `origin` repository                   |
| `git push -u origin flaskfile`                     | Push `flaskfile` branch changes to remote `origin` repository, set upstream  |
| `git clone https://github.com/JNRCHAYAN/Git_Test.git` | Clone a repository from GitHub to local machine                              |


  
