# Usefull commands 

## powershell delete a dir:
```bash
Remove-Item -Path "C:\MyOldProject" -Recurse -Force
```

## using ara2 cmd tool to download content on the internet.
```bash
aria2c -x 16 -s 16 "https://oslo2.nebula.to/c9ace27c58cf8efcd84c4a5c40d5f9fa6ec1cfeb.mp4?md5=bRsTS31MYuBqjJLHV8XsCg&expires=1757781247&fn=c9ace27c58cf8efcd84c4a5c40d5f9fa6ec1cfeb.mp4"
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

### how to build a docker image
```bash
docker build -t your-image-name:tag .
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

  example

sudo docker tag frankwere/stanbic-portal:1.1.0 frankwere/stanbic-portal:1.2.0
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

  docker stop <the container name>

remove the image
  docker images "this is to list all the images"

  docker rmi "<image ID>"

pull the new image
  docker pull "<repository>:<tag>"

run the container
  docker run -d --name my-frontend -p 8080:80 <your_image_name>:<tag>

  for example

docker run -d --name stanbic-portal -p 8080:80 frankwere/stanbic-portal:latest

```
### NOTE: docker ps -a will list all the container running and the once that has stopped.

### How to share data from one component to the other in angular
```bash
📌 Rule of Thumb

Use @Input / @Output for parent-child.

Use service with Subject/BehaviorSubject for siblings.

Use Router params or NgRx for cross-app state.
```

## Angular 18

#### How to install in locally
```bash
npm install @angular/cli@18
```
### how to build a docker image

```bash
docker build -t my-nodejs-app:1.0 .
```

### Create a new rule file
```bash
sudo nano /etc/udev/rules.d/51-android.rules
```

### restarting phone as an emulator for debuging.
```bash
sudo chmod a+r /etc/udev/rules.d/51-android.rules
sudo systemctl restart udev
```
#### after running the above command run the following
```bash
adb kill-server
adb start-server
```
