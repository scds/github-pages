---
layout: default
title: Lesson 4 - GitHub Desktop
nav_order: 7
---

# Lesson 4 - Sync with GitHub Desktop (and maybe git) 
In this lesson, you'll learn how to use GitHub Pages to turn the markdown files in your GitHub repository into a functioning webpage. Ensure that you've sucessfully installed [GitHub Desktop](preparation#3a-install-github-desktop-for-windows-or-mac-users) (for Windows and Mac users) or [git](preparation#3b-install-git-for-linux-users-or-adventurous-windowsmac-users) for Linux users. 

## Lesson objectives 
- Clone your GitHub repository to your local machine
- Use GitHub Desktop to control file versions on your local computer
- Push changes back to GitHub (and pull new changes back down)
- Fork a repository

## Lesson video
The following video demonstrates each of the steps outlined below in text:
<iframe height="480" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/99e82d8b-81a2-485e-afc6-236bd169c898/public?autoplay=false&automute=false"></iframe>

[**Go to GitHub Desktop Instructions**](#github-desktop)  |  [**Go to git Instructions**](#git)

# GitHub Desktop
## 1. Clone your repository to your computer
In this step, you will *clone* your existing GitHub repository to your local computer so that you can work on files locally.
### In GitHub
- In the root of your GitHub repository (click on the ```<> Code``` tab to get there) click the green ```Code``` button  ![Green button with the word code](assets/img/code-button-sm.png)
- Copy the https code (e.g. ```https://github.com/scds/github-pages.git```)  
### In GitHub Desktop
- Go to ```File > Clone repository```, and select to add by ```URL```
- Paste the copied URL to your GitHub repository.
- Choose a folder on your local computer where you want to download the repository contents--a new folder will be created with the name of the repository. 
- Click ```Clone```
  - **NOTE**: You can also use this approach to clone someone else's GitHub repository!

## 2. Make some changes on your computer
- In GitHub Desktop, click the ```Show in Explorer``` button to open up your file explorer to your repository's contents. 
- Open one of your Markdown (.md) files in a text editor. Make some changes and save them.
- Add a few files (perhaps some images to the ```images``` folder?). 

## 3. Commit new changes
- In GitHub Desktop, you should be shown the files that have been changed, and be able to view the specific changes. 
- If you are comfortable with the changes, you are ready to commit them.
  - Provide a summary of the changes (or used the suggested text), and lengthier description, if desired.
  - Click ```Commit to master```. This commits your changes to your local repository (but not yet to your GitHub one!). 
  - If you continue to work on your local files, you will need to again commit changes.  

## 4. Push changes to your GitHub (remote) repository
In this step, you'll *push* your local changes back up to your GitHub repository, so that both are synced. 
- In GitHub Desktop, click the ```Push origin``` button to send your changes to your GitHub repository.
- Verify your changes in your GitHub repository by clicking on the ```View on GitHub``` button.

## 5. Make changes in the GitHub (remote) repository
- Make and commit a change to a file in the GitHub (remote) repository using the web editor. 

## 6. Pull changes to the local repository
- In GitHub Desktop, click the **Fetch origin** button. This will check the GitHub repository to see if any changes have been made remotely.
- In GitHub Desktop, click the **Pull origin** button to sync remote changes to your local files. 

**Congratulations, you've made it to the end!** If you'd like to explore more, head to the [Learn More](learn-more) page.


# Git
These instructions assume that you have basic experience using the command line. 

## 0. Configure your git account 
Open up **git Bash** and navigate to the desired directory for your repository using the command line
- Set your name: ```git config --global user.name "John Doe"```
- Set your email address: ```git config --global user.email johndoe@example.com```
- Check your settings ```git config --list```
See [git documentation](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) for more information.

## 1. Clone your repository to your computer
In this step, you will *clone* your existing GitHub repository to your local computer so that you can work on files locally.
### In GitHub
- In the root of your GitHub repository (click on the ```<> Code``` tab to get there) click the green ```Code``` button  ![Green button with the word code](assets/img/code-button-sm.png)
- Copy the https code (e.g. ```https://github.com/scds/github-pages.git```)  
### In git Bash
- Open Git Bash in the desired directory for your repository. Enter the command: ```git clone <copied url>```, where ```<copied_url>``` is the URL you copied in the previous step.
- Git should now download the contents of your GitHub repository to a new folder in your current directory
  - **NOTE**: You can also use this approach to clone someone else's GitHub repository!

## 2. Make some changes on your computer
- In your local repository folder, open one of your Markdown (.md) files in a text editor. Make some changes and save them.
- Add a few files (perhaps some images to the ```images``` folder?). 

## 3. Add and commit new changes
- In **git Bash**, check the status of your repository (i.e. what's been modified): ```git status```
  - This will provide a list of items that are not yet being tracked (i.e. have not been added to the index), and those that are being tracked and have been modified.
- Add new items to the list of tracked files (individually): ```git add <filename>```
  - **OR** Add all items to this list of tracked files: ```git add --all```
- Commit changes to git (i.e. record changes): ```git commit -m '<enter a note on what has changed>'```
  - **OR** add and commit all at once: ```git commit -a -m '<enter a note on what has changed>'```

## 4. Push changes to GitHub (remote) repository
- To check if there are connected remote repositories use the command: ```git remote -v```
- Push changes to the target GitHub repository using the command: ```git push origin main```
  - In this example -- which is the default case -- **origin** specifies the remote (i.e. GitHub) repository that is the target of your 'push'. **main** specifies the branch of the git repository that you're working on as the source data.
- Verify your changes in your GitHub repository.

## 5. Make changes in the GitHub (remote) repository
- Make and commit a change to a file in the GitHub (remote) repository using the web editor. 

## 6. Pull changes to the local repository
- In **git Bash**, you can check changes (before merging them) with: ```git fetch```, and then ```git diff origin master```
- Pull (fetch and merge) changes: ```git pull origin master```
  - **Note:** ```git pull``` actually runs two processes: ```fetch``` (get changes) and ```merge``` (place in your directory) 
- Inspect the changes to your local repository.
<br>
<br>
**Congratulations, you've made it to the end!** If you'd like to explore more, head to the [Learn More](learn-more) page.
