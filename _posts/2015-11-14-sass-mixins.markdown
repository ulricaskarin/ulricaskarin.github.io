---
layout: post
title:  "Sass Mixins"
date:   2015-11-14 16:00:00
category: Sass

type: article
description: A little chat about Sass Mixins

author: Ulrica Skarin
comments: true
published: true
---

Sass is a fantastic CSS preprocessor tool that lets you implement features like variables, mixins and other fun stuff.
It is a great help in maintaining large chunks of CSS code and I am happy that I've been introduced to it.

Today I've been playing around with some mixins for my CSS and I thought I'd share some of my newly achieved experiences
within this area. **But first, lets get to the bottom with what a Mixin actually is**. According to [Sass Guide][Sass Guide]
a mixin lets you make groups of CSS declarations that you'd like to reuse throughout your site. It is kind of like a function
for all of you who are familiar with programming languages. For example it is possible to
even pass values to your mixins which makes them more flexible.

Lets take a simple example on how you may implement a mixin. On the front page of this website I've got two "boxes" with
a slight shadow - *All posts* and *Posts by category*. As you understand, this is basically just a simple box-shadow css.
BUT - instead of writing the regular box-shadow-css directly on this element, I've turned it into a mixin so that I may
reuse it in several places if I'd wish. Then the only thing I need to do is adding a short ```@include box-shadow``` to
those elements I want it applied to. On top of that I also made sure that in my original mixin it is possible to pass
arguments to it. This means that I on each element with a box shadow may adjust it in terms of blur, color, optional
inset etc.

This is how my shadow mixin is coded:

{% highlight scss %}
// Box shadow mixin:
@mixin box-shadow($top, $left, $blur, $color, $inset:"") {

    -webkit-box-shadow:$top $left $blur $color #{$inset};
    -moz-box-shadow:$top $left $blur $color #{$inset};
    box-shadow:$top $left $blur $color #{$inset};
}

{% endhighlight %}

This is how I have applied the mixin to my boxes:

{% highlight scss %}
.catblock {
    @include box-shadow(0, 5px,5px, rgba(0, 0, 0, 0.175));
{% endhighlight %}

I urge all of you to go dive into the wonderful world of Sass. It makes a web developers life somewhat easier!

[Sass Guide]: http://sass-lang.com/guide/
[here]: http://schoewilliam.fr/
