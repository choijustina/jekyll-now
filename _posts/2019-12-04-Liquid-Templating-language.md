---
layout: post
title: Liquid Templating language
date: 2019-12-04
tags: tutorial, blogging
---

See Jekyll documentation on [Liquid](https://jekyllrb.com/docs/liquid/) and a list of Liquid variables available [here](https://jekyllrb.com/docs/variables/).

### Front Matter

Each post should have something called Front Matter at the top between triple-dashed lines. These are predefined/custom variables such as the title or date. [Read more from the documentation.](https://jekyllrb.com/docs/front-matter/)

### Liquid templating

Liquid templating allows for each of your pages/posts to be dynamic even though the Jekyll framework is static. That means, if you add a new blog post, you don't have to change the default layout or post layout in order for your new post to show up. Jekyll uses the global variables or Front Matter variables to update other parts of your website. Github Pages builds your site again and then your new post appears auto-magically!

1. Objects 

Output content

2. Tags

Conditional statements and loops

3. Filters

More information: 
* <https://jekyllrb.com/docs/step-by-step/02-liquid/>
* "Liquid Templating" section from this tutorial <https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/).>

#### Example: Adding tags to each blog post

Add tags to your blog post's Front Matter in between the triple dashes. For example, this post's Front Matter looks like (missing the triple dashes):

```
layout: post
title: Customizing a Jekyll blog
date: 2019-12-04
tags: tutorial, blogging
```

Then, edit `/_layouts/post.html` using the Liquid templating language to include `page.tags`:

```
<div class="tags">
  Tags: {{ page.tags }}
</div>
```
