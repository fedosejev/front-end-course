# Day 1

## What is Git?

### Problem

+ Software changes.
+ Software involves changes from multiple developers.
+ We want to:
  + Manage software changes.
  + Develop a "historical" view of our software project and be able to go back to the previous state of our software.

### Solution

From __Local Version Control Systems__ to __Centralized Version Control Systems__ to __Distributed Version Control Systems__.

+ Git is a Distributed Version Control System.

## 1. Install Git

1. Go to https://git-scm.com
2. Download for Mac
3. Install

## 2. Configure Git

### Tell Git who you are

1. `git config --global user.name "Artemij Fedosejev"`
2. `git config --global user.email "artemij.fedosejev@gmail.com"`

> This information is _immutably_ baked into the commits you start creating.

---

> Immutable - cannot be modified after it is created.

### Check your config settings

+ `git config --global user.name`
+ `git config --global user.email`
+ `git config --list --global`
+ `git config --list --local`

### Tell Git to use Sublime as a default editor

`git config --global core.editor "sublime -w"`

Learn more: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup

## 3. [Learn Git](learn-git.md)

+ Book: https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
+ Cheat Sheet: https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf
+ Reference: https://git-scm.com/docs

## 4. [Do homework](homework.md)

Ask Art if something is not clear!