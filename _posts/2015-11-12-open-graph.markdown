---
layout: post
title:  "What is Open Graph?"
date:   2015-11-12 02:00:00
category: examination 1

image: ulricaskarin.github.io/assets/images/og_pic.png
type: article
description: Reflections over Open Graph Protocol, why to use it and how

author: Ulrica Skarin
comments: true
published: true
---

*This blogpost is part of an [examination assignment][examination assignment] at Linnaeus University.*

#### The Open Graph protocol, what is it?

The Open Graph Protocol enables a website to become a rich object by using special meta data in the head section
of a web page. In short, it puts the website owner in control over how his / her website is presented when shared in
social media.

#### Why is there a need for Open Graph?

*Content is king, but a king is powerless without followers*.

These words describe in short why there is a need for these special tags. In order to get a broader audience to
your website - Open Graph is actually essential. It has a great impact on website performance in social media (ie FaceBook).
Since social media sites are one major force in affecting a websites traffic (in a positive way) - the need for Open Graph all of a sudden becomes very clear.

#### How does it work?

The Open Graph Meta Tags is set in the head section of your code (just like ordinary meta tags).

*There are four required properties:*

- og:title - This defines the contents title. It serves a similar purpose as the traditional meta title tag.

- og:type - Describes the kind of object shared, for example - a blog post, video, picture and so on.

- og:image - Shows a thumbnail image when website is shared, this should be over 400x209px.

- og:url - Describes how the canonical URL is set for the page shared.

*...and some optional data...*

...like audio, description and site-name. If you'd like a list of all possible OG-tags, take a look
here: [The Open Graph Protocol][The Open Graph Protocol]. There are of course similar tools for other media,
Twitter uses something called TwitterCards for example, read more about this here: [Twitter Cards][Twitter Cards].

#### How I made use of Open Graph on this website:

I have used Open Graph in order to have control over how this website is presented when shared
in social media. In the head section of the original code I'm using Jekyll syntax with if statements to validate if for example
a page title or an image exists. This way I get an automatic dynamic and simple check to all my tags, without having to
do it manually for each page. As a concrete example I have implemented a description tag in my blogposts *front matter*
So if a user shares a specific blogpost, this is the description being shown.

To make sure it works as expected I have validated my OG with FaceBooks open graph debugger: [FaceBook Debugger][FaceBook Debugger].

![Open Graph Logo]({{ site.url }}/assets/images/og_pic.png){: .post-image }

[FaceBook Debugger]: https://developers.facebook.com/tools/debug/
[The Open Graph Protocol]: http://ogp.me/
[Twitter Cards]: http://davidensinger.com/2013/04/supporting-twitter-cards-with-jekyll/
[examination assignment]: https://coursepress.lnu.se/kurs/klientbaserad-webbprogrammering/examination/exam-assignment-1/
