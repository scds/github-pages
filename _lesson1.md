---
layout: default
title: Lesson 1 - Learn GitHub
nav_order: 3
---

<!-- Edit the content below for the workshop in question. Once you're ready to publish, remove the comment characters e.g. "<!--" at the start and end -->

# Lesson 1: Learning GitHub

## Lesson objectives 
- Create a GitHub repository.
- Create folders and files.
- Create and edit a markdown file.

## 1. Create a new GitHub repository
A repository is a container for related materials (i.e. folders and files), that allows for them to be managed (stored, version-tracked) and shared together. Usually, you create a separate repository for each project that you are working on. [Here are the New York Times' GitHub repositories](https://github.com/nytimes), for example.
- Ensure you have [created a GitHub account](preparation#2-create-a-github-account) and are logged in.
- From your GitHub main page, click on the green **New Repository** button. This is the repository (storage location) where the content of your website will be hosted. 
  - Provide a name for your repository. The name you enter will determine the URL of your repository.
    - The repository URL will take the form: ```https://github.com/<your-github-username>/<your-repo-name>```
	- e.g. ```https://github.com/jasonbrodeur/test-pages```
- Check the box to **Initialize this repository with a README**
	- **NOTE**: Your README file is a plain text file (same as a .txt file) that typically contains descriptive information about your repository (Who made it? What does it contain? What is it for?, etc.). The ```.md``` extension indicates to GitHub that this is a Markdown file (more on that later). One of the nice features of markdown files is that they are readable by almost any applications (and humans), since they are mostly just plain text files.
- Click the **Create repository** button
- Your browser will now open to the top-level page of the repository. Your repository will contain one file: **README.md**. 

## 2. Add files and folders
In this step, you'll create a file and folder in your repository and upload a file from your computer to your new folder. You will eventually use all of these items to create your first webpage with GitHub Pages 
 
### Create a file 
- In the top-level repository page (which you can navigate to by clicking the ```<> Code``` tab), click ```Add file > Create new file```
- When prompted to name your file, title it ```index.md```. This creates an empty text file that GitHub will assume contains Markdown code.
- Scroll down to the **Commit new file** section. Add a short description (or use the suggested one) and click ```Commit change```.
  - **NOTE**: Unlike programs such as Google Docs, GitHub does not save your changes automatically. Rather, you have to instruct it to **Commit** the changes, which takes a snapshot of the file and saves it as the newest version. 
  - **NOTE**: There are two comment boxes that can be filled in when committing changes. The short description **is required**--ideally, it comtains a brief message about the changes you made to the file. An optional larger description box can be filled out, as well. 
  
### Edit your text file
- Click on your ```index.html``` file to view it, and then click the edit button (pencil icon) to switch to editing mode
- Add a bit of text to this file (anything is fine for now). 
- When finished editing, modify the commit message and add a longer description (if desired) and **commit your changes**. 

### View your changes and change history
- While viewing your ```index.md``` file, explore the ```Blame``` and ```History``` buttons to better understand how GitHub keeps track of and visualizes file changes. 

### Create a folder 
- In the top-level repository page, click ```Add file > Create new file```
- When prompted to name your file, enter ```images/temp.txt```. **Commit your changes**. This will create a folder called ```images``` and an empty file inside of it called ```temp.txt``` (which can be deleted later, once you've moved more files into the images folder).

### Upload a file 
- Make sure you are located within the ```images``` folder (you should see your ```temp.txt``` file). 
- Click ```Add file > Upload files```. 
- Select an image from your computer to upload. If you want to download something from the web, try to use something that is not copyrighted or is royalty free ([e.g.](https://www.pexels.com/royalty-free-images/))


We want to create a folder named ```images``` in the top level of the repository. This folder will hold image content that we want to share on our webpage. 
- **NOTE**: In GitHub, a folder can't be created until there is a file inside of it. This means that to create an empty folder, you will have to [create a temporary file](https://github.com/KirstieJane/STEMMRoleModels/wiki/Creating-new-folders-in-GitHub-repository-via-the-browser) inside of it at the same time. 

You can , you need to add a trailing slash (/) to the name, and you need to create a file within the folder], since empty folders aren't saved. You can always delete this file later.
	- In the **Name your file...** box, enter ```docs/index.md```. Click **Commit change**. You will now have a folder named ```docs``` in your repository with a file named ```index.md```.




<!--

After ensuring that you've followed the [Preparatory steps](preparation), open Tableau and follow along with the workshop recording or slides. 

## Workshop recording

<iframe height="480" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/4378b2ec-7d0c-4632-a1e4-5a8076a494da/public?autoplay=false&automute=false"></iframe>

View the original [here](https://echo360.ca/media/4378b2ec-7d0c-4632-a1e4-5a8076a494da/public).


## Workshop slides

<div style="position:relative;padding-top:66.25%;">
<iframe src="//docs.google.com/viewer?url=https://github.com/scds/intro-tableau/raw/main/assets/docs/tableau_20201118.pdf?dl=0&hl=en_US&embedded=true" class="gde-frame" style="position:absolute;top:0;left:0;width:100%;height:100%;border:none;" scrolling="no"></iframe>
</div>
[Download as a PDF](https://github.com/scds/intro-tableau/raw/main/assets/docs/tableau_20201118.pdf)
<br>

## Worksheets
**Coming soon!**


-->
