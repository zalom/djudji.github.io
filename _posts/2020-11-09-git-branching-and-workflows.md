---
layout:     post
title:      Git branching and workflows
date:       2020-11-09 12:00:00
summary:    How do you organize your work in a code base? Here are my favorites.
categories: general
mathjax: false
---

How do you organize your work in a codebase? Is everything crammed in the `master`/`main` branch? What is the best branch naming approach? Do you use [Git Flow](#) or [GitHub Flow](#)? No "Flow" in particular?

All of us were juniors sometimes, and questions like these are common for both juniors and self-taught developers on a new project (not excluding starting your own project).

In this post, I'll try to go over some workflows I used, and I am still using to make sense of all that jazz.

[TL;DR](#), I use [GitHub Flow](#) with some modifications. I go light without too much complexity so I don't get lost in the code-organization hell.

### Git Branching Methodology

#### Types of branches
- `master`/`main` - protected and adored
- `development` - branched of the **master**, and targets the **master** in the PR/MR
- `epic` - branched of the **master** branch and targets the **development** branch in the PR/MR
- `csat` - branched of the **master** branch and targets the **master** or **development** branch in the PR/MR (optional)
- `story` - branched of the either branch above and targets the same "parent" branch

#### Naming branches
##### Story branches
- the name should start with the person's **initials** and a backslash **/**
- followed by the **story identifier** and then the brief **name** of the branch

_I assume you use some collaboration tools like JIRA, Clubhouse, Trello, or Pivotal Tracker. When you create a story/ticket/card, there is usually an identifier that can be used in the above context._

example:
  - `za/10-write-git-workflows-post`

##### Epic branches
- a collection of user stories
- the name should start with `epic` and a backslash **/**
- followed by the **epic story identifier** and the brief **name** of the branch

examples:
  - `epic/30-stripe-integration`
  - `epic/19-documents-upload`

##### Csat branches
- are a special type of **epic** branches that contain the collection of customer required changes
- the name should start with **csat** and a backslash **/**
- followed by a **memorable name**

examples:
- `csat/iron-man`
- `csat/nebula`
- `csat/chuck-norris` (use his name ONLY for the toughest, almost impossible customer requirements)

Hopefully our organization in the codebase will get better with time, and some common mistakes prevented with the use of "Flows".

My next blog post will discuss some collaboration strategies when it comes to working with these branches.

Some nice resources:
- <a href="https://nvie.com/posts/a-successful-git-branching-model/" target="_blank">Git Flow</a>
- <a href="https://guides.github.com/introduction/flow/" target="_blank">GitHub Flow</a>
- <a href="https://www.freshconsulting.com/git-development-workflows-git-flow-vs-github-flow/" target="_blank">Git Flow vs. GitHub Flow</a>

If you have any proposals or comments on the above, please share via the Disqus form below, and let's reach new heights together.

Z. - author
