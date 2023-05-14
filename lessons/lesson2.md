---
layout: default
title: Lesson 2 - Learn GitHub
nav_order: 2
parent: Lessons
---

# Lesson 2: Learn GitHub
In this first lesson, you'll get some introductory experience creating a GitHub repository and populating it with files from the web interface. 

## Lesson objectives 
- Create a GitHub repository.
- Create folders and files.
- Create and edit a markdown file.

## Lesson video
The following video demonstrates each of the steps outlined below in text:
<iframe height="416" width="100%" allowfullscreen frameborder=0 src="https://echo360.ca/media/db64dd93-a736-4936-9517-8d0a18c16a3e/public?autoplay=false&automute=false"></iframe>

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
- **Commit your changes**

<div style="display: flex;">
<div style="flex-grow: 1;" markdown="1">
[🡨 Lesson 1](lesson1){: .btn .btn-outline} 
</div>

<div markdown="1">
[Lesson 3 🡪](lesson3){: .btn .btn-outline}
</div>
</div>