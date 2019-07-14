# Git Cheatsheet

Git stuff I don't want to forget.

##

Move current branch's diversion commit up to the latest commit.

```bash
git fetch origin
git rebase origin/master
```

```
Before:

A-B-C-D-E
   \
    X-Y-Z

After:

A-B-C-D-E
         \
          X-Y-Z
```
