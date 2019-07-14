# Git Cheatsheet

Git stuff I don't want to forget.

## Aliases

- `git config --global alias.ammend 'commit --amend --reuse-message HEAD'`
  - Quick ammend.

## Rebase on origin

Move current branch's diversion commit up to the latest commit.

```
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
