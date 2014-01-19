---
title: Getting Involved
layout: default
---

## Get involved with the dis-orientation collective

Below, we aim to present a comprehensive guide as to how to get involved with the dis-orientation collective. 

The dis-orientation collective and its web presence at `dis-orientation.info` is a collaboration between individuals at a wide variety of universities. As such, the content on this website is not homogenous. Although the content is not necessarily homogenous, we are all committed to bringing to the fore systemic issues with universities by disrupting the normal narrative that unversities tell with dis-orienting information. To learn more about us, you should read our [about page](http://dis-orientation.info/about). 

Below, we will focus on how to get involved if your university isn't already involved.

### <a id="toc">Table of (dis)contents</a>

- <a href="#step-1">Step 1: Getting in touch</a>

- <a href="#step-2">Step 2: Getting your subdomain set up</a>

	- <a href="#why-github">Why GitHub? Why not something that might be a little easier to get set up, like Wordpress?</a>
	
- <a href="#step-3">Step 3: Using GitHub</a>

	- <a href="#web-interface">GitHub's web interface</a>
	
	- <a href="#software">GitHub's software application</a>
	
		- <a href="#mac">On a Mac computer</a>
		
		- <a href="#windows">On a Windows computer</a>
		
	- <a href="#github-summary">GitHub: Recap and summary</a>
		
- <a href="#step-4">Step 4: Writing dis-orienting content with Jekyll</a>

	- <a href="#default-layouts">Default layouts</a>
	
	- <a href="#markdown">Markdown</a>
	
	- <a href="#further-customization">Further customization</a>

- <a href="#step-5">Step 5: Un-learn and dis-orient!</a>

### <a id="step-1">Step 1: Getting in touch</a><a href="#toc">↩</a>

If your university is in the [list of universities](http://dis-orientation.info/universities) that already have content on our website, you should click on the link to visit their part of this website. There, they will have contact information, and you can get in touch with the folks at your university that are already working on dis-orienting information.

If you do not see your university listed, please get in touch with us by [contacting us](http://dis-orientation.info/contact) in order to get space on `dis-orientation.info`. Below, we will walk you through how to set up that space, how to manage it, and how to post content to it.

### <a id="step-2">Step 2: Getting your subdomain set up</a><a href="#toc">↩</a>

`dis-orientation.info` provides each university with its own subdomain in order for them to have space to post their own content. A subdomain indicates the first half of a web address. So, in `xyz.dis-orientation.info`, `xyz` is the subdomain part, and `dis-orientation.info` is the main domain name.

In terms of setting up your subdomain, most of the initial heavy lifting will be done by us, the dis-orientation collective. What is important to know is that our website is hosted using a service called GitHub. GitHub is a hosting service combined with a version control system, which is basically a software service that tracks changes to documents.

#### <a id="why-github">Why GitHub? Why not something that might be a little easier to set up, like Wordpress?</a><a href="#toc">↩</a>

There are a few reasons why we chose to host this project on GitHub.

1. First and foremost, GitHub provides free hosting. When setting up a website, there are usually two key aspects to doing so: (i) purchasing a domain name (something like `example.com`) and (ii) paying for someone to store the files that generate your website on a server that is connected to the internet. Since GitHub provides free hosting, the only thing we have to do is pay for the domain name, `dis-orientation.info`, reducing the cost to maintain this project.

1. Second, GitHub inherently employs a version control system. This allows us to run the website in a de-centralized manner, while still having a high degree of transparency and accountability. GitHub allows its users to see all of the changes that have been made to files, who made those changes, and when they were made. (It also allows us to revert to older versions of those files, which, practically speaking, is a great provision in case of accidental deletion of any of the website files!) The dis-orientation collective highly values transparency (after all, we're trying to make universities more transparent by airing dirty laundry that they otherwise hide with their narratives), and so using GitHub provides transparency within our collective itself by allowing all of our contributors to see who made which changes. It also easily allows us to have many universities contribute content, without necessarily having to coordinate with every other university that is involved with the collective, which we would have to do if we were sharing one Wordpress account.

1. Finally, once you've made it over the first hurdle of getting everything set up, GitHub hosting provides a really easy way to write content that is very straightforward to learn.

So, after finishing up the details of how to get your subdomain set up, we will walk you through how to use GitHub and how to write content, using the tools provided by GitHub. From then on, you're free to do whatever you wish with your subdomain, so long as it contributes to dis-orienting and un-learning and so long as it does not violate any of the values and policies of our collective, as detailed in our [about page](http://dis-orientation.info/about).

First, though, we need to finish getting your subdomain set up. As mentioned above, we will do the heavy lifting in order to get your subdomain initially set up. Since the project will be hosted on GitHub, this requires telling our domain name registrar (the company managing our domain name, `dis-orientation.info`, to point the new subdomain in the direction of GitHub's servers).

On GitHub, all parts of this website are hosted under an umbrella organization GitHub account called [`dis-orientation`](https://github.com/dis-orientation). If you visit that link, you will notice that there is a "repository" for each subdomain, as well as a repository for the main portion of the website.

We will create a new repository (or "repo", for short) for your university. While we do this, you will need to [create a GitHub account](https://github.com/join). Once we have the new repo set up and have told our domain name registrar to point to that repo on GitHub, we will then add your newly created GitHub account to be a collaborator for the repo for your university. (You can read more about how GitHub organization accounts work [here](https://github.com/blog/674-introducing-organizations).)

The great part about this is that we can add as many collaborators to a repo as we want. So, for everyone that is part of your dis-orientation group at your university, they can have their own GitHub account and be a collaborator for your university's repo. Just be sure to let us know what all of the GitHub accounts are that we need to add as collaborators to your new repo!

Now that we have your subdomain set up, we will next go over how to work with GitHub. After that, we will go over how to write content, and then we will send you on your merry un-learning and dis-orienting way!

### <a id="step-3">Step 3: Using GitHub</a><a href="#toc">↩</a>

Broadly speaking, there are two straightforward ways to use GitHub. One of these ways is directly through their website interface, while the other way uses free software that synchronizes the repo on their website with a "clone" of that repo that is stored directly on your computer. If you use the software version, you will then be able to edit the website directly on your computer without an internet connection. After you finish editing the website, all you will need to do is find an internet connection and synchronize the changes that you made on your computer with version of the repo stored on GitHub. (You can also do things from the command line, but we will not cover that here. If you're interested in this option, try poking around the internet for tutorials, if you don't already know how to use Git from the command line.)

Here, we will go over both the web interface option and the software application option.

#### <a id="web-interface">GitHub's web interface</a><a href="#toc">↩</a>

Once you have told us your GitHub account and we have added you to the `dis-orientation` account, you should see a grey box in the top left of `https://github.com`, like so:

<img alt="git-web-interface" width="400" src="/images/git-web-interface.png" style="display:block; margin:0 auto;" />

Clicking on this will allow you to switch to the `dis-orientation` account context. Clicking on `dis-orientation` will bring you to a page where you can see your repo on the right of the screen. Click on the repo for your university:

<img alt="git-web-find-repo" width="400" src="/images/git-web-find-repo.png" style="display:block; margin:0 auto;" />

After you click on this repo, you will be taken to the GitHub page for where the files are stored. (A way to get here that might be quicker is to navigate directly to `https://github.com/dis-orientation/xyz` in your browser, replacing `xyz` with the name of your subdomain.)

GitHub is set up so that each repository can have different "branches". When we tell our domain name registrar to send your subdomain towards GitHub, GitHub displays a special branch of the repository, called `gh-pages`. **Therefore, to edit any of the content on the website, you need to switch to the `gh-pages` branch**. (Odd as it may seem, the "master" branch will never be relevant for editing your website.)

<img alt="git-web-change-branch" width="400" src="/images/git-web-change-branch.png" style="display:block; margin:0 auto;" />

As you can see above, you can change to the `gh-pages` branch by clicking on the dropdown arrow for the branches. Now you should see all of the content of your website.

If you click on a file (for example, `contact.md`), you will see this screen, where you can click on "edit" to edit the file. (Here, you can also look at the history of all changes made to this file and delete the file, using the appropriate buttons.)

<img alt="git-web-edit" width="400" src="/images/git-web-edit.png" style="display:block; margin:0 auto;" />

After you make a change, in order to save that change, you need to "commit" the change. You can do so at the bottom of the screen. You can enter an extensive description of what change you made (and why), if you would like to do so. That information is stored in the history of the file, so that your collaborators know what changes were made and why. You do not necessarily need to enter an extensive description of the change you made, but it is required that you at least enter some description explaining the change.

<img alt="git-web-commit" width="400" src="/images/git-web-commit.png" style="display:block; margin:0 auto;" />

This method of editing the files for your website works well when you have an internet connection and when you are only working with files that have text in them. The web interface on GitHub, however, is not great for uploading pictures, for example. Doing things like this and also being able to work on your part of the website when you are not connected to the internet are the benefits of using the GitHub software application. We will provide an overview of how to use this software client next.

#### <a id="software">GitHub's software application</a><a href="#toc">↩</a>

First, you will need to download the GitHub's native software application. It can be downloaded [here](https://help.github.com/articles/set-up-git). The website should automatically display the correct version of the software for your operating system, but if it does not, there are links at the top of page for each operating system. Click on the correct one:

<img alt="git-software-os" width="400" src="/images/git-software-os.png" style="display:block; margin:0 auto;" />

##### <a id="mac">On a Mac computer</a><a href="#toc">↩</a>

After you have downloaded and installed the software, you will be asked to enter the username and password that you set up for GitHub. Once we have added you to the `dis-orientation` GitHub account, you should see a dashboard screen that looks like this, with `dis-orientation` on the left:

<img alt="git-mac-clone" width="400" src="/images/git-mac-clone.png" style="display:block; margin:0 auto;" />

After you click on `dis-orientation` on the left side of the screen, you can also click on the repository for your university to "clone" this repo to your computer. Cloning a repo to your computer creates a version that is stored and saved directly on your computer. You will be asked where you wish to save this repo and what you wish to call it. Choose a name and a place on your computer that is convenient for you.

Next, you can click on "My Repositories" to see a list of the repositories that you have cloned on your computer, and you can click on the repo for your university:

<img alt="git-mac-myrepos" width="400" src="/images/git-mac-myrepos.png" style="display:block; margin:0 auto;" />

After clicking on your repo for your university, you will see a screen where you can see the history of all changes made to this repository, a list of any current changes you have made, and the different branches of the repository. If you ever need to get back to the main dashboard in order to clone another repository, you can click on "Repositories" in the top left corner.

<img alt="git-mac-repo" width="400" src="/images/git-mac-repo.png" style="display:block; margin:0 auto;" />

The first thing you will need to do is change to the `gh-pages` branch. As noted above, the only branch that will ever be relevant is the `gh-pages` branch because this is what GitHub uses to display website content. So, you will always want to make sure that you're repository is set to the `gh-pages` branch, which you can do by clicking on "Branches" in the sidebar and then by clicking on the checkmark next to the `gh-pages` branch.

<img alt="git-mac-branch" width="400" src="/images/git-mac-branch.png" style="display:block; margin:0 auto;" />

Now that you have switched to the `gh-pages` branch, you can navigate to the folder where you cloned this repo on your computer, and you will be able to see all of the files. This allows you to add things like images and PDF files to your repository, which is something that you **cannot** do on the GitHub web interface, since there is no "upload" button on the GitHub website.

So, if you want to upload a PDF version of one of your university's disorientation guides, you can, for example, create a folder inside of the repo called "xyz-dogs", and then you can copy a PDF file into this folder:

<img alt="git-mac-pdf" width="400" src="/images/git-mac-pdf.png" style="display:block; margin:0 auto;" />

Before this change will take effect online, however, you have to do two things. First, just like with the web interface, you have to enter a description of your change and "commit" it. To do this, go to the dashboard for your repo in the GitHub application and click on the "Changes" tab in the sidebar. On the right side, you will see the changes that were made. In this case, we see the cover of the PDF that was uploaded. Next, enter a description of the change on the left, and click "Commit".

<img alt="git-mac-commit" width="400" src="/images/git-mac-commit.png" style="display:block; margin:0 auto;" />

Finally, the last step is to sync the changes that you made with the version of the repository on your computer to the version of the repository that is stored on GitHub's servers. To do this, click on "Sync" button that appears after you "Commit" the change.

<img alt="git-mac-sync" width="400" src="/images/git-mac-sync.png" style="display:block; margin:0 auto;" />

This last step must be done when you have internet connection. So, other than this last step, you can edit your website without an internet connection. Then, when you can connect to the internet, you can sync your changes.

Overall, that's the way to work with the GitHub software for Mac. Next, we'll go over the Windows version of the software, before moving on to how to edit your website files.

##### <a id="windows">On a Windows computer</a><a href="#toc">↩</a>

As with the Mac software, after you have downloaded and installed the Windows software, you will be asked to enter the username and password that you set up for GitHub. Once we have added you to the `dis-orientation` GitHub account, you should see a dashboard screen that looks like this, with `dis-orientation` on the left:

<img alt="git-windows-clone" width="400" src="/images/git-windows-clone.png" style="display:block; margin:0 auto;" />

After you click on `dis-orientation` on the left side of the screen, you can then click on the repository for your university to "clone" this repo to your computer. Cloning a repo to your computer creates a version that is stored and saved directly on your computer. The Windows version of the software has a default location that it puts all cloned repos on your computer. You can change this by navigating to "Tools > Options" and changing the default storage directory, if you would like. Otherwise, the default storage directory will probably be `C:\Documents\GitHub`, or something similar.

Next, you can click on "repositories" under the "local" heading to see a list of all of the repositories that you have cloned on your computer, and you can click on the repo for your university:

IMAGE IS MISSING. WILL BE HERE SOON.

<!--
<img alt="git-windows-myrepos" width="400" src="/images/git-windows-myrepos.png" style="display:block; margin:0 auto;" />
-->

The first thing you will need to do is change to the `gh-pages` branch. As noted above, the only branch that will ever be relevant is the `gh-pages` branch because this is what GitHub uses to display website content. So, you will always want to make sure that you're repository is set to the `gh-pages` branch. After you have clicked on the local repo for your university, you can do this by then clicking on the branch symbol in the top right that says master next to it. A menu will appear, and you want to select the `gh-pages` branch:

<img alt="git-windows-branch" width="400" src="/images/git-windows-branch.png" style="display:block; margin:0 auto;" />

Now that you have switched to the `gh-pages` branch, you can navigate to the folder where the cloned version of the repo is stored on your computer. Remember that this is the folder that is listed as the default storage directory location under "Tools > Options". Here, you will be able to see all of the files for your part of the website. Moreover, this allows you to add things like images and PDF files to your repository, which is something that you **cannot** do on the GitHub web interface, since there is no "upload" button on the GitHub website.

So, if you want to upload a PDF version of one of your university's disorientation guides, you can, for example, create a folder inside of the repo called "xyz-dogs", and then you can copy a PDF file into this folder:

IMAGE IS MISSING. WILL BE HERE SOON.

<!--
<img alt="git-mac-pdf" width="400" src="/images/git-mac-pdf.png" style="display:block; margin:0 auto;" />
-->

Before this change will take effect online, however, you have to do two things. First, just like with the web interface, you have to enter a description of your change and "commit" it. To do this, you just have to be viewing the local version of the repo inside the GitHub application. Any chances you make will automatically appear, and there will be a box in the upper left corner for you to write your description and commit the changes, by clicking "commit to gh-pages" after you enter your description.

IMAGE IS MISSING. WILL BE HERE SOON.

<!--
<img alt="git-windows-commit" width="400" src="/images/git-windows-commit.png" style="display:block; margin:0 auto;" />
-->

Finally, the last step is to sync the changes that you made with the version of the repository on your computer to the version of the repository that is stored on GitHub's servers. To do this, click on "sync" button in the top right corner of the screen, next to the "branches" button. After you have "committed" a change, you will see a blue button appear with the number of commits that you have made that you have not yet synchronized. In this case, there is only 1 commit that has yet to be synchronized.

IMAGE IS MISSING. WILL BE HERE SOON.

<!--
<img alt="git-windows-sync" width="400" src="/images/git-windows-sync.png" style="display:block; margin:0 auto;" />
-->

As with the Mac version, this last step with the Windows version of the software must also be done when you have internet connection. But, other than this last step, you can edit your website without an internet connection. Then, when you can connect to the internet, you can sync your changes.

Overall, that's the way to work with the GitHub software for Windows. After a brief recap that highlights the important points, we'll move on to how to edit your website files!

#### <a id="github-summary">GitHub: Recap and summary</a><a href="#toc">↩</a>

To briefly recap and summarize, there are a few important things to remember when working with your part of the website using GitHub, regardless of whether you're doing this via the web interface or the software application for Windows or Mac. First, you want to make sure that you are always editing the files in the `gh-pages` branch, **not the master branch**. Second, whenever you make a change, you need to briefly describe the change and "commit" the change, in order for it to be saved. Third, if you're editing the files on your computer, after committing a change, you need to "sync" it with the repository on GitHub's servers. Finally, if you use the software client and not the web interface, **it is best practice that you always "sync" the clone of the repo on your computer with the version that is stored online on GithHub's servers _before you begin editing_**. This is because other folks that you work with might have made changes to your website that will not be reflected in the clone on your computer until you sync it. You can do this by clicking "Sync Branch" in the top right of the Mac software client and "Sync" in the top right of the Windows software client.

And that's it. Those are the three main steps to working with GitHub. Next, we'll look at *how* to edit the website files themselves.

### <a id="step-4">Step 4: Writing dis-orienting content with Jekyll</a><a href="#toc">↩</a>

As some basic background information, basic websites are basically just a collection of HTML files. Browsers like Firefox and Google Chrome have instructions for how to display these HTML files. But, underneath it all is just a collection of text files. Now, HTML isn't necessarily the easiest thing to learn, but one of the thing that's nice about GitHub (and this is one of the reasons we chose to use GitHub) is that you can write website content in a really simple computer language called Markdown. GitHub uses a program called [Jekyll](http://jekyllrb.com/) to automatically convert the Markdown files into HTML to be displayed as your website. If you want to significantly change the appearance and layout of your part of the website, you will likely have to learn some HTML and CSS, or we can also work with you to help you change the layout how you would like. (If you would like to learn some HTML and CSS, [W3Schools](http://www.w3schools.com/) is a great way to do this. And if you need our help with something, don't hesitate to [contact us](http://dis-orientation.info/contact)!)

Nonetheless, we have aimed to set things up so that you can get to editing your subdomain straight away after learning some basic Markdown, something that should hopefully take no more than 30 minutes or so. This section of the getting involved page, then, covers three things. First, we will go over a few different default layouts that we can set up for you. Then, we will look at Markdown briefly. Finally, we will discuss a bit of what would be needed to further customize the design and layout of your subdomain.

#### <a id="default-layouts">Default layouts</a><a href="#toc">↩</a>

#### <a id="markdown">Markdown</a><a href="#toc">↩</a>

#### <a id="further-customization">Further customization</a><a href="#toc">↩</a>

### <a id="step-5">Step 5: Un-learn and dis-orient!</a><a href="#toc">↩</a>

- **Details coming soon**
