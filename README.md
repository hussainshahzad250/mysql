# Setup MySQL using docker

  ###  Pull MySQL Docker Image
  ```
    docker pull mysql
  ```

  ###  Run MySQL Container using below command
  ```
    docker run --name name-mysql -e MYSQL_ROOT_PASSWORD=root -d mysql:latest
  ```

  ###  Access MySQL: You can access MySQL from your terminal 
  ```
    docker exec -it name-mysql mysql -uroot -p
  ```

#  Create docker images from docker container and push to docker hub
    docker commit <container_id> your-docker-hub-username/your-image-name:tag

##  Ste-1 commit latest container changes, replace `90bb807b5928` with your docker container
```  
  docker commit 90bb807b5928 husssainshahzad/mysql:1.0
```

# Setup MySQL Using my custom MySQL docker image with default username `root` and password `root`
  
  ###  Pull docker image
  ```
    docker pull husssainshahzad/mysql:1.0
  ```
