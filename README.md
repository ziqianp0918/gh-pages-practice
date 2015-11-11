# GitHub Pages Practice

### The purpose of this repository is to hold a complete set of files that work together to make a simple webpage.  You can fork/clone this repo and practice using GitHub Pages.

---

### Directions
*  Fork and clone this repository.
*  Make your new branch with the command `git branch gh-pages`
*  Open `.git/config`   
(if you are using **cloud9**, type `c9 .git/config`)

*  Add these two lines in the `[remote “origin”]` section:
```
	push = +refs/heads/master:refs/heads/gh-pages
	push = +refs/heads/master:refs/heads/master
```
it should now look like:
```
[remote "origin"]
	url = git@github.com:user/repo.git
	fetch = +refs/heads/*:refs/remotes/origin/*
	push = +refs/heads/master:refs/heads/gh-pages
	push = +refs/heads/master:refs/heads/master
```
*  If you haven't already, it would be a good idea to save a short reminder of the steps above into a text file (such as `gh-pages.txt`) in the root directory of your workspace.  

```
***COMMAND LINE***
git branch gh-pages
c9 .git/config

***PASTE INTO REMOTE ORIGIN***
push = +refs/heads/master:refs/heads/gh-pages
push = +refs/heads/master:refs/heads/master
```

*  Your repo is now ready!  Customize the content of `index.html` and use `git push` to see your changes on `<your-username>.github.io/gh-pages-practice`