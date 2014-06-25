---
layout: docs
title: Git
prev_section: first-contribution-about
next_section: first-contribution-commits
permalink: /docs/first-contribution-git/
---

Before doing anything it's wise to set up Git correctly with your name and
email so other people can contact you if they have questions about your work:

```$ git config --global user.name "Your Name"
$ git config --global user.email your.name@example.com
```

Make a new branch from which you will make the changes

```$ git checkout -b mynewbranch```

This will create a new branch "mynewbranch" and immediately check out this branch.

type in the terminal type "git branch" to see your branch:

```$ git branch
  master
* mynewbranch ```

I assume you have made a github account (youraccount) and forked the Machinekit repo.
The next thing to do is to let Git and the local copy know about this. You want 
to get the changes you'll do locally transferred to your Github repository
at some point in time. Substitute "yourname" below with a name of your choice.

```$ git remote add yourname https://github.com/youraccount/machinekit.git```

now check this and "git remote -v" in the terminal will yield:

```$ git remote -v
yourname	https://github.com/youraccount/machinekit.git (fetch)
yourname	https://github.com/youraccount/machinekit.git (push)
origin	https://github.com/machinekit/machinekit.git (fetch)
origin	https://github.com/machinekit/machinekit.git (push)
```


