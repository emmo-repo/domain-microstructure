Guidelines to develop the ontology with Git and Github
==========================================================

## Settings up your account on Github

### Create an account

### Add a public ssh key

## Installing Git on your computer

https://git-scm.com/downloads


## Interacting with the repository remotely

In our collaborative work, we aim at developing the ontology in parallel.
Each participant has a local repository to make its development. The local
developments are then pushed to the remote repository to be available for all the partners.

The main operations are described in the following sections.

### Clone the repository

The current version is available on GitHub so we want to copy that repository locally
to make our changes.
We will ***clone the repository*** with the following command line:
```
git clone git@github.com:emmo-repo/domain-microstructure.git
```

This operation uses ssh protocols so you need to have stored your public ssh key in your profile.
It is possible to clone also with https but it is simpler with ssh.

After that operation, you have the copy of the default branch (*main* in our case) 
but also all the branches.

### Transfer changes to the remote repository

Git aims at tracking the changes between version. For that reason, when you have made 
some changes two operations are needed: staging and committing. Staging will consist
in indicating which file is to be marked as changed (and so which changes will be recorded
in the repository). Committing will actually do the recording of the changes.

Staging is done by: ```git add name_of_file```

Commiting is done by:  ```git commit -m "my description of the changes" ```

The command ```git status``` will give you an overview of the tracked files that 
have been modified, the staged files, and also of the files that are not tracked.
It also indicates on which branch you are.

After the commit, your local repository has been updated. This update needs to 
be transferred to the remote repository stored on GitHub. We need to push the changes
by:
```git push```

### Update your local repository

```git fetch``` The git fetch command downloads commits from the remote repository
into your local repository to see the changes.

```git pull``` The git pull command is used to fetch and download content from a remote repository
and immediately update the local repository to match that content. 

To avoid merging issues, it is important to pull from the remote repository before 
adding new changes.

### Branching

Significant modifications on the code are usually done in branches. When the new feature of
the branch is developed, the branch can be merged with the main branch.

<p align="center"><img src="branching diagram.png" width="600"></p>

The main commands are:

```git branch ``` to get the list of branches.

```git checkout name_of_branch ``` to change to an existing branch.

```git checkout -b name_of_branch ``` to create a new branch and change to it.

```git checkout -b name_of_branch ``` to create a new branch and change to it.


### Merging

```git merge name_of_branch``` to merge the branch with your current branch.

In case of conflicts between your changes and what has been changed since your latest
update from the remote repository, you will need to resolve the conflicts.
During merge, the files will be modified to contain both versions of the portions
of codes. You need then to select what to keep.

More details are available here: 
https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts







