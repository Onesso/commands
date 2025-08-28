# Usefull commands 

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

### enable docker engine in ubuntu in the terminal
```bash
sudo systemctl enable docker
```

### starting docker engine in ubuntu in the terminal (cmd)
```bash
sudo systemctl status docker
```

### how to install a new node version
```bash
nvm install <the node version>
```

### how to install a new node version
```bash
nvm install <the node version>
```

### how to stop a docker command that is running.(first the containers running to get there id's)
```bash
docker ps
```

### how to stop a docker command that is running.(seconnd run the following command with theur id to stop it)
```bash
docker stop <container_id_or_name>
```
## How to push a docker image to docker hub

### step1: how to tag the image with your dockerhub username
```bash
docker tag capbackend:latest <YOUR_DOCKER_USERNAME>/capbackend:latest
```

### step2: Log in to Docker Hub
```bash
docker login
```

### step3: Push the Image
```bash
docker push <YOUR_DOCKER_USERNAME>/capbackend:latest
```

### ghana: 
```bash
"start": "node --max_old_space_size=8192 ./node_modules/@angular/cli/bin/ng serve",
```

### redeploying the image
```bash
stop the container
  docker ps "lists all the runing container"

  docker stop <container ID>

remove the image
  docker images "this is to list all the images"

  docker rmi "<image ID>"

pull the new image
  docker pull "<repository>:<tag>"

run the container
  docker run -d --name my-frontend -p 8080:80 <your_image_name>:<tag>

```
