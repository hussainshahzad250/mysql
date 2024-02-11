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

# Setup MYSQL Using my custom MySQL docker image with default username `  root ` and password `root`
  
  ###  Pull docker image
  ```
    docker pull husssainshahzad/mysql:1.0
  ```
