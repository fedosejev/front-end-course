# Learn Git

## 1. How to edit files in Git?

### What is `Working Directory`, `Staging Area` and `Repository`?

<img src="https://git-scm.com/book/en/v2/book/01-introduction/images/areas.png" />

The basic Git workflow:

1. You modify files in your __working directory__.
2. You stage the files, adding snapshots of them to your __staging area__.
3. You do a commit, which takes the files as they are in the staging area and stores that snapshot permanently to your Git directory.

`Working Directory` > `Staging Area` > `Repository`

1. All changes are created in __Working Directory__.
2. They are then moved to __Staging Area__ when you tell Git to track them with `git add` command.
3. They are then become a part of a __Repository__ when you commit them with `git commit` command.

Learn more: https://git-scm.com/book/en/v2/Getting-Started-Git-Basics#The-Three-States

### How to clone an existing Git repository?

`git clone https://github.com/fedosejev/example.git`

> That creates a directory named `example`, initializes a `.git` directory inside it, pulls down all the data for that repository, and checks out a working copy of the latest version.

Learn more: https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository

### How to ignore files?

1. Create `.gitignore` file and open it in editor.
2. Add names of the file that you would like Git to ignore.

Learn more: https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Ignoring-Files

### How can you check status of your files?

+ `git status`
+ `git status -s` - short format.
+ `git status -b` - include branch and tracking, even when used with short format.

The lifecycle of the status of your files:

<img src="https://git-scm.com/book/en/v2/book/02-git-basics/images/lifecycle.png" />

Initially you have a clean working directory – in other words, there are no tracked and modified files.

+ When you edit `README.md` file in your repository it gets status of modified. The changed file is stored in your Working Directory.
+ You run `git add README.md` file to move current state of `README.md` file from Working Directory to Staging Area and change it's state from `modified` to `staged`.
+ You run `git add about.md` to track new file. This will change `about.md`'s state from `untracked` to `staged`.
+ You run `git commit -m "Add description"` to commit changes, i.e. change files' state from `staged` to `unmodified` and move changes from Staging Area to Repository.

Learn more: https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Tracking-New-Files

### How to move change from Working Directory to Staging Area?

`git add README.md` - take snapshot of the current state of `README.md` file and move it to Staging Area.

---

`.md` is a [Markdown](https://guides.github.com/features/mastering-markdown/) file format.

### How to move changes from Staging Area to Repository?

`git commit -m "Add description"` - move all changes from Staging Area to Repository.

Learn more: https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes

### How to move changes from Working Directory to Repository and skip Staging Area?

`git commit -a -m "Add description"` - move all changes from Working Directory to Repository.

### How to see commit history?

+ `git log`
+ `git log --oneline --decorate --graph --all`

> Commit history tells you a story of how the project was built.

### How to compare `Working Directory` with the `Staging Area`?

`git diff`

+ Use `up` and `down` keyboard arrow keys to scroll.
+ Press `q` to exit.

### How to compare `Working Directory` and `Staging Area` with the last commit at the branch you are currently on?

`git diff HEAD`

### How can I remove a file from Git?

1. `git rm`
2. `git commit -m "Remove README.md"`

Learn more: https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Removing-Files

### How can I tell Git to forget a file?

1. `git rm --cached "README.md"`
2. `git commit -m "Remove README.md"`

## 2. How can I undo things in Git?

### How to rename commit message or add more changes to my previous commit?

`git commit --amend -m "Add all changes"`

### How to move changes from Staging Area back to Working Directory?

`git reset HEAD README.md`

+ WARNING: Do not use `git reset --hard`

### How to revert all change in your Working Directory?

`git checkout -- README.md`

+ WARNING: You will loose all changes in this case.

Learn more: https://git-scm.com/book/en/v2/Git-Basics-Undoing-Things

## 3. What is commit, commit history and Git branch?

### What is commit?

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/commit-and-tree.png" />

### What is commit history?

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/commits-and-parents.png" />

### What is branch?

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/branch-and-history.png" />

### How to create a new branch?

`git branch testing`

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/two-branches.png" />

Learn more: https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell#Creating-a-New-Branch

### How to switch branch?

`git checkout testing`

You can create and switch to a new branch in one command:

`git checkout -b testing`

Which is a shortcut for:

`git branch testing`
`git checkout testing`

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/head-to-testing.png" />

+ Which Git command will produce this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/advance-testing.png" />

+ Which Git command will produce this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/checkout-master.png" />

+ Which Git command will produce this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/advance-master.png" />

### What is `HEAD`?

`HEAD` is one of many references (pointers) or `refs` in Git. A `ref` refers (points) to a centain commit on a branch. `HEAD` will always point to the last commit at the branch you are currently on.

### What is `refs`?

> In Git, a `ref` is a word that refers (points) to a specific commit hash in a commit history.

+ `origin/master` - points to tip of master branch on remote.
+ `HEAD` - points to tip of current local branch.

### What is a `tip`?

> A branch tip is the last commit or most recent commit on a branch.

## 4. How to merge branches?

Starting with this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-branching-1.png" />

---

Do this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-branching-2.png" />

---

Then this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-branching-3.png" />

---

Then this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-branching-4.png" />

---

Finally we want to do this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-branching-5.png" />

We want to merge `hotfix` branch into `master` branch:

1. `git checkout master` - switch to branch you want to merge into.
2. `git merge hotfix` - merge `hotfix` branch into your current branch.

---

Do this:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-branching-6.png" />

---

Now we want to do a three-way merge:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-merging-1.png" />

---

Which will produce a merge commit:

<img src="https://git-scm.com/book/en/v2/book/03-git-branching/images/basic-merging-2.png" />

Learn more: https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging

### How to delete branch?

`git branch -d hotfix`

### WARNING: Do not use `--hard`

You will loose your work, unless you know __exactly__ why you're using `--hard`.

### Why should I use Git commands if there is SourceTree app?

+ SourceTree app: https://www.sourcetreeapp.com

> The command line is the only place you can run all Git commands – most of the GUIs only implement some subset of Git functionality for simplicity. If you know how to run the command line version, you can probably also figure out how to run the GUI version, while the opposite is not necessarily true.
