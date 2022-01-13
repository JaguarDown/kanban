# kanban

## What
Personal version of Jira using the Kanban idea

## Why
- No other apps that I love
- Opportuniy to make something

## Getting Started
### Branch Conventions
#### Dev
All development will happen on the **dev** branch. All commits to this branch will be in the form of merging finished, local **feature** branches or **release** branches.
#### Feature
A local branch from **dev** for implementing features. Merged back into **dev** before being pushed or pull requested, then deleted locally. Naming convention: *feature-[name]*.

Commands:

Checkout: `git checkout -b feature-name dev`

Merge & delete:
```
git checkout dev
git merge --no-ff feature-name
git branch -d feature-name
```
#### Release
A branch from **dev**. Commits to this branch will be for bugfixes only. Merged into **master** with a version number tag and back into **dev**, then deleted. Increments the major version number. Naming convention: *release-[version number]*
#### Master
Commits to this branch will be merges from **release** branches or **hotfix** branches
#### Hotfix
A temporary branch from **master** meant only for fixing severe bugs on production releases in **master**. Merges back into **master** and **dev**. Increments the patch version number. Naming convention: *hotfix-version number*

### Version Number Convention
Semantic versioning. Major.minor.patch

### Useful reading:
- [github-flow](https://docs.github.com/en/get-started/quickstart/github-flow)
- [git cheat sheet](https://training.github.com/downloads/github-git-cheat-sheet/)

## Get help

## Maintainers
- Jaguardown
- Diggyblock