The Berkeley *FFS* was created as an improvement to the [[Unix]] File System. It consists of a fixed, asymmetrical [[tree]] index structure consisting of inodes ([[inode]]).

It is a combination of direct, indexed, and multi-level indexed allocation.

Characteristics:
- Tree structure: Efficient random access
- High degree: Each indirect block points to 100s of blocks; minimize seek
- Fixed structure: Byte $n$ will always be accessible via the same pointers
- Asymmetric: Supports small and large files