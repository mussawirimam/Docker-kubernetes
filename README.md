# Docker-kubernetes
https://www.geeksforgeeks.org/kubernetes-images/?ref=lbp


```
Docker start <Container ID or Name>
```

```
Docker stop <Container ID or Name>```
```

```
Docker pull <image name>
```

```
docker run -it --name mycon ubuntu:latest
```

```
docker run -itd --name myapp5 -p 9090:80 ubuntu:latest
```

```
exit
```
**If you want to exit without killing the process of bash within the container and run it in the background**
```
Ctrl p + q
```

```
docker exec -it myapp4 bash
```
```
Docker attach -it
```

```
docker image ls -aq
```

```
docker rm $(docker ps -aq)
```

```
docker rmi -f $(docker images -aq)
```

```
docker create --name app01 -p 8090:80 ubuntu 
```

```
apt get net-tools -y
```

```
netstat -tunalp
```

```
ps -elf
```

```
kill -9 <pid>
```

```
docker system prune 
```

```
docker container prune 
```

```
docker rm -f $(docker images -aq)
```

```
docker rmi -f $(docker image ls -aq)
```

```
docker container rm 25cbce5d329d <or name of container>
```

```
docker top <container ID or name>
```
```
```
```
```
```
```
```

