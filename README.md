# Tutorial on Hosting a Resume on Github Pages

Learn how to create and publish your resume on a website using Markdown, Visual Studio Code, GitHub Pages, and Jekyll.

- [Tutorial on Hosting a Resume on Github Pages](#tutorial-on-hosting-a-resume-on-github-pages)
  - [Prerequisites](#prerequisites)
  - [Instructions](#instructions)
    - [1. GitHub Pages](#1-github-pages)
    - [2. Hosting Your Site](#2-hosting-your-site)
    - [3. More Resources](#3-more-resources)
  - [Authors and Acknowledgements](#authors-and-acknowledgements)

## Prerequisites
Before you start, make sure you have the necessary tools installed:

- **Markdown Editor** 
  - Using a markup language can be really helpful. Andrew Etter explains in his book "Modern Technical Writing" that it's important because it makes it easy to create content that can be shared online, like XML[^1]. Out of all the markup languages out there, I chose Markdown because it's the most commonly used and it's pretty versatile[^2].
  - You can use any markdown editors of your choice, but I like to use [VS Code](https://code.visualstudio.com/download). 
  - Other Markdown editor options: [Typora](https://typora.io/), [Ghostwriter](https://ghostwriter.kde.org/), or [Atom](https://atom.io/)
  - I have provided a Markdown tutorial in [More Resources](#3-more-resources).
- **GitHub Account**: 
  - Sign up [here](https://github.com/) for a GitHub account if you don't have one. This will allow you to store your code in a repository online for free and use [GitHub Pages](https://pages.github.com/).
- **Git & Git Desktop**: 
  - Install [Git](https://git-scm.com/downloads). Andrew Etter states that using a GUI system such as Git is better for basic everyday operations.[^3]
  - Use [Github Desktop](https://desktop.github.com/) to connect your local computer files to the repository.  Connect your account and clone the `[your-github-name].github.io` repository. This will allow you to push your files to the repository. 
  - If you ever get stuck, I have provided a link in [More Resources](#3-more-resources) where you can find more information on how to navigate Git Desktop.
- **Resume in Markdown**: 
  - I have provided a copy of my own [resume](index.md) for use in this repository. My resume is a template. Feel free to edit and personalize it using the markdown editor of your choice. ![resumegif](https://media0.giphy.com/media/72YyXcnj0DVZzVaF2d/giphy.gif)

- **Ruby & Jekyll**: 
  - Install [Ruby](https://www.ruby-lang.org/en/documentation/installation/) and [Jekyll](https://jekyllrb.com/docs/installation/) to run your website. 

## Instructions
### 1. GitHub Pages
   
**Creating a Repository:**
- Go to [GitHub](https://github.com/) and create a repository named `[your-github-name].github.io`.
  ![Create Repository]()
- Use Git Desktop to clone `[your-github-name].github.io` repository to your computer.

### 2. Hosting Your Site
Hosting a static website allows you to easily keep your content up to date and accessible to anyone. We'll use Jekyll for this because of its popularity, and it's recommended by Andrew Etter[^4]. Andrew Etter explains that static websites are basically just a bunch of simple markup files that you can edit using any text editor you like[^5].

1. **Verifying Ruby and Jekyll**
   - Verify installation by running `ruby -v` on the command line or terminal.
   - Confirm installation with `jekyll -v` on the command line or terminal.
   - Follow Jekyll's [Quickstart Guide](https://jekyllrb.com/docs/) for your OS.

2. **Initialize Your Site:**
   - Open your command line and navigate to your repository directory. For example: `cd Documents/GitHub/[your-github-name].github.io`
   - Run `jekyll new [your-site-name]` on the command line.
   - Navigate into the newly created folder by typing `cd [your-site-name]`.
   - Install `webrick` by running `bundle add webrick` and `bundle install`.
   - Start hosting your site with `bundle exec jekyll serve`.
   - Your site will be live at the provided LocalHost URL, which is in your terminal. Open the link in your web browser, and you can see that your site is created!

3. **Edit Your Resume:**
   - Copy your **resume.md** file to the `_posts` folder in `[your-github-name].github.io`.
   - Rename the file with the date format `YYYY-MM-DD-resume.md`.
   - Add to the top of your resume markdown file so the Jekyll compiler can find your resume and list it as a post.
```
---
layout: post
title:  "Resume"
date:   [current date + time]
categories: jekyll update
---
```

1. **Push and View Your Website:**
   - Use Git Desktop to push your changes to the repository.
   - Visit `https://[your-github-name].github.io` to see your website live with your resume.

### 3. More Resources

1. [Markdown Tutorial](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax): This tutorial will help you learn Markdown.
2. [Andrew Etter's *Modern Technical Writing*](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS): Dive deeper into Technical Writing with this book.
3. [Git Tutorials](https://www.atlassian.com/git/tutorials): Understanding Git will be valuable as you progress. Troubleshooting and reading over this tutorial when you feel like you're stuck will make it easier for yourself in the future.

## Authors and Acknowledgements

[Jacob Seraspi](https://github.com/jacobseraspi)

Thanks to my group mates:
- [Farah Hegazi]()
- [Fengfan Bian]()

Acknowledgements to 

[^1]: Andrew Etter - Modern Technical Writing, 33  
[^2]: Andrew Etter - Modern Technical Writing, 39  
[^3]: Andrew Etter - Modern Technical Writing, 46  
[^4]: Andrew Etter - Modern Technical Writing, 51  
[^5]: Andrew Etter - Modern Technical Writing, 52  