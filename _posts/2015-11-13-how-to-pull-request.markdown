---
layout: post
title:  "How to pull request on GitHub"
date:   2015-11-13 20:30:00
category: github

type: article
description: How to make a pull request on GitHub

author: Ulrica Skarin
comments: true
published: true
---

What is a pull request? Well in simple words it's just a way of letting others know about changes you've pushed to a
repository on GitHub. Once a pull request is sent - the owner of the repo may review your added changes / modifications and
merge them with the master branch (if he / she finds it adequate). As a GitHub newbie - all this seemed kind of hard to grip.
It turned out it wasn't complicated at all once I went through with my first pull request. For those of you who feels like I primarily did,
here's a short description of how to make PR's happen!

Assuming you have got a GitHub account and found a repo you'd like to contribute to in a smart and well thought through way
(spam like PRs are big no no's!) - lets do a **pull request**:

- Fork the existing repo to get your own copy. This may be done by the little "button" fork in the top right corner of the repo page in question:
![Fork button]({{ site.url }}/assets/images/fork.png) *(no 6 in this image means it has been forked 6 times)*

- In your local terminal, now clone the repo by:

```git clone https://github.com/<your-username>/<forked-repo>.git```

- Make sure you stand in the right directory by writing: ```cd <forked-repo>/```

- To add the upstream remote to your local terminal do this by:
``` git remote upstream https://github.com/<repo-owner-name>/<repo-name>.git```

- Make a separate branch that you may do your work upon: ```git branch <name-of-branch>```

- Change to your newly created branch:
```git checkout <name-of-branch>```

- Make your contributions to the repo and then add this to your branch: ```git add .```

- Commit your changes: ```commit -m"<your smart words on the contribution>"```

- Push your changes: ```git push -u origin <name-of-branch>```

- Now when all is done, lets travel back to your own GitHub account. You may now see that in your forked repo a green
button has appeared: "Compare & pull request". Clicking this button takes you to a new page where you may add a comment
to the owner to the repo and then click the button "Create pull request". Voilà! Your PR is sent. Now, just wait and see
if it gets accepted.
