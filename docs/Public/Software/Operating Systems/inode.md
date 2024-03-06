An *inode* contains a file's [[metadata]] and a set of pointers to locate its [[data blocks]]. 

The index structure is a combination of all of the indexed-based approaches. Files are represented as a fixed, asymmetric tree, with 4KiB data blocks as leaves. 

*Inodes* are stored consecutively in a big array, and indexed via an i-number. 

![inode](inode.png)
