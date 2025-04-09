        COMMON STEPS
-----------------------------------------
##main banda folder and initial files banaayega:
##ab usse github par daal de:
```
1. create repo on github
2. at code section in perticular repo we will get link to push our code to this repo like: 
- echo "# repo_name" >> README.md
- git init
- git add .
- git commit -m "first commit"
- git branch -M main
- git remote add origin https://github.com/HarshV-910/GITHUB.git
- git push -u origin main
- git push -u origin main --force -> if we want overwrite forcefully without pull changes
- git pull origin main --rebase -> if there is changes in github then first we have to pull changes then we can push



```

##collaborators add kare:
```
 - go to perticular repo
 - then go to settings
 - then collaborator menu at left side
 - then add collaborator using email or username
```

------------------- 
##saare bande us repo se cloning karein:
```
git clone https://github.com/HarshV-910/GITHUB.git
```
##[VERY IMPORTANT] apni branch create karein:
```
git switch -C New_branch_name
```
apna code usi branch mein likhein
 complete hone par commit dein
 inform karein teammate ko about the commit
 merger banda(leader) fetch karega and merge karega and re-push