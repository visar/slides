# Basic concepts

  - <https://i.redd.it/7q82mjjyh6z01.jpg>
  - <http://i.imgur.com/MKjkKJ9.jpg>

---

# Anatomy of git

  - <https://i.imgur.com/oodiCnB.png>

---

# Commit messages

  - <https://imgur.com/8s753HN>
  - <https://chris.beams.io/posts/git-commit/>
  - <https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html>

---


# Tips and tricks

  - reflog
 
---

 - amend
 
---

 - diff (staged)
 
---

 - rebase (interactive)
 
---

 - stash
 
---

 - I accidentally committed something to master that should have been
    on a brand new branch\!

<!-- end list -->

``` bash
# create a new branch from the current state of master
git branch some-new-branch-name
# remove the commit from the master branch
git reset HEAD~ --hard
git checkout some-new-branch-name
# your commit lives in this branch now :)
```

 
---

 - I accidentally committed to the wrong branch\!

<!-- end list -->

``` bash
# undo the last commit, but leave the changes available
git reset HEAD~ --soft
git stash
# move to the correct branch
git checkout name-of-the-correct-branch
git stash pop
git add . # or add individual files
git commit -m "your message here"
# now your changes are on the correct branch
```

---


``` bash
git checkout name-of-the-correct-branch
# grab the last commit to master
git cherry-pick master
# delete it from master
git checkout master
git reset HEAD~ --hard
```

---


# GITIGNORE

  - <https://www.gitignore.io/>

---


# GIT FLOW

  - <https://veerasundar.com/blog/2018/03/gitflow-animated/>
  - <https://opensource.com/article/18/6/anatomy-perfect-pull-request>

---


# CHEATSHEETS

  - <https://zeroturnaround.com/rebellabs/git-commands-and-best-practices-cheat-sheet/>
  - <https://github.com/k88hudson/git-flight-rules/blob/master/README.md#flight-rules-for-git>

---


# Extra: bisect

  - <https://rkoutnik.com/articles/The-gits-guide-to-git-Bisect.html>

---


# MISC

  - <https://www.troyhunt.com/10-commandments-of-good-source-control/?m=1>

---


# BOOK

  - <https://git-scm.com/book/en/v2>

---


# xkcd

  - <https://www.xkcd.com/1597/>
  - <https://xkcd.com/1296/>

---


# Videos

  - <https://www.youtube.com/watch?v=ZDR433b0HJY>
  - <https://youtu.be/HDRXwokgWpo>
  - <https://www.youtube.com/watch?v=Y9XZQO1n_7c>
  - <https://www.youtube.com/watch?v=IHaTbJPdB-s>

---


# COURSES

  - <https://www.udacity.com/course/how-to-use-git-and-github--ud775>
  - <https://gettinggit.com/>
  - <https://trevordmiller.com/courses/real-world-git>
