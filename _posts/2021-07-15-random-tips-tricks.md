---
layout: post
title: "Random Tips and Tricks"
subtitle: ":thought_balloon: Some useful findings to make coding a little bit easier (maybe)"
tags: [workspace, tips]
comments: true
---

*searches google for how to do something* ... *finds great source* ... *bookmark*
... *months later* ... *wait, how did I do that again?* ... *checks bookmarks* ...
*holy &$^! ... way too many bookmarks* ... *searches google again* ... *repeat cycle forever*

To note here, I primarily work in the macOS environment (with some dabbling in
Linux in my free time). So a lot of these tips will require the installation
of [Homebrew](https://brew.sh/) on your system.


# Syntax highlighting in nano
## MacOS

Install nano via homebrew
```
brew install nano
```

Open nanorc file
```
nano ~/.nanorc
```

Add the following line
```
include "/usr/local/share/nano/*.nanorc"
```

Refresh your terminal and voila, nano syntax highlighting

## Linux

Open nanorc file
```
nano ~/.nanorc
```

Add the following line
```
include /usr/share/nano/sh.nanorc
```

Refresh your terminal and voila, nano syntax highlighting

**Refs:**

[GithubGist](https://gist.github.com/BlakeGardner/5587269)  
[Stack Overflow](https://askubuntu.com/questions/90013/how-do-i-enable-syntax-highlighting-in-nano)




# Delete commits from a branch in Git
###### It happens sometimes... no judging here

**Careful:** `git reset --hard` *WILL DELETE YOUR WORKING DIRECTORY CHANGES*. Be sure to **stash any local changes** you want to keep before running this command.

Get rid of current commit (HEAD~1 means the commit before head)
```
git reset --hard HEAD~1
```

Or look at `git log` output to find the id of the commit you  want to back up to, and then

```
git reset --hard <sha1-commit-id>
```

If you already pushed it, you will need to do a force push to get rid of it
```
git push origin HEAD --force
```

**Refs:**

[Stack Overflow](https://stackoverflow.com/questions/1338728/delete-commits-from-a-branch-in-git)
