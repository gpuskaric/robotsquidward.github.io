---
layout: post
title: "Painfully Simple Jekyll Sites"
description: "A *painfully* simple guide for how to build a blog or website in 10 minutes using Jekyll and GitHub Pages."
date: 2018-02-06
tags: [jekyll, blogging, github, pages, web development, jekyll-guides]
comments: false
share: false
---

Everybody wants to have a website.  A lot less people realize how easy it is to get started.  Lucky you, I'm going to show you exactly how you can get started with a live website in less than 10 minutes - for free!

We're going to build our site using [GitHub Pages](https://pages.github.com/).  GitHub harnesses the power of [Jekyll](https://jekyllrb.com/) to turn [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) documents into lovely websites.

## Create a New Repository on [GitHub](https://github.com/)

If you don't have an account [sign up for free](https://github.com/join).

Once you have an account, go back to the [GitHub landing page](https://github.com/), click on the (+) dropdown and select New repository.

![new repo](/images/jekyll-tutorial-01.png)

Add a repository title, optional description, and make sure you check the box next to 'Initialize this repository with a README'.

![repo details](/images/jekyll-tutorial-02.png)

## Generate Your Site

After your repository is created, go to the **Settings** tab and scroll down to the **GitHub Pages** section.

Here, you turn on GitHub Pages by selecting the branch you want GitHub to build your site from.  We want to build our site from our repository's `master` branch.

![settings](/images/jekyll-tutorial-04.png)

This will prompt GitHub to start building your site.  At the top of the **GitHub Pages** section you'll see the url GitHub will publish your site to.

![published url](/images/jekyll-tutorial-05.png)

If you preview the site now, it will just be a prettified-version of your README.  This is the essence of the Jekyll blog.  But we want our site to have a bit more pizzaz, so we're going to pick a theme.

## Pick A Theme

Click on **Choose a theme** button under the **Theme Chooser** section.

Here, we can select any theme for our site.  Most built-in Jekyll themes in GitHub Pages offer us a simple UI boost for our README, so choose whichever one you like the best.  For my basic site I'm picking the **Minimal** theme.

![theme chooser](/images/jekyll-tutorial-06.png)

Now we can check out our site (*from that link in the Settings page*).  Here's what mine looks like.

![generated site](/images/jekyll-tutorial-07.png)

## Update Site Content

The **Minimal** theme is just that - minimal.  All you have to do to update your site content is update your `README.md` file.

I'm just going to add a couple of my own posts to my 'blog'.

![update readme](/images/jekyll-tutorial-08.png)

When you're done updating, click on the **Commit changes** button to save your updates.  Your changes should be updated almost immediately.  Here's what mine look like.

![updated site](/images/jekyll-tutorial-09.png)

And that's pretty much it!  You have a live site and blank slate for your updates!

## What's Next?

You just published a site in less than 10 minutes!  But we just scratched the surface of the possibilities of Jekyll and GitHub Pages.  Here's some resources to get you on to your next site.

### Jekyll Docs

* [Quick-Start](https://jekyllrb.com/docs/quickstart/)
* [More on GitHub Pages](https://jekyllrb.com/docs/github-pages/)
* [Additional Resources](https://jekyllrb.com/docs/resources/)

### Themes

I like themes from [CloudCannon](https://cloudcannon.com/announcements/2016/12/05/free-jekyll-templates/) which are all available on their [GitHub profile](https://github.com/CloudCannon).

If you like my theme, check it out [here](https://github.com/aweekj/Kiko-plus).  *Fair warning - this theme is deprecated.*
