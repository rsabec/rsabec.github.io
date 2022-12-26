---
layout: post
title:  "Create and Update Jekyll Posts"
date:   2022-11-24 20:51:00 -0800
categories: personal website hosting jekyll 
---

Updating or adding to your posts in Jeckyll is done with the 'markdown' files located in the '\_posts' directory in your Jeckll site.
Find and open an existing post - Copy and 'save as' to create a new post.

Documentation - <a href="https://jekyllrb.com/docs/posts/">https://jekyllrb.com/docs/posts/</a>


Open Terminal and change your directory to the jekyll site saved locally on your localhost. <br>
>Example for my setup ( yours will have different path/filename )<br>
```terminal
cd Documents/GitHub/rsabec.github.io/
```

Update the file contents: Text formatting links below.
* Quick [reference](http://simpleprimate.com/blog/markdown-basics) to formatting
* How to format [code](https://stackoverflow.com/questions/51313127/jekyll-inserting-extra-code-when-generating-blog-posts) snippets.


Run the command from that directory to compile and run your site locally to test - <br>
>
```terminal
bundle exec jekyll serve
```

 <br>

Documentation:
* [bundle]( https://jekyllrb.com/tutorials/using-jekyll-with-bundler/)
* [stackoverflow](https://stackoverflow.com/questions/51157446/whats-the-difference-between-bundle-exec-jekyll-serve-and-jekyll-serve)

You can then test your site locally - typically this address will be http://127.0.0.1:4000/ <br>

Commit your changes to Github and retest:
* Github [Desktop](https://desktop.github.com/ )<br>



Setting up `jekyll` and `GitHub Pages` only required basic programming skills and beginner Github experience.  I would recommend using GitHub Pages for your personal site.


[Github]( https://pages.github.com/ ) pages <br>
[Jekyll]( https://github.com/jekyll/jekyll ) Github repo <br>
[Jekyll]( https://jekyllrb.com/ ) website
