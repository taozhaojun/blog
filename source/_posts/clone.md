---
title: Cloning and Working on Your Hexo Project on a New Computer
date: 2023-11-09 08:42:51
tags: github
---

Transitioning to a new computer and want to continue working on your Hexo blog? No problem! Here's a straightforward guide to get you up and running in no time.

<!-- more -->

## Getting Started

Before you begin, make sure that the new computer has Git, Node.js, and npm installed. These are essential for running and maintaining Hexo projects.

### Step 1: Install Git

Download and install Git from [git-scm.com](https://git-scm.com/). Git is a version control system that lets you manage and keep track of your source code history.

### Step 2: Install Node.js and npm

Hexo is a static site generator built on Node.js. Grab the latest version of Node.js, which includes npm, from [nodejs.org](https://nodejs.org/).

## Clone Your Project

With the prerequisites out of the way, it's time to bring your project to the new machine.

### Step 3: Clone the Repository

Open your command line tool and clone your Hexo project from GitHub with the following command:

```sh
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to your project directory:

```sh
cd your-repository-name
```

### Step 4: Install Dependencies

Within the project directory, run:

```sh
npm install
```

This command installs all the necessary dependencies listed in your project's `package.json` file.

## Fire Up Your Blog

Now, let’s see your blog in action.

### Step 5: Run Hexo Server

Execute:

```sh
hexo server
```

Check out your blog at `http://localhost:4000` and ensure everything looks good.

## Keep on Blogging

You're all set! Continue creating content, tweaking your theme, or whatever else your blog needs.

### Step 6: Commit Your Changes

After making some changes, don't forget to commit them:

```sh
git add .
git commit -m "Describe your changes here"
```

### Step 7: Push to GitHub

Keep your remote repository updated:

```sh
git push origin master
```

And that's it! You're now ready to continue your blogging journey on your new computer.

Remember, consistency is key in blogging and version control. Happy blogging!
