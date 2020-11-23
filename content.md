# Catalyst <!-- .element: class="catalyst-logo" -->

# <img data-src="img/git.png" style="height: 120px; vertical-align: -20px; margin-right: 20px" />Git

Version control with Git and GitHub


## Introduction

- Evan Giles and Rebecca Blundell
<evan@catalyst.net.nz>
<rebeccablundell@catalyst.net.nz>
- Please interrupt to ask questions

Note:
This is us.


## Overview

- These slides are online: https://cat-training-2020.github.io
- Tutorial format (with some lecturing thrown in)
- Tutorial will be in phases (time permitting)
  1. <!-- .element class="fragment" --> Hands-on with GitHub and Atom
  2. <!-- .element class="fragment" --> Questions
  3. <!-- .element class="fragment" --> Discussion of GitHub workflows
  4. <!-- .element class="fragment" --> Hands-on with Git on the command line

Note: Need a place to host slides! They're not there!

## Overview

- Git is a powerful and potentially complex tool
- Two goals for the day
  1. <!-- .element class="fragment" --> Cover core concepts and terminology
  2. <!-- .element class="fragment" --> Familiarise with a useful workflow


# Git

<img data-src="img/git.png" style="height: 48px; vertical-align: middle;" /> <https://git-scm.org/>


# Git

Git is a **version control system**:

software that manages different versions of files


## Git

Why is it useful?

1. <!-- .element class="fragment" --> Keep track of changes to files
2. <!-- .element class="fragment" --> Review and revert back to old versions
3. <!-- .element class="fragment" --> Synchronise files between different locations
4. <!-- .element class="fragment" --> Test changes without losing the original copy

Note: 1. See who made changes when
2. Combine changes from different versions
3. Local, remote, many people
4. Work on a separate 'branch' or easily return to a past version


## Git

Why Git and not some other software?

1. <!-- .element class="fragment" --> Performance
2. <!-- .element class="fragment" --> Flexibility
3. <!-- .element class="fragment" --> **Popularity**

Note: Industry standard, lightweight
(Evan to comment on other possibilities, if needed)

# GitHub

<img data-src="img/github.png" style="height: 48px; vertical-align: middle;" /> <https://github.com/>


# GitHub

GitHub is a **hosting site for Git repositories**

(with lots of extra features)

Note: Website allowing collaboration using git.

Can see/share/edit/manage files online, even serve a website with Github pages


## GitHub

Why is GitHub useful?

1. <!-- .element class="fragment" --> Free hosting for open source projects
2. <!-- .element class="fragment" --> Interface for browsing and editing code
3. <!-- .element class="fragment" --> Workflows for collaborating with others
4. <!-- .element class="fragment" --> Create a static website with GitHub pages
5. <!-- .element class="fragment" --> Comprehensive documentation: https://docs.github.com/en

Note:


## GitHub

Why GitHub and not some other software?

1. <!-- .element class="fragment" --> **Popularity**

Note: Free, accessible to everyone, great for community/ education


# Atom

<img data-src="img/atom.png" style="height: 48px; vertical-align: middle;" /> <https://atom.io/>


# Atom

Atom is a **text editor**

with some useful Git and GitHub-related features


## Let's get started

Using Git's primary workflow


## Overview

1. **Create** a project (on GitHub)
2. **Clone** the project (onto your computer)
3. **Change** some files
4. **Commit** the changes
5. **Push** the changes (to GitHub)


### 1. Create a project

Initialise a new "repository" from within GitHub


### Create a project

- Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>


<img data-src="img/6.1.1 github signup.png"  style="margin: -130px; max-width: 130%;">
Note: - Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>

<img data-src="img/6.1.2 github create account.png" style="max-width: 80%; margin: -80px;">
Note: - Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>

<img data-src="img/6.1.3 account info.png" style="margin: -60px; max-width: 110%;">
Note: - Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>

<img data-src="img/6.1.4 account info.png" style="margin: -60px; max-width: 110%;">
Note: - Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>

<img data-src="img/6.1.5 verify email.png" style="vertical-align: 400px; margin: -60px; max-width: 120%;">
Note: - Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>

<img data-src="img/6.1 sign in_.png">
Note: - Go to <https://github.com/>
  - If you have an account, log in
  - If you don't, create one
    - You may need to verify your email address
- Click **New**
  - Or navigate to <https://github.com/new>

### Create a project

