---
layout: default
title: Lesson 4 - GitHub Desktop
nav_order: 6
---

# Lesson 4 - Syncing with GitHub Desktop (and maybe git) 
In this lesson, you'll learn how to use GitHub Pages to turn the markdown files in your GitHub repository into a functioning webpage. Ensure that you've sucessfully installed [GitHub Desktop](preparation#3a-install-github-desktop-for-windows-or-mac-users) (for Windows and Mac users) or [git](preparation#3b-install-git-for-linux-users-or-adventurous-windowsmac-users) for Linux users. 

## Lesson objectives 
- Clone your GitHub repository to your local machine
- Use GitHub Desktop to control file versions on your local computer
- Push changes back to GitHub (and pull new changes back down)
- Fork a repository

[**Go to GitHub Desktop Instructions**](#github-desktop)  | [**Go to git Instructions**](#git)

# GitHub Desktop
## 1. Clone your repository to your computer
In this step, you will *clone* your existing GitHub repository to your local computer so that you can work on files locally.
### In GitHub
- In the root of your GitHub repository (click on the ```<> Code``` tab to get there) click the green ```Code``` button  ![Green button with the word code](assets/img/code-button.png)
- Copy the https code (e.g. ```https://github.com/scds/github-pages.git```)  
### In GitHub Desktop
- Go to ```File > Clone repository```, and select to add by ```URL```
- Paste the copied URL to your GitHub repository.
- Choose a folder on your local computer where you want to download the repository contents.
- Click ```Clone```



your newly forked repository should appear in the **Your repositories** list (You may need to refresh the list for it to show). 
  - **NOTE:** If it doesn't appear, double-check that the repository exists in your GitHub profile. If it does exist, you can copy the repository URL from GitHub and paste it into the appropriate place using the "Clone a repository from the Internet" button on GitHub Desktop. You can also use this approach to clone someone else's repository!
- Highlight your repository in the list and click "Clone <*repository name*>". Select the local path where you would like to download the repository--a new folder will be created with the name of the repository. 

## 2. Make some changes on your computer
- In GitHub Desktop, click the ```Show in Explorer``` button to open up your file explorer to your repository's contents. 
- Open one of your Markdown (.md) files in a text editor. Make some changes and save them.
- Add a few files (images, maybe?) to the ```docs``` folder. 

### Commit new changes
- In GitHub Desktop, you should be shown the files that have been changed, and be able to view the specific changes. 
- If you are comfortable with the changes, you are ready to commit them.
  - Provide a summary of the changes (or used the suggested text), and lengthier description, if desired.
  - Click **Commit to master**. This commits your changes to your local repository. 
  - If you continue to work on your local files, you will need to again commit changes.  

### Push changes to GitHub (remote) repository
In this step, you'll 'push' your local changes back up to your GitHub repository, so that both are synced. 
- In GitHub Desktop, click the **Push origin** button to send your changes to your GitHub repository.
- Verify your changes in your GitHub repository.

### Make changes in the GitHub (remote) repository
- Make and commit a change to a file in the GitHub (remote) repository using the web editor. 

### Pull changes to the local repository
- In GitHub Desktop, click the **Fetch origin** button. This will check the GitHub repository to see if any changes have been made remotely.
- In GitHub Desktop, click the **Pull origin** button to sync remote changes to your local files. 

### (optional) Advanced: Fork a partner's repository | Request a pull
One of the use cases for version control is that it allows multiple individuals to work on a project at the same time. Collaborators can work on a single 'branch', or (often) they choose to 'fork' it and work on separate branches (with the idea that these branches could be 'merged' later). 

In this exercise, your task is to fork a partner's repository, make some changes locally, 'push' it to your forked repository, and then make a 'pull request' to merge the changes. 
- Navigate to a partner's repository and click the **Fork** button. Follow the prompts to complete the task. 
- If successful, you now have a new repository in your GitHub account that is a 'forked' version of your partner's.
- Make a (minor) edit/change to a Markdown (.md) file using the GitHub editor. Commit the changes
- Click on the **Pull requests** tab for your repository. Click **New Pull Request** and then **Create pull request**
- Your partner will now be notified of a pull request in their repository. They can choose to merge your change (automatically or manually), or reject it. 


# Git
