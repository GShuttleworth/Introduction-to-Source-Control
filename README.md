# Introduction-to-Source-Control

Source control solutions allow you to remotely store a group of files, keep track of changes including when the changes are made and who made them, and intelligently collaborate and share the files within your team.

This lab will be focussing on the [Git](https://git-scm.com/) version control system, however there are plenty of other alternatives available, Git is the most popular and very straightforward to get started with.

# What is Git

Git is a distributed version-control system for tracking changes in source code during software development.

Git was created by Linus Torvalds in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development.

Every Git directory on every computer is a full-fledged repository with complete history and full version-tracking abilities, independent of network access or a central server.

Git is free and open-source software distributed under the terms of the GNU General Public License version 2.

# What is GitHub

GitHub (https://github.com)is a popular cloud service providing hosting for Git repositories.

GitHub hosts repositories for many software projects large and small, open-source, public and private and it is a key resource for developers to share, collaborate on, and discover source code.

# Installing Git

Git is available for Mac, Windows and Linux. To install Git, go to the Git website and install the correct version for your operating system. https://git-scm.com/downloads

To verify you have installed Git correctly, run the following commands in a terminal.

```bash
git --version
```

If everything has installed correctly you will get your installed Git version reported back to you.

# Git Concepts

Git is a very powerful tool and there is lots you can learn. The good news is that you only need to know a few key concepts to get started.

- **Repository (Repo)** - The container that your project files are stored within. This is usually hosted on a remote server.
- **Cloning** - Make a copy of a repository, usually to your own local computer.
- **Commit** - Tell Git to store changes you have made to your local repository.

- **Branch** - A version of the main repository. This allows users to make changes to the repository without altering the master branch. Is is common practice to have separate branches for development, testing and production.

- **Merge** - A way to move changes from one branch into another. E.g. when you have finished testing the changes in your test branch, you can merge the test branch into your production branch.

# Git Workflow

The basic Git workflow looks like this:

1. Create a repository on a remote server (e.g. Github).
1. Clone the remote repository to your local computer.
1. Make changes to your local repository.
1. Add the changes to your local repository to your local Git staging area. (Use the `git add` command.)
1. Commit the changes added to the staging area.
1. Push the local changes to your remote Git repository.

# Git Commands

The basic set of commands you need to start using Git:

- To clone a remote repository:
  ```bash
  git clone <path-to-repository>
  ```
- To update your local repository with the remote repository, downloading any changes that are present:
  ```bash
  git pull
  ```
- Add any changes you have made on your local repository to a staging area in preparation for a commit.
  ```bash
  git add .
  ```
- Commit any file changes added to the staging area into the repository. It is best practice to include a comment about what changes have been made.
  ```bash
  git commit -m "Comment about the changes"
  ```
- Push committed changes on the local repository to the remote repository.
  ```bash
  git push
  ```
