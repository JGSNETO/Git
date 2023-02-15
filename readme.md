### Basic Commands

- CLI: Comand Line Interface

- Windows: cd, dir, mkdir, del, rmdir - Shell
- Unix: cd, ls, mkdir, rm-rf - Bash


### How it works 

- Sha1: Encrypt the files. That is how git knows if something change. 


### Internal Objects

- Blobs: Files are stored inside blobs, and they contain metadata(Type, Size, content). 
- Trees: Blobs are stored inside trees. Point to different blobs. Contain also, metadata. Point to other blobs or trees. Recursive object. 
- Commits: Put it all together. Point to a tree, parent(Last commit), Message and author. 


### Merge conflict 

- When the same file is changed in different branches. You need to solve the conflicts before finish the merge process. 

### Merge

-  Merging is git's way of putting a forked history back together again. 
- A fast-forward merge can occur when there is a linear path from the current branch tip to the targe branch. Instead of "actually" merging the nbranchs, all git has to do to integrate the histories is move("fast forward") the current branch tip up to the target branch tip.

### Merge x Rebase

- Git rebase solves the same problem as git merge. 
- Merge will create a new "merge commit" in the feature branch that ties together the histories of both branchs, giving you a branch structure. Merge is a non-destructive operation. 
- Rebase moves the entire feature branch to begin on the tip of the main branch, effectively incorporating all of the new commits in main. But, instead of using a erge commit, reabse re-writes the project history by creating brand new commits for each commit in the original branch. This all yo can have a more clean project. 
- Golden rule of rebasing: Never use it on public branches. The rebase moves all of commits in main onto the tip of feature. The problem is that this ony happened in your repository. All of the other developers are still working with the original main. 
