# GIT-05: Track Multiple Files
# GIT-05: Track Multiple Files

## Problem Statement
Create three files in a project and add all of them to Git in a single operation.

## Solution

### Files created
- f1.txt
- f2.txt
- f3.txt

### Commands used
```bash
echo "Hello from file 1" >| f1.txt
echo "Hello from file 2" >| f2.txt
echo "Hello from file 3" >| f3.txt

git add f1.txt f2.txt f3.txt
git commit -m "Add three files to track multiple files"
```

### Explanation
`git add f1.txt f2.txt f3.txt` stages all three files in a single command,
satisfying the "single operation" requirement — rather than running
`git add` three separate times.

