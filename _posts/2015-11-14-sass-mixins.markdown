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

On the front page of this website I've got a link to *Show all posts* that when clicked on - it folds out and shows a list of
all posts (well I know, I probably have to rewrite this one in the future when the list grows). The "folding out thing" I
created after tips in a tutorial [here][here].  The border and the box-shadow though, are mixins that I wrote myself and applied
to my "show posts div" with the ```@include box-shadow``` and ```@include element_border``` commands. I am truly in love with this feature and I strongly recommend
everyone who is developing web pages to take a deeper look into Sass. This is how my shadow and border mixin are coded:

{% highlight scss %}
// Box shadow mixin:
@mixin box-shadow($top, $left, $blur, $color, $inset:"") {

    -webkit-box-shadow:$top $left $blur $color #{$inset};
    -moz-box-shadow:$top $left $blur $color #{$inset};
    box-shadow:$top $left $blur $color #{$inset};
}

// Border mixin:
@mixin element_border($size, $color, $style) {
    border: $size $style $color;
}
{% endhighlight %}

I urge all of you to go dive into the wonderful world of Sass. It makes a web developers life somewhat easier!

[Sass Guide]: http://sass-lang.com/guide/
[here]: http://schoewilliam.fr/
