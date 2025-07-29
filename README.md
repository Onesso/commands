# usefull commands 

## powershell delete a dir:
```bash
Remove-Item -Path "C:\MyOldProject" -Recurse -Force
```

## to remove remote github from you local project.

### first command to check list
```bash
git remote -v
```

### the remove the github
```bash
git remote remove orgin
```
### having essues creating a service or component in angular cli 
example
Schematic input does not validate against the Schema: {"style":"scss","type":"component","name":"qq"}
Errors:

  Data path "" must have required property 'project'.
```bash
ng g c <name-of-component> --project=<project-name>
```
### git command to only add the modified file
```bash
git add -u
```
### installing dependencies for legacy angular application
```bash
npm install -legacy-peer-dep 
```
### copying the file in the path(from windows) to the current dir in the wsl
```bash
sudo cp /mnt/c/Users/karao/Desktop/pem/giktekgreenlife.pem .
```

### in a scenarion where the remote repo is a head of your local repo and you want them to be together
```bash
git pull
```



