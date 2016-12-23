# Git Commands

### Commit with a message :

```bash
git commit -m "this is my message"
```

### Create new branch :

```bash
git branch newBranch
```

### Switch to the new branch :

```bash
git checkout branchName
```

### Create a branch and switch to this branch :

```bash
git checkout -b branchName
```

### Switch to a special commit :

```bash
git checkout commitNumber
```

### Move a branch to a commit : 

```bash
git branch -f branchName <HEAD or commitNumber>
```
### Reset code to a previous commit in local :

```bash
git reset <HEAD or HEAD^ or HEAD~2>
```
### Reset code to a previous commit in remote :

```bash
git revert <HEAD or HEAD^ or HEAD~2>
```
### Copy commit to the current branch :

```bash
git cherry-pick <commit number>
```
### Interactive rebase :

```bash
git rebase -i <Commit number of the first commit to rebase>
```
