# Tutorial on Hosting a Resume on Github Pages

Learn how to create and publish your resume on a website using Markdown, Visual Studio Code, GitHub Pages, and Jekyll.

- [Tutorial on Hosting a Resume on Github Pages](#tutorial-on-hosting-a-resume-on-github-pages)
  - [Prerequisites](#prerequisites)
  - [Instructions](#instructions)
    - [1. GitHub Pages](#1-github-pages)
    - [2. Hosting Your Site](#2-hosting-your-site)
    - [3. More Resources](#3-more-resources)
  - [Authors and Acknowledgements](#authors-and-acknowledgements)
  - [FAQs](#faqs)
    - [1. Why is Markdown preferable to a word processor?](#1-why-is-markdown-preferable-to-a-word-processor)
      - [Ease of Use](#ease-of-use)
      - [Web Compatibility](#web-compatibility)
    - [2. Why isn't my resume displaying?](#2-why-isnt-my-resume-displaying)

## Prerequisites
Before you start, make sure you have the necessary tools installed:

- **Markdown Editor** 
  - Using a markup language can be really helpful. Out of all the markup languages out there, I chose Markdown because it's the most commonly used and it's pretty versatile[^1]. Andrew Etter explains in his book "Modern Technical Writing" that it's important because it makes it easy to create content that can be shared online, like XML[^2]. 
  - You can use any markdown editors of your choice, but I like to use [VS Code](https://code.visualstudio.com/download). 
  - Other Markdown editor options: [Typora](https://typora.io/), [Ghostwriter](https://ghostwriter.kde.org/), or [Atom](https://atom.io/)
  - I have provided a Markdown tutorial in [More Resources](#3-more-resources).
- **GitHub Account**: 
  - Sign up [here](https://github.com/) for a GitHub account if you don't have one. This will allow you to store your code in a repository online for free and use [GitHub Pages](https://pages.github.com/).
- **Git & Git Desktop**: 
  - Install [Git](https://git-scm.com/downloads). Andrew Etter states that using a GUI system such as Git is better for basic everyday operations.[^3]
  - Use [Github Desktop](https://desktop.github.com/) to connect your local computer files to the repository.  Connect your account and clone the `[your-github-name].github.io` repository. This will allow you to push your files to the repository. 
  - If you ever get stuck, I have provided a link in [More Resources](#3-more-resources) where you can find more information on how to navigate Git Desktop.

## Instructions
### 1. GitHub Pages
   
**Creating a Repository:**
- Go to [GitHub](https://github.com/) and create a repository named `[your-github-name].io`.  
  ![Create Repository](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNXFraW5ndG9pazQ0dDNpMmEzZjE5Ym1nZDZrc2xyeXNjd29zM3lwaiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/ffwCPcPxAyxXr5gJbs/giphy.gif)
- Use Git Desktop to clone `[your-github-name].io` repository to your computer.

**Choosing a theme:**
- Here are some Jekyll [themes](https://pages.github.com/themes/)
- In your 'config.yml' file, fill in the theme of your choice. In my example, I used the midnight theme.
```
remote_theme: pages-themes/midnight@v0.2.0
plugins:
- jekyll-remote-theme 
```

### 2. Hosting Your Site
Hosting a static website allows you to easily keep your content up to date and accessible to anyone. Andrew Etter explains that static websites are basically just a bunch of simple markup files that you can edit using any text editor you like[^4]. We'll use a Jekyll for this because of its popularity, and it's recommended by Andrew Etter[^5]. 


1. **Initialize Your Site:**
   - In Github, go to settings > pages > select main branch as the source.  
    ![Static Site Generation](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNmk0azdlbzdqYWVmb216eXd2amNoMjgyb2U0NXdybnU0bHhxNDNreiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/wvhPyqNlwhP36mmbHo/giphy.gif)
   - This will allow Github to build your website.
  
1. **Edit Your Resume:**
     - I have provided a copy of my own [resume](index.md) for use in this repository. Feel free to edit and personalize it using the markdown editor of your choice.  
    ![Resume](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZHZzcGFyeWEwNXpoMm5wb2NzbTR1M3h0YThham40amcwNG9taWVvYyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/RNok9IhsyZ9a3wWr3G/giphy.gif)

2. **Push and View Your Website:**
   - Use Git Desktop or Visual Studio Code to push your changes to the repository.
   - Visit `https://git-username.github.io/repository-name/`. Make sure you fill in your Github username as well as the repository name, and there you have it, a functional static website!

### 3. More Resources

1. [Markdown Tutorial](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax): This tutorial will help you learn Markdown.
2. [Andrew Etter's *Modern Technical Writing*](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS): Dive deeper into Technical Writing with this book.
3. [Git Tutorials](https://www.atlassian.com/git/tutorials): Understanding Git will be valuable as you progress. Troubleshooting and reading over this tutorial when you feel like you're stuck will make it easier for yourself in the future.
4. [Jekyll Theme Tutorial](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll): An additional resource for how to apply a Jekyll theme to your Github Pages site.

## Authors and Acknowledgements

[Jacob Seraspi](https://github.com/jacobseraspi)

Thanks to my group mates:
- [Farah Hegazi](https://github.com/farahhegazi)
- [Fengfan Bian](https://github.com/Fyfe-c)

Acknowledgements to:  
 - [Matt Graham]([https://github.com/tsusdere](https://twitter.com/mattgraham)) for their template that I used on my site.
 - To Andrew Etter, for his book 'Modern Technical Writing'

## FAQs

### 1. Why is Markdown preferable to a word processor?

Markdown stands out for its technical prowess and ease of use.

#### Ease of Use
- **Simplified Syntax:** Markdown employs a straightforward syntax, relying on symbols rather than complex formatting options. It streamlines the writing process by minimizing the learning curve.
- **Universal Compatibility:** Markdown operates seamlessly across various text editors, ensuring consistent performance regardless of the platform. This universal compatibility fosters flexibility and independence from proprietary software.

#### Web Compatibility
- **HTML Conversion:** Markdown facilitates effortless conversion of plain text into HTML, enabling seamless integration with web publishing platforms. This feature simplifies the transition from document creation to online publication.
- **Extensibility:** Markdown's extensibility allows for the incorporation of additional features and customization options. Users can enhance their documents with supplementary functionalities, enhancing the richness and interactivity of their content.

### 2. Why isn't my resume displaying?

If your resume isn't visible, consider these troubleshooting steps:

- **Check Server Status:** Verify the operational status of the GitHub servers to ensure uninterrupted service. Temporary disruptions or maintenance activities may impact accessibility.
- **Validate URL:** Review the accuracy of the resume's URL, ensuring alignment with the designated link in the GitHub repository settings. Inaccurate URLs can lead to accessibility issues and hinder visibility.
- **Branch Configuration:** Confirm the selection of the appropriate branch for website deployment within the repository settings. Accurate branch selection is crucial for reflecting updates and changes on the live site effectively.



[^1]: Andrew Etter - Modern Technical Writing, 39  
[^2]: Andrew Etter - Modern Technical Writing, 33  
[^3]: Andrew Etter - Modern Technical Writing, 46  
[^4]: Andrew Etter - Modern Technical Writing, 52  
[^5]: Andrew Etter - Modern Technical Writing, 51  
