---
layout: post
title: Customizing a Jekyll blog
date: 2019-12-04
tags: tutorial, blogging
---

# Customizing a Jekyll blog

The hard part isn't getting started. WHY DOES IT LOOK SO UGLY.
I tried to change the theme by following these [instructions](https://help.github.com/en/github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-with-the-theme-chooser) from the Github Help section, but it still looked exactly the same to me.

## Liquid Templating

There are two main concepts when using Liquid: front matter and tags. [Jekyll documentation](https://jekyllrb.com/docs/liquid/)

### Front Matter

Each post should have something called Front Matter at the top between triple-dashed lines. These are predefined/custom variables such as date or tags. [Read more from the documentation.](https://jekyllrb.com/docs/front-matter/)

#### Example: Adding another Front Matter variable, "tags"

Add tags to your blog post's Front Matter.
Edit `/_layouts/post.html` 

```
<div class="tags">
  Tags: {{ page.tags }}
</div>
```

### Liquid template tags


Not to be confused with the above tag variable, Liquid template tags allow for each of your pages/posts to be dynamic even though the framework is static. That means, if you add a new blog post, you don't have to change the default layout or post layout in order for your new post to show up. Github Pages builds your site again and then your new post appears auto-magically!

1. Output dynamic content

2. Coditional statements and loops

See "Liquid Templating" section from this [tutorial](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/).

### Difference between pages and posts

#### Default.html

Pages are static pages and posts are your blog entries derived from the `_post` directory. 
In the `_layouts` directory, there is a `post.html` and `post.html` with the layout Front Matter variable set to `default`. This means that both pages and posts depend on `default.html`.

Around line 29 of `/_layouts/default.html`, there should be an HTML tag called `nav`. That's the navigation toolbar (Blog, About) found at the top of your website. I prefer it the opposite way (About, Blog) so I just swapped the two lines. Simple!



