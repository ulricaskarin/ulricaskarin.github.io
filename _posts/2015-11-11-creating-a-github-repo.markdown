---
layout: post
title:  "Creating a GitHub repo"
date:   2015-11-11 20:32:15
category: github

image: ulricaskarin.github.io/assets/images/git_book.png
type: article
description: When I created my first basic GitHub repo

author: Ulrica Skarin
comments: true
published: true
---

I first learned about git and GitHub this fall (2015) when I started my studies at the Linnaeus University. We have
used it to version control our code exercises as well as code tests, cloning repos that already existed. I quickly
learned all the basic commands such as ```git add``` ```git push``` and so on, but really not much deeper than that.
Today I made a first change to that, and as simple as it might sound - I am so glad I went through with it.

I created my first basic test repo - a cookbook - and it wasn't at all complicated!

Logged in at my github account I went to the **repositories tab**, clicked on the button that says **"new"**. I chose the name
"cookbook" for my new repo and added a short description. I also initialized a README file before I went back to my
local terminal in order to clone the repo:

 ```git clone https://github.com/<username>/<repositoryname>.git```

This command resulted in a new cookbook folder containing a *downloaded copy of my repository*. Inside the folder I found
the README file that I created when initializing the repo. I then added a new branch (christmas) with the command ```git checkout -b christmas```
and added two new files to it, a recipe of [delicious treats][delicious treats] ... (yum) and a recipe of [lussebuns][lussebuns]. I will continue to
add different category recipes to my "cookbook", but as for now - I am mostly happy that I took my first step of some
self exploring inside git and GitHub.

For those of you who would like to learn more about git and GitHub, I strongly recommend the book by *Ferdinando Santacroce*:
[Git Essentials][Git Essentials]. Well worth the read!

![Open Graph Logo]({{ site.url }}/assets/images/git_book.png){: .post-image }

> GIT according to Linus Torvalds: You’re in a good mood, and it actually works for you. Angels sing and light suddenly fills the room.

[delicious treats]:https://github.com/ulricaskarin/cookbook/blob/Christmas/Delicious-Treats.md
[lussebuns]:https://github.com/ulricaskarin/cookbook/blob/Christmas/Lussebuns.md
[Git Essentials]:http://www.amazon.com/Git-Essentials-Ferdinando-Santacroce/dp/1785287907
