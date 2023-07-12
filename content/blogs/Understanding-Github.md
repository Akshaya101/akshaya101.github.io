---
title: "Understanding Github"
date: 2022-04-22T20:07:12+05:30
description: 'This article summarizes the importance of Github.'
ShowBreadCrumbs: true
ShowToc: true
TocOpen: false
cover:
    image: "images/workflow.png"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "<alt text>"
    caption: "<text>"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
---

### Version Control

Version Control or Source Control is the practice of tracking and managing changes made in the software code. Version Control Systems are software tools which allow you to track and manage all the changes that are made to the source code during the development of a project. It keeps track of changes made in the source code and allows you to roll back to the previous version whenever necessary.

### Need of Version Control Systems

- Version Control Systems are necessary as they help you keep track of your code, and access it whenever necessary. If the code is stored locally, the source code is lost whenever the system crashes.
- Distributed Version Control Systems checks out the latest version where each collaborator will have an exact copy (mirroring) of the main repository(including its entire history) on their local machines. Here each user has their own repository (like on Github) and a working copy (on the local machine).

### Git vs Github

- Git : Git is a version control software tool that is used to track changes of the source code.
- Github : Github is a web-cloud based platform that hosts your source code.

Note that, it is possible for Git to exist without Github, but vice versa is not possible.

### Github Workflow

A Git project consists of three main parts

- Repository
    - Consider Github to be a bookshelf, each book on the shelf can be called a repository.
    - A repository holds details and files related to a project.
    - The repository also keeps track of all commits made during the development of projects.
    - Commits can be said to be changes that are made to a single or set of files. Whenever you make a commit a unique ID or SHA or hash is created that allows you to keep track of specific changes that have been made. Commit messages are usually short texts that describe the changes made in the project briefly. A list of commits that have been made in a project can be obtained by using the command git log.
    - Repositories have 2 scopes: public and private.
- Working tree
    - The files and folders that a developer adds to the Git repository residing outside the **.git** folder are known as the Git working tree.
- Staging Area
    - The staging area is where commits are prepared.
    - The repository is compared with the working tree, the staging area marks the files before they are committed.

To sum up!

- Working tree(locally existing files) → Staging area(where files are sent after changes are made) → repository(those files which are passed from the staging area onto the repository)

### Types of files you find during development

- Tracked Files : Tracked files are those files that are added and committed, these files are sent into the staging area so that they could be sent to the remote repository or in simple terms the place where your code is stored.
- Untracked Files : Untracked files are those files that are present in your working directory but are not added to the staging area, hence are not queued to send to the remote repository.

### States of Git Files

Three main states any file undergoes are : 

- Modified
- Staged
- Committed

→ When you create and modify a file in the working directory/tree, it will only be updated locally. 

→ The file must then be sent to staging area if you want to include them in your next commit.

→ Once the files are committed with proper message, they are then pushed to the remote repository, where they will be stored safely.

Being aware of how Git and Github work is very important, especially when you're just starting out. If you're trying to share your code with the world or if you want to contribute to open source, knowing Github inside and out would be helpful.