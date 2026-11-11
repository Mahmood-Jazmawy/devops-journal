# Git Undo Guide

This guide explains common Git commands used to undo changes or recover work.

| Situation | Command | Safe after push? |
|---|---|---|
| Discard unstaged changes in a file | `git restore filename` | Yes |
| Unstage a file but keep its changes | `git restore --staged filename` | Yes |
| Fix the most recent commit message or contents | `git commit --amend` | No |
| Undo a commit by creating a new commit | `git revert COMMIT_ID` | Yes |
| Move back commits while keeping changes staged | `git reset --soft HEAD~N` | No |
| Move back commits and discard changes | `git reset --hard HEAD~N` | No |
| Temporarily save uncommitted changes | `git stash` | Yes |
