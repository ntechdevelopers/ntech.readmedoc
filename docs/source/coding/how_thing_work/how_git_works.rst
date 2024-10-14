How Git Works
===================================

At its heart, Git is a content-addressable filesystem. This means that every piece of data—commits, files, directories—is identified by a unique hash value (usually a SHA-1 hash).
This hash is calculated from the content itself, ensuring that even the tiniest change results in a different hash.

**Git stores three primary types of objects:**

- **Blobs**  
  These are the fundamental building blocks, representing the contents of individual files.

- **Trees**  
  Trees organize blobs and other trees, forming a hierarchical structure similar to your project's directories and subdirectories.

- **Commits**  
  Commits are snapshots of your project at a specific point in time.
  They contain metadata (author, timestamp, commit message) and a reference to the root tree representing the project's state at that moment.

Git uses references (pointers) to track branches, tags, and other important points in your project's history. These are simply files that contain a hash value.

The most important reference is **HEAD**, which indicates the current commit you're working on.

**Let's understand the Git Workflow.**

- **Staging Changes**  
  When you use `git add`, Git calculates a hash for the modified file's content and stores it as a new blob object. It then updates the staging area (the index) with this blob's hash.

- **Committing**  
  When you `git commit`, Git creates a tree object representing the state of your entire project at that moment. This tree includes references to the blobs and trees that make up your files and directories. It then creates a commit object, referencing this tree, the parent commit(s), and your metadata.

- **Branching**  
  Branches are simply lightweight, movable pointers to specific commits. When you create a new branch, Git creates a new file (the branch reference) that initially points to the same commit as the branch you branched from. As you make changes on your new branch, the branch reference moves forward, while the original branch remains unchanged.

- **Merging**  
  When you merge branches, Git analyzes the changes made on each branch since their last common ancestor. If there are no conflicting changes, Git creates a new merge commit that combines the changes from both branches. If there are conflicts, Git marks them in your files and you need to resolve them manually.

**Exploring the .git Directory**

The hidden `.git` directory in your project's root is where Git stores all of its internal data.

1. **objects**  
   This directory contains all the blobs, trees, and commits, organized by their hash values. You can use the `git cat-file -p <hash>` command to inspect them.

2. **refs**  
   This directory stores branch references, tags, and other pointers.

3. **HEAD**  
   This file points to the current branch reference.

4. **config**  
   This file contains your repository's configuration settings.
