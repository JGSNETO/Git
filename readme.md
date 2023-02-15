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