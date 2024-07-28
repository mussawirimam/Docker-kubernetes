# Docker-kubernetes
ghcr.io
hub.docker.com
https://www.geeksforgeeks.org/kubernetes-images/?ref=lbp

**Start the Container**
```
Docker start <Container ID or Name>
```
**Stop the Container**
```
Docker stop <Container ID or Name>
```
**To Restart the Container**
```
docker restart <Container ID or Name>
```

**Docker pulls the image from docker hub or specified respository**
```
Docker pull <image name>
```

**Docker run pull OR if the image is already downloaded on host creates container in interactive mode**
```
docker run -it --name mycon ubuntu:latest
```

**Mapping the port and running it in interactive terminal as detached mode**
```
docker run -itd --name myapp5 -p 9090:80 ubuntu:latest
```
**exits the terminal**
```
exit
```
**If you want to exit without killing the process of bash within the container and run it in the background**
```
Ctrl p + q
```
**to execute a process within the running container**
```
docker exec -it myapp4 bash
```
**Attaches the host terminal to the container terminal without creating a /bin/bash proccess within the container (you can veryify it by running ps -ef within the container ton check the process)**
```
Docker attach -it
```
**List images without details**
```
docker image ls -aq
```
**Removes the unused docker containers with bash**
```
docker rm $(docker ps -aq)
```
**Force removes the unused docker containers images with bash variable/parameters**
```
docker rmi -f $(docker images -aq)
```
**Creates a docker container**
```
docker create --name app01 -p 8090:80 ubuntu 
```
**Linux networking utility**
```
apt get net-tools -y
```
**Linux command to check used ports**
```
netstat -tunalp
```
**Linux command to check the process list**
```
ps -elf
```
**kills the process with PID**
```
kill -9 <pid>
```
**Removes all unused resources by docker**
```
docker system prune 
```
**Removes all stopped containers**
```
docker container prune 
```
**Forcefully removes docker containers with bash variable/parameter**
```
docker rm -f $(docker containers -aq)
```
**Forcefully removes docker images with bash variable/parameter**
```
docker rmi -f $(docker image ls -aq)
```
**removes docker containers**
```
docker container rm <or name of container>
```
**Displays docker processes within the container**
```
docker top <container ID or name>
```
**To display the docker system usage**
```
docker system df 
```
**Gives you docker system info**
```
docker system info
```
**docker-commit - Create a new image from a container's changes**
```
docker commit <name of the container> <desiredname:version>
```
**to turn the image into tar file in order to email or send it to your collegue**
```
docker save <image ID or name with tag> -o <tarfilename>.tar 
```
to load back the docker image from tar file to docker image
```
docker load < <name of the tar image file>.tar
```
**To Login to dockerhub account to access your own repository**
```
docker login
```
**Unencrypted password location on host machine for hub.docker.com**
```
cat /root/.docker/config.json
```
**In order to push the image from host machine to hub.docker.com repository you will need to tag the username before the image in order to successfully push the image to remote repository**
```
docker tag myapp:v1 <username>/myapp01:v1
```
**docker-push - Upload an image to a registry**
```
docker push <username>/myapp01:v1
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
```
