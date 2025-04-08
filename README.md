# GITHUB
we can set out all values golbally on our local computer like this:

```markdown
git config --global user.name "Harsh Vekariya"

git config --global user.email "harshvekariya910@gmail.com"

git config --global core.editor "code --wait"

git config --global core.autocrlf "input"

```
  
we can edit all this things by:

```markdown
git config --global -e
```

##Tags:
```markdown
U : untracked
A : added or staged
C : commited
M : modified

```
##To know current status of staged or unstaged files
```
git status -s
```
##To know current status of saved checkpoints
```
git log --oneline
```

##Process:
```
first add file and make changes -> (M)

 then click on **+** icon to create checkpoint-> (A)

then give name to checkpoint and press commit -> (C)

now by this command we can check all checkpoint: git log --oneline
here all checkpoints have unique id
```

