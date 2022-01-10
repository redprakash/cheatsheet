# Docker

## Login to the Docker Hub using the command 
- ```docker login -u YOUR-USER-NAME```

## Pull images
- docker pull <imnageName>
  
## View Containers
  - docker ps ```shows running container```
  - docker ps -a ```shows all the containers```
  - docker container ls

## View only the ids of the container/s
  -  docker ps -aq
  
## Delete Container
  - docker rm <container name or id> 

## Delete all Containers
  - docker rm $(docker ps -aq)
  - Force remove running container too ``` docker rm -f $(docker ps -aq) ```

## View Images
  - docker imnages

## Run Container on detached mode
  - docker run -d image:tagName <nginx:latest>

## Start Container
  - docker start <container name or id> 

## Stop Conatiner
  - docker stop <containerId> (To view container details ```docker ps```)
  - docker stop <name of the container
                      
## Naming a Conatiner
   - docker run --name ```testname``` -d nginx:latest
                      
## Mapping nginx to port 80
  -  docker run -d -p 8080:80 nginx:latest
  ``` can map differnt port number to port 80 ```
  
 ## Mapping multiple ports to port 80.
  - docker run -d -p 8080:80 ```-p 3000:80``` nginx:latest