- Enter repository name **cs4hs**
- Check **Add a README file**
- Click **Create repository**

<img data-src="img/6.2.1 new repo.png" style="margin: -180px; max-width: 130%;">

Note: - Click **New**
  - Or navigate to <https://github.com/new>
- Enter repository name **cs4hs**
- Check **Add a README file**
- Click **Create repository**

<img data-src="img/6.2 new repo create_.png" style="margin: -60px; max-width: 80%;">
Note: - Enter repository name **cs4hs**
- Check **Add a README file**
- Click **Create repository**

<img data-src="img/6.2 new repo created_.png" style="margin: -180px; max-width: 130%;">
Note: This is what it looks like created.

### Remote cs4hs repository

- Exists on GitHub's servers
  - It is a "remote" repository
- Publically accessible
  - Anyone can see it
  - Only you can modify it

Note: <p style="color:rebeccapurple;">wb: Draw remote with one commit ("initial commit")</p>


### 2. "Clone" the project

Copy the project so you can edit it


### "Clone"

- Given the location of a repository
- Makes a copy of the project
- Stores it on your computer
- Links the two copies


### Clone the cs4hs repository

- Open Atom
  - Close any "welcome" tabs


<img data-src="img/7.3 atom-open.png" style="margin: -80px; max-width: 100%;">
Note: - Open Atom
  - Close any "welcome" tabs

### Clone the cs4hs repository

- Press **Control-Shift-P** to enter a command
  - Type **GitHub: Clone** and press **Enter**
- Choose file locations
  - **Clone from:** your GitHub repository URL <https://github.com/username/cs4hs>
  - **To directory:** wherever you like, e.g. home/yourname/code/cs4hs
  - To view folder pane on left in Atom, press Alt + \ or View -> 'Toggle tree view'

<img data-src="img/7.4.1 clone.png" style="margin: -80px; max-width: 100%;">

Note: Press **Control-Shift-P** to enter a command
- Type **GitHub: Clone** and press **Enter**


<img data-src="img/7.4.2 clone directories_.png" style="margin: -180px; max-width: 130%;">

Note:
Choose file locations
- **Clone from:** your GitHub repository URL <https://github.com/username/cs4hs>
- **To directory:** wherever you like, e.g. home/yourname/code/cs4hs
- To view folder pane on left in Atom, press Alt + \ or View -> 'Toggle tree view'

### Local cs4hs repository

- Exists on your computer
  - It is a "local" repository
- Files and folders behave as usual
- Linked to the version on GitHub

Note: <p style="color:rebeccapurple;">wb: Add local</p>

### 3. Change some files

Now you can make changes to your local copy


### Edit the README

- Edit file "README.md"

``` markdown
# cs4hs

## Test project

This is a project used to experiment with Git and GitHub.
```

- Save with **Control-S** (or from the **File** menu)


<img data-src="img/8.2 edit readme.png" style="margin: -100px; max-width: 130%;">

<img data-src="img/8.2.2 saved readme .png" style="margin: -100px; max-width: 130%;">

### Add a Python program
- Enter **Control-Shift-P** and **Add File**
- Enter the path for the new file: **hello.py**

``` python
print("Kia ora koutou,")
print("")
print("This is a simple python program.")
print("What does it do? Just prints out this message.")
print("")
print("Ngā mihi, Evan & Rebecca")
```

- Remember to save with **Control-S**



<img data-src="img/8.3.1 add file.png" style="margin: -100px; max-width: 130%;">
Note: Enter **Control-Shift-P** and **Add File**

<img data-src="img/8.3.2 add path.png" style="margin: -100px; max-width: 130%;">
Note: - Enter the path for the new file: **hello.py**

### Sidenote: the ".git" folder

- The ".git" folder contains Git's data files
- They can be edited but not saved in your repository


### Local changes

- You now have:
  1. Some edits to a file
  2. An entirely new file
- These changes only exist locally
- They have not been "saved" to your repository yet!


### 3.1 Tell Git who you are

- Click the **Git** button on the lower right corner of your Atom window

 - You should see a **Git Identity** pane

- Check the username and email you want to use for commits are correct

- Click **Continue**



Note: The 'git' pane in Atom has this
or edit the config file in .git to avoid using terminal


<img data-src="img/9.1.1 git identity_.png" style="margin: -60px; max-width: 120%;">
Note: - Click the **Git** button on the lower right corner of your Atom window

 - You should see a **Git Identity** pane

