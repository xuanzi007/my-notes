[markdown syntax cheetsheet](https://www.markdownguide.org/cheat-sheet/)

# gitclone troubleshoot solutions takedown

## 1. error:can't push refs to remote.try running pull first to integrate your changes

This error occurs when your local Git repository has diverged from the remote GitHub repository. reasons might be:
1 Remote Changes Exist: The GitHub repository has new commits that you don’t have locally.
2 Diverging Histories: Your local commits and the remote commits have separate histories (e.g., someone pushed to GitHub after you cloned the repo).
way to solve:
pull the remote change, and then push your local change again.

## 2. fatal: refusing to merge unrelated histories

The error fatal: refusing to merge unrelated histories occurs when you try to merge or pull commits from two Git repositories that Git considers unrelated.
way to solve:
open your VScode terminal(Ctrl + `), then code: ```git pull origin main --allow-unrelated-histories```
and then push again.
