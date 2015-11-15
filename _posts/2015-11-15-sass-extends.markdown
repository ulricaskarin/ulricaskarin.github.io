---
layout: post
title:  "Sass Extend"
date:   2015-11-15 16:00:00
category: Sass

type: article
description: Why to use sass extends

author: Ulrica Skarin
comments: true
published: true
---

You may have noticed that I've kinda got a crush on Sass. Well, with that said, let's take a quick look at another helpful Sass-tool:
Sass ```@extend```. In short this feature means that you may reuse properties from one selector to another,
kind of like *inheriting* properties.

Lets say that you for example have got a class with properties which you
also use in several other classes. One possible way of writing this is by writing multiple class names in a row:

{% highlight scss %}
// All of my classes that share the same properties:
.classA, .classB, .classC {
    color: blue;
    background-color: yellow;
    border: 1px solid black;
}
{% endhighlight %}

This is not dumb at all, the problem emerges when you would like classB (or classC) to have additional properties apart from
the shared ones. In the above code this is not possible in any other way than separating the classes and writing them exclusively.
The **Sass Way** of doing this is really simple though. The command ```@extend``` is used to inherit, and then you may set
all the additional properties. All in one code-snippet:

{% highlight scss %}
// ClassA properties:
.classA {
    color: blue;
    background-color: yellow;
    border: 1px solid black;
}

// ClassB inherits ALL of classA properties AND has got additional properties:
.classB {
    @extend .classA;
    font-size: 2em;
}
{% endhighlight %}
