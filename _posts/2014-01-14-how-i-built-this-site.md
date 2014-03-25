---
layout: post
title: "How I build this site?"
modified: 2014-03-24 16:19:09 -0400
tags: [jekyll, pygments, rake]
image: 
  feature: post-2-pic.jpg
  credit: pic-jumbo
  creditlink: http://picjumbo.com/macbook-and-clutter/ 
comments: true 
share:  true
---
### Yes, I used Jekyll to build this site. If you haven’t used a static web generator to create a website before then here is one for you to try. 

My Goals for this site

1.  should be simple and fast
2.  should be able to blog without an internet connection
3.  should be responsive therefore it should look good on all devices
4.  should be easy to maintain and the only thing I need to do is to post articles
5.  should have clean CSS so that I can change the look and feel if I wish to do so

To achieve these goals, I used the following tools:

* Jekyll site generator in order to create a static web site that will be fast and easy to deploy.
* Bootstrap CSS and widgets for clean CSS and maintainability.
* Markdown along with Kramdown for text file formatting. This allows me to create my posts in almost plain text that gets converted to HTML.
* Pygments syntax highlighter
* Font Awesome for sprite icons.
* Rake build tool for build and deployment.
* Optipng image shrinker for making all my image files smaller and faster to load.

Jekyll is a blog aware static web generator which allows you to publish and maintain a blog by simplymanaging a folder of text files. It is simple to use and does not require any databases, complex javascript or HTML manipulation.

Apart from Jekyll, I also looked into a Python based static site generator, called Jinja. Looks interesting, however did not get enough time to play around with it.

It uses Markdown which is a simple text-toHTML conversion tool and the Liquid templating engine. If you use git hub to store your precious code then you are already familiar with Markdown syntax. Remember the Readme.md files that get automatically generated for you when you create a new repository in github?

The Jekyll asset bundler plaugin concatenates several javascript files into a single download. It only does this during a deployment build therefore while developing you will see all the individual files.

I am using Rake for very simple build tasks such as commit my changes and resync my remote github repository for this site, clean the last build, run the jekyll server and deploy the site toHeroku.

I am planning to use a lot of images for my blog in the future therefore I found this optipng tool to be quite useful for image optimization. My rake build scripts will scan for all images and automatically run optipng in order shrink the size of all images.

Finally, a word regarding hosting this blog, I initially used a hosting service provider but then migrated this site to Heruku. You can obviously use Github to host your site. Heruku by default does not seem to support static site hosting but a simple trick will make it think that this is a PHP site and your site will be hosted immediately. All you need to do is to insert a small .php file in your site, no need to put any PHP code inside this file.
