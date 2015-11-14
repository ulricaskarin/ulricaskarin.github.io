---
layout: post
title:  "Pre-compiling CSS"
date:   2015-11-13 14:16:23

type: article
description: Reflections over pre-compiled CSS
category: examination 1
author: Ulrica Skarin
comments: true
---

*This blogpost is part of an [examination assignment][examination assignment] at Linnaeus University.*

#### What do you think of pre-compiling your CSS?

In short, CSS preprocessors like *Sass* (which is used in this project) takes the written code (for example scss) and
converts it to "normal CSS". I think that the beauty of it all is that it's not at all bound by the limitations of "old" CSS code. The
preprocessed language offers much more functionality like variables, nesting, mixins and other fancy techniques. Still,
the final outcome works just like the browser would expect it to do. For me personally the pre-compiling process has spared me
a lot of repeated code-writing which is just great.

#### Compare to regular CSS:

As mentioned above, pre-compiled CSS offers the developer extended techniques compared to normal CSS. For example one may
avoid repeating CSS by writing mixins (ie functions) that can be applied to an element with just a single code-row. One may
also declare variables to hold for example font-styles and hex-colors which greatly reduces both time and effort when
applying and maintaining the CSS. Another difference between pre-compiled CSS and CSS is that the pre-compiler makes you
aware of typos and missing components within the code. If you for example apply a color variable to an element without having
the variable declared - this will be pointed out to you.

#### Which techniques have you used?

I have tried to use as many techniques as possible within this project. For example I've used variables for all my colors and
font-styles. My theme-color that is applied to several elements may then be changed with one single line of code, which I believe is great.
I have also used several mixins in order to reduce code when applying for example shadows or borders to elements. Nesting
is another technique I have made use of, as well as a few mathematical operations to adjust spacing, width and so on.

#### Pros and cons?

I honestly believe that there are more pros than cons when it comes to pre-compiled CSS. It is efficient, time-sparing and
best of all - it allows you to reuse code and maintain the DRY principle. Disadvantages may derive from the fact that you
do need special tools to compile your code. Debugging the code may also offer some problem since generated code line-numbers
are not the same as within the source code. There is a solution to this though, for example one may use source mapping.
Source mapping is a .map file in JSON format that contains information that links the outputted CSS to the corresponding scss source line.

Read more about SASS that is used for pre-compiling in this project here: [Sass Guide][Sass Guide].

[examination assignment]: https://coursepress.lnu.se/kurs/klientbaserad-webbprogrammering/examination/exam-assignment-1/
[Sass Guide]: http://sass-lang.com/guide/
