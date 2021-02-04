---
layout: default
title: Lesson 3 - GitHub Pages
nav_order: 6
---

<!-- Edit the content below for the workshop in question. Once you're ready to publish, remove the comment characters e.g. "<!--" at the start and end -->
# Lesson 3: Create web pages with GitHub Pages
In this lesson, you'll learn how to use GitHub Pages to turn the markdown files in your GitHub repository into a functioning webpage.

## Lesson objectives 
- Explore GitHub repository functionality
- Create a webpage from markdown files using GitHub Pages & jekyll
- Customize your web pages; create a website
- Embed multimedia content

## Lesson video
The following video demonstrates each of the steps outlined below in text:
<iframe height="480" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/fbed2775-7252-4c33-977f-8e232fc6caa3/public?autoplay=false&automute=false"></iframe>

## 1. A GitHub Pages explainer
<iframe width="864" height="514" src="https://www.youtube.com/embed/2MsN8gpT6jY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 2. Explore features and settings | Set up GitHub Pages
In this step, you will explore some of the functionality available in a GitHub repository, which includes GitHub Pages. 
- Ensure that you've created two Markdown files in the ```docs``` folder (```index.md``` and one other), as outlined in [Lesson 2](lesson2).
- Click through the various top-level tabs in the repository to explore the features that are available
![GitHub repository tabs](/assets/img/github-tabs.png)
  - ```Issues``` allow you, collaborators, and external users to report problems with your code and suggest changes
  - ```Pull requests``` lists any requests from external users to merge their code into yours to provide new functionality
  - ```Actions``` allow you to run automate processes from within your GitHub repository
  - ```Projects``` is a Trello-like task planner 
  - ```Wiki``` is a wiki for yourself and collaborators
  - ```Security``` lets you configure security features for your repository and code
  - ```Insights``` shows stats on contributions, viewership, and use of your repository
  - ```Settings``` allows you to configure a variety of other features within your repository
- Open the ```Settings``` Tab. Briefly explore the various options on the side panel.
- Go to ```Settings > Options```. Scroll down to the **GitHub Pages** section
  - For the **Source**, set ```Branch:main``` and set the folder to ```/(root)``` and click **Save**. This directs GitHub pages to the top-level of your repository for your website content.
  - Scroll back down and click ```Choose a theme``` to select a theme for your web page
- Congratulations, your website is ready. The link will be provided in the **GitHub Pages** section.
  - **NOTE**: You may initially receive a ```404 error```, but after a minute, your website will appear with the content from ```index.md``` as the landing page.
  - **NOTE2**: By default, GitHub Pages expects at least one file in the root folder named ```index.md```. This file becomes the homepage for the web page (i.e. ```index.md``` is translated to ```index.html```.

## 3. Customize pages | What is jekyll?
You may have noticed by now that there is another file (```_config.yml```) in your root folder that you didn't create or put there. This is your configuration file, and it's written in a language called [YAML](https://en.wikipedia.org/wiki/YAML). The ```config.yml``` file was created at the time that you turned on GitHub Pages, and it provides instructions to a static site generator software called [jekyll](https://jekyllrb.com/). GitHub pages uses jekyll in the background to convert your Markdown file(s) to formatted HTML to display as web pages. 

There is ***a lot*** that you can do with *jekyll* (within GitHub Pages and as a standalone application on your computer) to generate customized webpages. While only the theme information is set in your file initially, there are many ways that you can [customize it](https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll#default-plugins).  
Here, we'll add a few changes to improve your website's functionality and appearance:
- Use the GitHub editor to open your ```_config.yml``` file for editing.
- Replace the contents of the ```config.yml``` file with the text below (by copying and pasting)

```
title: <your web page title> # EDIT: Fill this in
description: <description of your web page> # EDIT: Fill this in

remote_theme: pmarsceill/just-the-docs # Borrowing the theme from https://github.com/pmarsceill/just-the-docs
github_repo_url: "https://github.com/scds/github-pages" # EDIT: REPLACE WITH THE URL TO YOUR WEBPAGE

# Heading anchor links appear on hover over h1-h6 tags in page content
# allowing users to deep link to a particular heading on a page. (true or false)
heading_anchors: true

# Activate a "Back to top" link
back_to_top: true
back_to_top_text: "Back to top"

# Footer last edited timestamp
last_edit_timestamp: true # show or hide edit time - page must have `last_modified_date` defined in the frontmatter
last_edit_time_format: "%b %e %Y at %I:%M %p" # uses ruby's time format: https://ruby-doc.org/stdlib-2.7.0/libdoc/time/rdoc/Time.html

# A footer with "Edit this page on GitHub" link text
gh_edit_link: true # show or hide edit this page link
gh_edit_link_text: "View this content on GitHub"
gh_edit_repository: "https://github.com/iSci-3A12/intro-github-markdown" # EDIT: ADD THE URL TO YOUR GITHUB REPO
gh_edit_branch: "master" # the branch that your docs is served from
# gh_edit_source: docs # the source that your files originate from
gh_edit_view_mode: "tree" # "tree" or "edit" if you want the user to jump into the editor immediately

# Include plugins for relative links and a remote theme
plugins:
  - jekyll-relative-links
  - jekyll-remote-theme
```

- **NOTE**: The function of each line is explained in comments (i.e. any text on a line that comes after a ```#``` symbol.)
- Edit the information for the four lines tagged with **EDIT:** in the comments.
- **COMMIT** your changes.

## 4. Embedding videos and other web content
As you've already experienced, the nice thing about GitHub Pages (using jekyll) is that it doesn't just accept Markdown--it also accepts HTML code, meaning that you can insert things like embed codes to insert multimedia content.
- Find a video on YouTube that you want to embed into your webpage. Once it begins playing, right click and click on ```Copy embed code```. You should have copied to your clipboard something like this: 

```
<iframe width="1487" height="691" src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

- Paste the embed code into one of your Markdown documents. **COMMIT** your changes.
  - **NOTE**: The embedded video won't show in your rendered Markdown file--it will only appear on your final webpage. 
  - **NOTE**: Remember that it may take a couple of minutes for changes to propagate from your GitHub repo to your webpage.
- You can do the same with other content that provides embed codes, like Google Slideshows, for example.
<br>
<br>
**Have your website up and running?** Head to the [fourth and final lesson](lesson4) to learn how to sync this repository between GitHub and your local computer. 
