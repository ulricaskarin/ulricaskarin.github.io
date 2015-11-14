---
layout: post
title:  "Implementing comments"
date:   2015-11-10 15:15:00
category: programming

type: article
description: How I used disqus to implement comments in my blog

category: examination 1
author: Ulrica Skarin
comments: true
published: true
---

*This blogpost is part of an [examination assignment][examination assignment] at Linnaeus University.*

*User interaction is good*. It gives the user an opportunity to leave feedback, ask for more information on an
article and so on. It is also good for me as the website owner - to get a feeling of how my fellow readers think and
feel. It gives me a chance to be a better developer.

Disqus is a free service for comment support to websites. It is not hard to integrate a disqus commentary field in your blog.
All it takes is two simple steps:

- Register an account at [Disqus], fill in required fields.

- Grab the source code snippets that Disqus provides for you and you're good to go.

#### How I implemented comments on this website:
Following the two steps above, I then created a **commentary.html** page for my disqus code (includes directory). This page
was then included with a minimal code snippet at the bottom of my **post layout** - where I wanted the commentary field to show up.
I have also added some CSS to the commentary field, just to adjust the width a little bit. In each blogposts front matter comments
are enabled by using the tag: ```comments: true```

[Disqus]: https://disqus.com
[examination assignment]: https://coursepress.lnu.se/kurs/klientbaserad-webbprogrammering/examination/exam-assignment-1/
