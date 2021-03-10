## Working with Branches

**What are Branches?**

Branches in GitHub are a very easy way to work on a code file parallel, while the origin file stays untouched. In most other VCS you will need two files to do this.\
In Git, it is a lot less space consuming. You create Branches. Each Branch is a tip of a commit series. Because of this, Git only creates new Bubbles for the different parts between the files and reconstruct the files like it also does it normally.\
To summarize, Git Branches are only a history of commits divided from the main Branch at some point.
<br><br>
**Most important commands for Branches:**

`git branch` --> shows a list of all Branches in your local repository

`git branch -a` --> shows a list of all Branches in your remote repository

`git branch NAME` --> creates a Branch called NAME

`git branch -m NAME` --> renames Branch

`git branch -d NAME` --> deletes the Branch, but only, if all changes are merged

`git branch -D NAME` --> forces deletion even if unmerged

the Branches still exist in the remote repository --> to delete a remote Branch: `git push origin --delete crazy-experiment`

`git checkout NAME` --> switch to the Branch NAME

`git checkout -b NAME` --> creates Branch and switches to it

`git reflog` --> shows the last actions taken, view the history


**Merging and Rebasing**

Merging and rebasing basically do the same thing, just in different ways. As the name implies "Merging" merges the Master and the feature branch together \
resulting in a forked development history. Master and feature are brought back together. Rebasing on the other hand sets the feature branch on the tip of the\
 master branch. This action incorporates all the commits in the master branch therefore rewriting the development history and resulting in a linear history. \
This means  