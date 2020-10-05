---
layout: page
title: Git
categories: git
permalink: /git/
---

Copy a remote repository to your local machine:

```git
git clone <url for repository you want to copy>
```

Create a branch:

```git
git checkout -b <add-your-new-branch-name>
```

Switch branches:

```git
git checkout <branch>
```

Push your changes to a branch on your own repository that is forked from another repository:

```git
git push origin <branch-name>
```

Write to a remote repository:

```git
git push
```

Fetch and download content from a remote repository to update the local repository to match that content:

```git
git pull
```

Add the upstream repository (repository you forked from) as another remote:

```git
git remote add upstream <url for upstream repository>
```

Merge changes to upstream master with your local fork:

```git
git pull upstream master
```

Connect a local repository to a repository on GitHub using ssh (create new a repository on GitHub and then push an existing local repository):

```git
git remote add origin git@github.com:username/new_repo
git push -u origin master
```