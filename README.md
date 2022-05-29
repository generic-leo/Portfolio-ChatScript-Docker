# Portfolio-ChatScript-Docker

Start container 
```
docker start tagName
```
Stop container 
```
docker stop tagName
```

List all containers 
```
docker ps -a 
```

Remove container by id 
```
docker rm containerId
```

Get all images 
```
docker images
```

Remove image by id 
```
docker rmi imageId 
```

Build image 
```
docker built -t chatscript-ace:1 .
```

Run container 
```
docker run -t -i --name chatscript-ace -p 1024:1024 chatscript-ace:1
```
-t container tag name 
-i interactive mode 
-p local port number mapping to container port number 
"chatscript-ace:1" is the name of the image 

Once container has already started you can run the container using docker start command. 

Docker structure & chatscript reference - https://github.com/Mirrdhyn/chatscript-in-docker 

Update image for the container 
1. Remove the existing container 
2. Build the image with new version Ex. 'chatscript-ace:1' to 'chatscript-ace:2'
3. Run the container 
