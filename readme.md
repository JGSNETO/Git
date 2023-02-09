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