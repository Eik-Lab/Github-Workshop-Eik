# Git and GitHub Workshop for Beginners

Welcome to the Git and GitHub workshop! This guide is designed for participants who have never used Git or GitHub before. By the end of this workshop, you'll have a basic understanding of version control, Git, and how to collaborate using GitHub.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installing Git](#installing-git)
- [Basic Git Concepts](#basic-git-concepts)
- [Using GitHub](#using-github)
- [Collaboration Workflow](#collaboration-workflow)
- [Additional Resources](#additional-resources)

## Introduction

Version control is a system that helps you manage changes to your code over time. Git is a popular version control system, and GitHub is a platform that hosts Git repositories and adds collaboration features. This workshop will introduce you to the fundamental concepts of Git and how to use GitHub for collaborative projects.

## Prerequisites

Before you start, make sure you have:

- A basic understanding of coding concepts.
- A GitHub account. If you don't have one, you can sign up [here](https://github.com/join).
- Git installed on your computer. You can download it from [here](https://git-scm.com/downloads).

## Installing Git

### Windows

If you're using Windows, you can install Git using Windows PowerShell:

1. **Open Windows PowerShell:**
   - Search for "PowerShell" in the Windows search bar and open it.

2. **Install Git:**
   - Run the following command in PowerShell:
   
     ```bash
     choco install git -y
     ```
   
     This will use the Chocolatey package manager to install Git.

3. **Verify Installation:**
   - After the installation is complete, you can verify it by running:
   
     ```bash
     git --version
     ```
   
     You should see the Git version number.

### macOS

If you're using macOS, Git might already be installed. To check if it's installed:

1. **Open Terminal:**
   - You can find Terminal in the Applications > Utilities folder.

2. **Check for Git:**
   - In the Terminal, enter the following command:
   
     ```bash
     git --version
     ```

   - If Git is installed, you'll see the version number.

3. **Install Git (if not installed):**
   - If Git is not installed, macOS might prompt you to install it when you use Git for the first time. Follow the prompts to install it.

## Basic Git Concepts

1. **Repository (Repo):**
   - A repository is where your project's files and revision history are stored.

2. **Commit:**
   - A commit is a snapshot of your code at a specific point in time. It helps you track changes and add descriptions.

3. **Branch:**
   - A branch is a separate line of development. It's useful for working on features without affecting the main codebase.

4. **Pull Request (PR):**
   - A pull request is a request to merge changes from one branch into another. It's used for code review and collaboration.

## Using GitHub

### Create a Repository

1. Click the "New" button on your GitHub profile.
2. Give your repository a name and optional description.
3. Choose visibility (public or private).
4. Initialize with a README (optional).

### Making Changes

1. Edit files directly on GitHub or clone the repository and make changes locally.
2. Use `git add` to stage changes and `git commit` to save them.
3. Push changes to your repository using `git push`.

## Collaboration Workflow

1. Create a new branch for your feature.
2. Make and commit your changes.
3. Push your branch to GitHub.
4. Open a pull request to merge changes.
5. Collaborators review and discuss the changes.
6. Make additional commits based on feedback.
7. Once approved, merge the pull request.
