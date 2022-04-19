---
layout: post
title:  "Hosting your Site on GitHub"
date:   2022-04-16 12:00:00 -0700
categories: user-guides
---

This portfolio is hosted on Github and built in Jekyll. GitHub is an excellent (and free!) way to host your own website. This guide walks you through the steps to host your Jekyll site on GitHub using Atom.

# Prerequisites
* A GitHub account
* A Jekyll website that you have successfully built and deployed locally
* Atom installed on your device

# Intializing the GitHub Repository in Atom
1. Go to **File > Open Folder...**
2. Navigate to the folder where your project is located. Click **Select Folder**.
3. Click the GitHub logo at the bottom of the Atom window. Two tabs should appear: a Git tab and a GitHub tab.
![The GitHub button](/images/initial_screenshot.png "GitHub button")
4. In the GitHub tab, click the button that says "Initialize and publish on GitHub".
![Initialize and publish your repository](/images/initialize_and_publish.png "Initialize and Publish")
5. In the window that appears, name your repository username.github.io. You must follow this naming convention for the site to work. Notice that the name of this site is ghanvik.github.io, since my username is ghanvik.
![Publish window](/images/Publish.png "Publish")

# Pushing your Site to the Remote Repository
1. Open the Git tab.
2. Click "Stage All".
![Stage all](/images/Stage_all.png "Stage all changes")
3. Add a commit message that says "Initial commit" and click "Create detached commit".
4. Click "Publish" on the bottom of the window. This will be right next to the GitHub button you clicked earlier.

In your web browser, you should now be able to go to username.github.io and see your site live!
