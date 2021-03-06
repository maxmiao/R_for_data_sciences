---
title: "GitHub Version Control"
author: "Brian S. Yandell"
date: "7/5/2017"
output: html_document
---

GitHub seems to be the best version control system. It was designed by Linus Torvalds to solve a problem of sharing ideas in the development of Linux (see [TED interview with Linus Torvalds](https://www.ted.com/talks/linus_torvalds_the_mind_behind_linux)).
While GitHub can be used for any type of documents, the `RStudio` folks have made elegant and easy connections.

- [Happy Git and GitHub for the useR](http://happygitwithr.com/)
- [Software Carpentry Version Control with Git](http://swcarpentry.github.io/git-novice/)
- [Tools for Reproducible Research by Karl Broman](http://kbroman.org/Tools4RR/)
    + [GitHub Tutorial](http://kbroman.org/github_tutorial/)
- [How GitHub uses GitHub to Build
        GitHub](https://speakerdeck.com/holman/how-github-uses-github-to-build-github)
- [ProGit Book by Scott Chacon and Ben Straub](https://git-scm.com/book/en/v2)
- [Getting Started With Git (UCSC Genome Browser)](http://genomewiki.ucsc.edu/index.php/Getting_Started_With_Git)
- [Good resources for learning git and github](https://help.github.com/articles/good-resources-for-learning-git-and-github/)
- [Git for humans](https://speakerdeck.com/alicebartlett/git-for-humans)
- [BFG Repo Cleaner](https://rtyley.github.io/bfg-repo-cleaner/)

## Github for Course Organization
 
- [How to point a domain on Google Domains to GitHub pages](http://www.curtismlarson.com/blog/2015/04/12/github-pages-google-domains/)
- [Happy Git Classroom Overview](http://happygitwithr.com/classroom-overview.html)
- [GitHub Education Staff](https://education.github.community) (education@github.com)
    + [CS50 at Harvard, automated tests, and portfolios](https://github.com/blog/2322-how-cs50-at-harvard-uses-github-to-teach-computer-science)
    + [Real-time feedback for students using continuous integration tools](https://github.com/blog/2324-real-time-feedback-for-students-using-continuous-integration-tools)
    + [Student-created portfolios using GitHub Pages](https://education.github.community/t/who-uses-github-pages-portfolios-peer-learning/9365)
- [COMBEE Git Workshop](https://combee-uw-madison.github.io/2017-09-29-git-workshop/setup/)
    
## Using Github for Pull Requests

Collaboration using version control is widespread and important.
However, it can be painful at times. Here are some code and links

### Add upstream source

This example uses [Data Carpentry](http://datacarpentry.org) protocols (such as `gh-pages` rather than `master` for main page). Here `upstream` is the source repository, `origin` is your copy of the repository on GitHub, and `gh-pages` is the local copy of the main branch of your repository.

Add the `upstream` source; pull contents into `gh-pages`; force the changes to be pushed to `origin`.

```
git remote add upstream https://github.com/datacarpentry/OpenRefine-ecology-lesson.git
git remote -v
git pull upstream gh-pages
git push --force origin gh-pages
```

- [Creating a pull request](https://help.github.com/articles/creating-a-pull-request/)
 
## Merge branch named `branch` into `master`

```
git checkout master
git pull
git checkout branch
git merge master
```

- [Create new branch with git and manage branches](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches) 
- [Git Branching Basic Branching and Merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
 
## Reset Master

This is a DANGEROUS thing to do as it is irreversible. ALWAYS cache a copy before doing something like this.

- [https://git-scm.com/2011/07/11/reset.html]
- [http://stackoverflow.com/questions/4359681/want-to-change-my-master-to-an-older-commit-how-can-i-do-this]
- [https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches]
- [http://stackoverflow.com/questions/8085838/how-to-move-the-changes-from-one-branch-to-another-branch-git]
 
