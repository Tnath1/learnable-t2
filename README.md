# LEARNABLE TASK 2
## - Explain version control.
Version Control or Version Control Systems are software tools that help software engineers track the changes made to a file or set of files(code). It saves code snapshots when changes are made so that developers can recall specific versions later.

Version control sytems allows developers to revert selected files back to it's previous state, revert the entire project back to it's previous state, compare changes over time, see who last modified something that might be causing a problem, who introduced an issue and when. Using a version control systems also means if at any point on a project you loose files or mess things up, you can easily recover. The system makes sure that team members can collaborate effectively on the same project and making sure that team members are working on the latest version of the file or project. Examples include perforce, Beanstalk, AWS codeCommit, e.t.c
## - Explain the  difference between git and github.
The major difference bwtween git and git hub is:
* Git is a version control system that help software developers track their code changes or snapshorts of their code changes over time.
* GitHub is a web-based hosting service for git repositories, In a nutshell, you can use Git without GitHub, but, You cannot use GitHub without Git.
## - List 3 other github alternatives.
1. Concurrent Versions System (CVS)
1. Gitlab
1. Apache Subversion
## - Explain the difference between git fetch and git pull.

Git fetch and Git pull are Git commands used to update your local repository with changes from a remote repository. However, they differ in how they handle the updates:

1. git fetch: Fetches changes from a remote repository but does not automatically merge them into your working branch.

```bash
git fetch [remote]
```
* Downloads new branches, updates to existing branches, and new commits from the remote repository.
* Updates your remote-tracking branches (e.g., origin/master) to reflect changes in the remote repository.
* Does not change your working directory or current branch.


2. git pull: Fetches changes from a remote repository and automatically merges them into the current branch. 
```
git pull [remote] [branch]
```
* Performs a ``git fetch`` to download changes from the remote repository.
* Automatically merges the changes into your current branch.
* Updates your working directory to reflect the changes.

## - Explain in simple terms git rebase and the command for it.
In simple terms, git rebase rewrites commits from one branch unto another branch or moves commits from one branch (e.g develop) to another branch(e.g main). The command for that is written below: 
```bash
git rebase [develop]
```
* NOTE: The branch you want to rebase onto, is the branch that will be the new base of your current branch.

## - Explain in simple terms git cherry-pick and the command for it.
 git cherry-pick simply means choosing a commit from one branch and applying it to another branch. This command applies the changes introduced by one or more commits unto another branch.
 
 In other to run this command, you need to be sure you are on the branch you want to merge to and also you need the unigue hash code for the particular commit you want to cherry-pick
 * To cherry-pick one commit:
 ```
 git cherry-pick 867he79
 ```
 * To cherry-pick more than one commits:
 ```
 git cherry-pick 7980d367 98j0p91 86e9079
 ```
 Note: this commits will be picked and merged in the specified order.
