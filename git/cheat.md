# Git Cheatsheet

Git stuff I don't want to forget.

## Aliases

```bash
git config --global alias.ammend 'commit --amend --reuse-message HEAD'

git config --global alias.br 'branch'

git config --global alias.cm '!git add -A && git commit'

git config --global alias.co 'checkout'

git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"

git config --global alias.lg2 "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)' --all"
```

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
