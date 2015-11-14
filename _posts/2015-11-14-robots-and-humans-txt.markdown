---
layout: post
title:  "Robots and Humans text"
date:   2015-11-14 15:17:25
category: examination 1
author: Ulrica Skarin
comments: true
---

*This blogpost is part of an [examination assignment][examination assignment] at Linnaeus University.*

#### What is robots.txt and how have you configured it?

Robots.txt is a small text file located in the root of a website. This file is what tells the search engines (as well as
the web crawlers) what content to index. In short when a robot is about to visit a website it first checks for the robot.txt
file. I have for now configured my robots.txt to disallow all robots to do any indexing on my website. The text-file:

{% highlight scss %}
User-agent: *
Disallow: /
{% endhighlight %}

Read more about [robots text][robots text].

#### What is humans.txt and how have you configured it?

Humans.txt is a file that provides human readable information about the website. This may contain info such as website owner,
the team, credits and contributions or development tools. This file is as well as the robots.txt file put in the website root.
My humans.txt provides information about the site, my contact channels as well which tools I have used when developing.

{% highlight html %}
/* TEAM */

Development and design: Ulrica Skarin
Twitter: @acirlu33
GitHub: ulricaskarin
Mail: ls222xp(at)student.lnu.se
Location: Sundsvall, Sweden

Support: The great staff at Linnaeus University, Kalmar, Sweden

/* SITE */

Last Update: 2015/11/14
Site Name:
Site URL: https://ulricaskarin.github.io
Language: English
Standards: HTML5
Components: Jekyll, GitHub
IDE: WebStorm
Graphic Tools: Illustrator CC / Photoshop CC
{% endhighlight %}

Read more about [humans text][humans text].

[examination assignment]: https://coursepress.lnu.se/kurs/klientbaserad-webbprogrammering/examination/exam-assignment-1/
[robots text]: http://www.robotstxt.org/
[humans text]: http://humanstxt.org/
