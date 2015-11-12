---
layout: post
title:  "Implementing comments"
date:   2015-11-10 15:15:00
category: programming

type: article
description: How I used disqus to implement comments in my blog

author: Ulrica Skarin
comments: true
published: true
---

*User interaction is good*. It gives the user an opportunity to leave feedback, ask for more information on an
article and so on. It is also good for me as the website owner - to get a feeling of how my fellow readers think and
feel. It gives me a chance to be a better developer.

It is not hard to integrate a disqus commentary field in your blog. All it takes is two simple steps:

- Register an account at [Disqus], fill in required fields and voilà! You're good to go.

- Grab the source code snippets that Disqus provides for you and put them where stated.

I created a commentary.html page for my disqus code (in my includes directory). I then included this page with a minimal code snippet
at the bottom of my post layout - where I wanted the commentary field to show up. I have also added some CSS to the
commentary field, just to adjust the width a little bit. In each blogposts front matter I have then implemented a tiny
little *comments tag* - which allows me to choose if I'd like the commentary field to show up or not. If I set this
to true - users are allowed to interact with me, otherwise not.

So. Go grab your own disqus - and don't forget to leave me a comment before you go ;-).

[Disqus]: https://disqus.com