- Check the username and email you want to use for commits are correct

- Click **Continue**


### Tell Git who you are

An alternative to setting your **Git Identity** as above, is editing the config file:
- Edit file ".git/config"
- Add to the end of the file:

``` none
[user]
  name = Your Name
  email = you@example.com
```
Note: If the Git Identity window worked for you, you don't need to do this step.

### 4. "Stage" and "Commit" the changes

Save your edits to a new version of the project


### "Commit"

- Saving changes is a two-step process:
  1. Add them to the "staging area"
     - Tells Git to include the file in the next commit
  2. "Commit" the changes
     - Tells Git to save a new version of the project
- A "commit" is a version
  - Includes a message and attribution information



### Stage the edited file

- Open the "Git" pane
- Your changes are currently "unstaged"
- **Right-click** and **Stage** "README.md"


<img data-src="img/10.3.1 stage readme.png" style="margin: -60px; max-width: 120%;">
Note: **Right-click** and **Stage** "README.md"
<>Jump to File opens for editing, stage file adds all, stage hunk (visible), click in file to stage line

Can unstage in the same ways

### Commit the edited file

- Enter a **Commit message**: something descriptive
- Click **Commit to main**

<img data-src="img/10.4 commit readme.png" style="margin: -60px; max-width: 120%;">
Note: - Enter a **Commit message**: something descriptive
- Click **Commit to main**
<p style="color:rebeccapurple;">wb: add "Update readme" commit</p>

### Stage and commit the new file

Use the same process, this time for "hello.py"


<img data-src="img/10.4 stage hellopy.png" style="margin: -60px; max-width: 120%;">
Note: **Right-click** and **Stage**

<img data-src="img/10.5 commit hellopy.png" style="margin: -60px; max-width: 120%;">

Note:- Enter a **Commit message**
- Click **Commit to main**

<p style="color:rebeccapurple;">wb: add "Add hello.py" commit</p>

### Local commit history

- You now have a series of changes
- This is your project's "commit history"
- It tells you who changed what, how, and when
- You can "revert" to previous versions


### 5. "Push" the changes

Now you can publish these new commits on GitHub


### Log in to GitHub

- Edit file ".git/config"
- Add your username to the cloned URL

``` none
[remote "origin"]
  url = https://<username>@github.com/<username>/cs4hs.git
```
Note: Replace 'username' with your github username


### Push your commits

- Open the "GitHub" pane
- Click **Login**
- Follow the link to <https://github.atom.io/login>
- Copy the generated token
- Paste it into Atom under **Enter Token**
- Click **Login**

<img data-src="img/11.3.1 login to github.png" style="margin: -60px; max-width: 120%;">
Note: - Open the "GitHub" pane
- Click **Login**

<img data-src="img/11.3.2 get token.png" style="margin: -60px; max-width: 120%;">
Note: - Follow the link to <https://github.atom.io/login>

<img data-src="img/11.3.3 copy token.png" style="margin: -60px; max-width: 120%;">
Note:
- Copy the generated token
- Paste it into Atom under **Enter Token**
- Click **Login**

### Push your commits

- Open the "Git" pane
- Click **Push 2** on the bottom right in Atom
- Visit GitHub to view your published changes

Note: Push 2 commits
<p style="color:rebeccapurple;">wb: add commits to remote</p>


## Review

1. Created a project (on GitHub)
2. Cloned the project (onto your computer)
3. Changed some files
4. Committed the changes
5. Pushed the changes (to GitHub)


## Next Steps

Reviewing and modifying commits


## Reviewing changes

Your project now has a "history" you can review


### Your project's history

- A series of commits
- Every commit has:
  1. <!-- .element class="fragment" --> A message
  2. <!-- .element class="fragment" --> An author
  3. <!-- .element class="fragment" --> A date
  4. <!-- .element class="fragment" --> A set of changes
  5. <!-- .element class="fragment" --> A "parent" commit
  6. <!-- .element class="fragment" --> A unique ID
     - This is also known as its "hash" or "SHA1"


<img data-src="img/14.2 commit elements.png" style="margin: -60px; max-width: 120%;">

Note:- Every commit has:
  1. A message
  2. An author
  3. A date
  4. A set of changes
  5. A "parent" commit
  6. A unique ID
     - This is also known as its "hash" or "SHA1"


## Fix-ups

What to do when you've made a mistake?


