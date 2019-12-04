---
layout: post
title: Starting a blog
date: 2019-12-03
tags: tutorial
---

# Starting a blog

After procrastinating on starting a blog for years, I finally decided to use Github Pages. That way, I could use version control I'm already familiar with. As a static site hosting service, Github recommends Jekyll and even though I had never used it before, it only took me 30 minutes to get started!

I did have to spend some more time familiarizing myself with the specifics of Markdown (my prior knowledge is elementary and I still keep mixing up which brackets to use for links) but this [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) includes all of the basics.

Based on this [tutorial](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/), I wrote the below TLDR version. Please do be sure to at least skim the tutorial as it has tips I didn't include, useful pictures, and other optional steps. 

### Directions

1. Fork the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) from GitHub

2. Rename your repository to *username.github.io*

   Note: Your site might not be published yet (it should be after step 3, or after commiting any changes within your repository)
   
3. Personalize the `_config.yml`

4. Edit `/_posts/2014-3-3-Hello-World.md` and update the date and title of your post. Your website should be rebuilt automatically so that the `READ MORE` link points to your first post.
   
   Note: Jekyll follows the following naming convention: `YEAR-MONTH-DAY-title.md` where `YEAR` is four digits and `MONTH` and `DAY` are both two digits. Be sure to update the information between the three dashes - that's the [Front Matter](https://jekyllrb.com/docs/front-matter/) and where you can set predefined/custom variables such as date or tags.

DONE!

### More steps

* Choose a [theme](https://help.github.com/en/github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-with-the-theme-chooser)


### Other useful resources:

* <https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll>
* <https://help.github.com/en/github/working-with-github-pages/getting-started-with-github-pages>
* <https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site>
* <https://help.github.com/en/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site>
* <https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>
