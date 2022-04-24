---
layout: post
title:  "Hosting your Site on GitHub"
date:   2022-04-16 12:00:00 -0700
categories: user-guides
---

This portfolio is hosted on GitHub and built in Jekyll. GitHub is an excellent (and free!) way to host your own static site. This guide walks you through the steps to host your Jekyll site on GitHub using Atom. This guide assumes that you do NOT already have a git repository for your project.

# Prerequisites
* A GitHub account
* A Jekyll website that you have successfully built and deployed locally
* Atom installed on your device

# Logging into GitHub in Atom using OAuth
1. Open Atom
2. Click the GitHub logo at the bottom of the Atom window. Two tabs should appear on the right: a Git tab and a GitHub tab.
![The GitHub button](/images/initial_screenshot.png "GitHub button")
3. If you are not already logged into GitHub, click **Login** and the window should then say **Enter Token**
4. Visit [github.atom.io/login](github.atom.io/login) and click **Authorize Atom**.
5. If you are not logged in to GitHub, you will be taken to a sign in page. Go ahead and sign in.
6. Copy the token that shows up on the next page and paste it into the GitHub window in Atom

# Initializing the GitHub Repository in Atom
1. Go to **File > Open Folder...**
2. Navigate to the folder where your project is located. Click **Select Folder**.
3. In the GitHub tab, click the button that says **Initialize and publish on GitHub**.
![Initialize and publish your repository](/images/initialize_and_publish.png "Initialize and Publish")
4. In the window that appears, name your repository username.github.io. You must follow this naming convention for the site to work. Notice that the URL of this site is ghanvik.github.io, since my username is ghanvik.
![Publish window](/images/Publish.png "Publish")

# Pushing your Site to the Remote Repository
1. Open the Git tab.
2. Click **Stage All**.
![Stage all](/images/Stage_all.png "Stage all changes")
3. Add a commit message that says "Initial commit" and click "Create detached commit".
4. Click **Publish** on the bottom of the window. This will be right next to the GitHub button you clicked earlier.

In your web browser, you should now be able to go to username.github.io and see your site live!