### Undo a commit

- Open the "Git" pane
- Click **Undo** on the most recent commit
  - The commit is deleted
  - Its changes are moved back into the staging area
  - Its message is preserved

Note: <p style="color:rebeccapurple">wb: rub out the local commit</p>


### Fix a commit

- Edit "hello.py" and add two lines at the end

``` python
print("Kia ora koutou,")
print("")
print("This is a simple python program.")
print("What does it do? Just prints out this message.")
print("")
print("Ngā mihi, Evan & Rebecca")
print("")
print("PS. I'm learning Git")

```

- Save the file
  - The new changes are now *unstaged*


### Fix a commit

- Stage the new changes
- Commit the result
  - You have just replaced the old commit with a new one

Note: <p style="color:rebeccapurple">wb: replace the local commit</p>

### Push the commit

- Hover over the button you used to push
  - What does it say now?

Note: It says "Pull 1". (But it can't pull without a conflict)
We undid after pushing to remote, so repos diverged...


### Push the commit

- To push these commits you must "force push"
- **Right-Click** and choose **Force Push**

Note: We must either fix merge conflict or force push. In **this** case we will force push.


You will see a warning message as this overwrites data on the remote repository!
<img data-src="img/force push.png" style="max-width: 120%;">

Note: Normally we would avoid this, but we know no one else is working on the repo at this stage.

<p style="color:rebeccapurple;">wb: replace the commit on the remote</p>

## Branches

Isolating and sharing specific sets of changes


### Branches

- Each "branch" indicates a separate version
- Multiple branches in a single repository
- Let you work without interfering with others
- Eventually combined or "merged"
- The default branch is called "main"


## Overview

1. Create a new **branch**
2. **Commit** to the branch
3. **Push** the branch (to GitHub)
4. Create a **pull request** (on GitHub)
5. **Accept** the pull request (on GitHub)


### 1. Create a new branch

Starts a new set of changes


### Create a branch

- Open the "Git" pane
- Click **main**
  - Click **New Branch**
  - Type **feature**
  - Click **New Branch** (again)
- You have a new "feature" branch


### 2. Commit to the branch

New commits are added to the active branch


### Create a new commit

- Edit the file "README.md"

``` markdown
# cs4hs

## Test project

This is a project used to experiment with Git and GitHub.

This is some information about the project.
```

- Save and commit the change as usual


### Isolated changes

- Click **feature** to open the branch picker
  - Click **main** to switch branches
- README.md has changed back
  - The edit has been made to the **feature** branch
  - The **main** branch remains unchanged


### 3. Push the branch

Send the new branch to GitHub


### Push the branch

- Open the "Git" pane
- Switch back to **feature**
- Click **Publish**
- Visit your project on GitHub
  - The **feature** branch has been pushed


### 4. Create a pull request

Request your branch to be "merged"


### Request a merge

- Click **Compare & pull request**
- Enter some information
- Click **Create pull request**



### 5. Accept the pull request

Merge the "feature" branch into "main"


### Merge the branch

- Make sure you're happy with the changes!
- Click **Merge pull request**
  - Add any information you'd like to include
  - Click **Confirm merge**
- Click **Delete branch**
  - Removes it from the remote repository


### Review the new commits

- The two branches have been combined
- There are two new commits:
  1. Your own
  2. A "merge commit"
- The combination happened on GitHub
  - GitHub is the *remote* repository
  - Your *local* repository is now out of date


### Update your local repo

- Back in Atom, open the "Git" pane
- Open the branch picker
  - Switch back to **main**
- Click **Fetch**
- Click **Pull 2**


### Update your local repo

- The two new commits are pulled from GitHub
- You are back up to date with "origin"


## Review

1. Created a new branch
2. Committed to the branch
3. Pushed the branch (to GitHub)
4. Created a pull request (on GitHub)
5. Accepted the pull request (on GitHub)


## Merge Conflicts

When two branches can't be combined safely


## Overview

1. Create two **incompatible commits**
   - One locally
   - One on GitHub
2. **Pull** the remote change (from GitHub)
3. **Resolve** the resulting conflict


### 1. Create two commits

Changing the same line but with different content


### Edit a file locally

- Open "README.md" and change the last line

``` markdown
# cs4hs

## Test project

This is a project used to experiment with Git and GitHub.

This is some important information about the project.
```

- Make it read "important information"
- Commit the result



### Edit a file remotely

- Visit your repository on GitHub
- Click the **pencil icon** on README.md

``` markdown
# cs4hs

## Test project

This is a project used to experiment with Git and GitHub.

This is some unimportant information about the project.
```

- Make it read "unimportant information"
- Enter a commit message
- Click **Commit changes**


### 2. Pull the remote change

Try (and fail) to combine the two branches


### Fetch changes

- **Right-click** the **Push 1** button
- Click **Fetch**
  - This retrieves the new commits
- Click **Pull 1**
  - This attempts to merge the changes
- You should hit **Merge conflicts**


### 3. Resolve the conflict

Indicate how the two changes should be combined


### Pick a side

- The two different versions are coloured
- Edit the highlighted region to be "correct"

``` markdown
# cs4hs

## Test project

This is a project used to experiment with Git and GitHub.

This is some potentially important information about the project.
```

- Remember to save the file when finished


### Commit the result

- Stage the file
- Click **Commit to main**
- The conflict is resolved locally


### Share the result

- We still need to push the resolution
- Click **Push 2**
- Now everything is back in sync


## Review

1. Created two **incompatible commits**
2. **Pulled** to combine the two
   - Encountered a merge conflict
3. **Resolved** the conflict


## Questions?


## GitHub Workflows

A few helpful tips for working with GitLab


### Forking

Contributing to a project that isn't yours


### Forks

- A "fork" is a copy of a repo *on GitHub*
  - Copies from one user account to another
  - Think of it like a "remote clone"


### Forks

- The result is a repo you control
  - You clone your forked copy
  - You push commits
- Pull request comes from your fork


### Let's try it

- Navigate to my cs4hs repository
  - <https://github.com/cat-train1/cs4hs>
- Click **fork**


### Clone your fork

- In Atom use **Control-Shift-P**
  - Choose **GitHub: Clone**
- Enter the fork's URL *including your username*
- Click **Clone**


### Make some changes

- Use the standard workflow:
  1. Edit
  2. Stage
  3. Commit
  4. Push
- Visit your project on GitHub


### Open a pull request

- Click **New pull request**
- Click **Create pull request**
  - This request will be in my repo


### Git Culture

Some keywords to help navigate the landscape


### Git Keywords

- **Squash**: Combining many commits into one
- **Rebase**: Alternative to merging
- **Feature**: Branch dedicated to specific feature
- **Hotfix**: Branch dedicated to a single bug
- **CI**: Testing new commits automatically
- Others?


## Command Line

Using the Git program from the terminal


### Open a Terminal

- This depends on your Operating System
  - Windows: Git Bash
  - macOS: Terminal
  - Linux: Terminal


### Using the Terminal

- Quick command line how-to


### The Git Command

- The **git** command (lower case) runs Git
- Enter **`git --version`** to see whether it works


### Configuring Git

- `git config core.editor "atom --wait"`
- <!-- .element class="fragment" --> `git config user.name "Evan Hanson"`
- <!-- .element class="fragment" --> `git config user.email "evanh@catalyst.net.nz"`


### Cloning a project

- `git clone <url>`
- <!-- .element class="fragment" --> `cd cs4hs`
- <!-- .element class="fragment" --> `git status`


### Making commits

- `atom README.md`
- <!-- .element class="fragment" --> `git status`
- <!-- .element class="fragment" --> `git add README.md`
- <!-- .element class="fragment" --> `git commit -m "message goes here"`


### Reviewing history

- `git log`
- <!-- .element class="fragment" --> `git show`
- <!-- .element class="fragment" --> `git show <commit>`


### Fixing commits

- `git reset <commit>`
- <!-- .element class="fragment" --> `git reset --hard <commit>`
- <!-- .element class="fragment" --> `git add`
- <!-- .element class="fragment" --> `git commit`


### Branching

- `git branch`
- <!-- .element class="fragment" --> `git branch <name>`
- <!-- .element class="fragment" --> `git checkout <name>`


## Questions?


## Thanks!

- Evan Giles & Rebecca Blundell
- <evanh@catalyst.net.nz>
- <rebeccablundell@catalyst.net.nz>
- Slides will be emailed out
- Don't hesitate to contact me!


<!-- .slide: class="image-slide" -->
![freedom to innovate](css/theme/images/freedom-to-innovate.svg "freedom to innovate") <!-- .element: class="cat-slogan-image" -->
