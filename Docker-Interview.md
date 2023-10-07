vim /etc/group
usermod -aG docker ubuntu


🔴🔸🔹✅⭕❌✔🔴🔸


🔸RUN vs CMD vs ENTRYPOINT
🔸Tell us something about Docker Compose.
🔸What is the lifecycle of a Docker Container?
🔸What is Docker?
🔸Suppose you have an application that has many dependant services. Will docker compose wait for the current container to be ready to move to the running of the next service?
🔸What is Docker Swarm?
🔸Will you lose your data, when a docker container exists?
🔸Can I use JSON instead of YAML for my compose file in Docker?
🔸How far do Docker containers scale? Are there any requirements for the same?
🔸What platforms does docker run on?
🔸Is there a way to identify the status of a Docker container?
🔸Can a container restart by itself?
🔸Is it a good practice to run stateful applications on Docker?
🔸How to check for Docker Client and Docker Server version?
🔸If you wish to use a base image and make modifications or personalize it, how do you do that?
🔸How to login into docker repository?
🔸If you vaguely remember the command and you’d like to confirm it, how will you get help on that particular command?
🔸Do you know why docker system prune is used? What does it do?
🔸How to delete an image from the local storage system?
🔸How do you list all the running containers?
🔸How to start, stop and kill a container?
🔸How will you monitor Docker in production?
🔸How to delete a stopped container?
🔸Once you’ve worked with an image, how do you push it to docker hub?
🔸Suppose you have 3 containers running and out of these, you wish to access one of them. How do you access a running container?
🔸How do you create a docker container from an image?
🔸How do you get number of container running, paused and stopped?
🔸How to build a Dockerfile?
🔸how to know the details of the list of networks?
🔸List all locally stored docker images?
🔸How to debug/see logs of our Docker container?
🔸
🔸






🔸RUN vs CMD vs ENTRYPOINT
🔹RUN
  ⭕The RUN instruction is used to execute commands When the container is created.
  ⭕It used to Installing applications and packages.
        RUN apt-get update && apt-get install -y python3
        RUN pip install Flask
🔹CMD
  ⭕The CMD instruction is used to specify the default command that will be executed when the container starts.
        CMD ["python", "app.py"]
🔹ENTRYPOINT
  ⭕The ENTRYPOINT instruction is used to specify the command that will always be executed when the container starts.
        ENTRYPOINT ["java", "-jar", "myapp.jar"]





🔸Tell us something about Docker Compose.
🔹Docker compose is a yaml file that contains services, network and volumes for setting up the docker container.


🔶What is the lifecycle of a Docker Container?
🔹Create the container
🔹Run the container
🔹Pause the container [optional]
🔹Unpause the container [optional]
🔹Start the container
🔹Stop the container
🔹Restart the container
🔹Kill the container
🔹Destroy the container


🔸What is Docker?
🔹Docker is a tool to create, run and deploy apps in the form of containers.
🔹Container is a package of code, libraries and dependencies requires application to run
🔹Using docker you can run application on-premises, local host, cloud any where you want.


🔸Suppose you have an application that has many dependant services. Will docker compose wait for the current container to be ready to move to the running of the next service?
🔹The answer is yes. Docker compose always runs in the dependency order. These dependencies are specifications like depends_on, links, volumes_from, etc.


🔸What is Docker Swarm?
🔹Docker swam manage and deploy docker container across multiple machines.


🔸Will you lose your data, when a docker container exists?
🔹Yes, you will lose any data when a Docker container exits unless you have persisted your data to a volume outside the container.


🔶Can I use JSON instead of YAML for my compose file in Docker?
🔹To use JSON file with compose, specify the JSON filename to use, for example: $ docker-compose -f docker-compose.json up


🔶How far do Docker containers scale? Are there any requirements for the same?
🔹Docker containers can be scaled to a very large number because they are lightweight and efficient.
🔹The main requirements for scaling Docker containers are:
  ⭕Hardware: This means that you need to have enough CPU, memory, and storage space.
  ⭕Network: This means that you need to have a high-bandwidth network connection.
  ⭕Software: You need to use a container orchestration tool to manage the deployment and scaling of the containers.Some of the popular container orchestration tools include Kubernetes, Docker Swarm, and Mesos.



🔶What platforms does docker run on?
🔹Docker runs on various Linux administration:
  ⭕Ubuntu 12.04, 13.04 et al
  ⭕Fedora 19/20+
  ⭕RHEL 6.5+
  ⭕CentOS 6+
  ⭕Gentoo
  ⭕ArchLinux
  ⭕openSUSE 12.3+
  ⭕CRUX 3.0+
🔹It can also be used in production with Cloud platforms with the following services:
  ⭕Amazon EC2
  ⭕Amazon ECS
  ⭕Google Compute Engine
  ⭕Microsoft Azure
  ⭕Rackspace


🔶Is there a way to identify the status of a Docker container?
🔹There are six possible states a container can be at any given point – Created, Running, Paused, Restarting, Exited, Dead.


🔶Can a container restart by itself?
🔹No, it’s not possible for a container to restart by itself. By default the flag -restart is set to false.


🔶Is it a good practice to run stateful applications on Docker?
🔹The concept behind stateful applications is that they store their data onto the local file system.
🔹You need to decide to move the application to another machine, retrieving data becomes painful. I honestly would not prefer running stateful applications on Docker.


🔶How to check for Docker Client and Docker Server version?
🔹$ docker --version //[This Commands gives you information about docker client and docker version.]


🔶If you wish to use a base image and make modifications or personalize it, how do you do that?
🔹$ docker pull <image_name> //[You pull an image from docker hub on to your local system.]


🔶How to login into docker repository?
🔹$ docker login //[Then there will be a prompted for your username and password]


🔸If you vaguely remember the command and you’d like to confirm it, how will you get help on that particular command?
🔹$ docker --help [lists all Docker commands]
🔹$ docker <command> --help  [help with one specific command]


🔸Do you know why docker system prune is used? What does it do?
🔹$ docker system prune
  ⭕Remove all stopped container
  ⭕Remove all the network that are not used
  ⭕Remove all dangling images
  ⭕Remove all build caches


🔸How to delete an image from the local storage system?
🔹$ docker rmi <image-id>





🔸How to start, stop and kill a container?
🔹$ docker start <container-id>
🔹$ docker stop <container-id>
🔹$ docker kill <container-id>


🔸How will you monitor Docker in production?
🔹docker stats and docker events to monitor docker in production.
  ⭕Docker stats provides CPU and memory usage of the container.
  ⭕Docker events provide information about the activities taking place in the docker daemon.


🔸How to delete a stopped container?
🔹$ docker rm <container id>


🔸Once you’ve worked with an image, how do you push it to docker hub?
🔹$ docker push <username/image name>


🔸Suppose you have 3 containers running and out of these, you wish to access one of them. How do you access a running container?
🔹$ docker exec -it <container id> bash
  ⭕The exec command lets you get inside a container and work with it.


🔸How do you create a docker container from an image?
🔹Run the Container: $ docker run [options] <image_name>
                     $ docker run -it -d --name my_nginx nginx
🔹Access the Container (Optional): docker run -d --name my_nginx -p 8080:80 nginx


🔸How do you get number of container running, paused and stopped?
🔹$ docker info


🔸How to build a Dockerfile?
🔹$ docker build <path to build docker file>


🔸how to know the details of the list of networks?
🔹$ docker network ls


🔸List all locally stored docker images?
🔹$ docker images


🔸How to debug/see logs of our Docker container?
🔹$ docker logs <container_id>


# Docker Commands
**<ins>_Run - Start a Container_</ins>** <br/><br/>
If not exist it pull the image and then run.
```bash
docker run nginx
```

**<ins>_ps - List containers_</ins>** <br/><br/>
List all running containers.
```bash
docker ps
```
List all running containers and also stopped and existed container.
```bash
docker ps -a
```
**<ins>_Stop - Stop a Container_</ins>** <br/><br/>
Stop container by the help of conatiner_id or container_name
```bash
docker stop container_id
```

**<ins>_rm - Remove a Container_</ins>** <br/><br/>
First stop a conatiner then remove.
```bash
docker rm container_id
```

**<ins>_List Images_</ins>** <br/><br/>
```bash
docker images
```

**<ins>_Remove Images_</ins>** <br/><br/>
```bash
docker rmi nginx
```

**<ins>_Pull - download image_</ins>** <br/><br/>
Download image not run the container
```bash
docker pull nginx
```

If not exist it pull the image and then run.
```bash
docker run nginx
```

**<ins>_Exec - execute a command_</ins>** <br/><br/>
See the content of running container
```bash
docker ps
```
```bash
docker exec <"container_id" or "container_name"> cat /etc/hosts
```

**<ins>_Append a command_</ins>** <br/><br/>
Make it sleep for 20 seconds before exiting.
```bash
docker run -d centos sleep 20
```

**Start an interactive Bash shell session within the container.**
`docker run -it centos bash`

# Docker Run
**<ins>_Run - tag_</ins>** <br/><br/>
```bash
docker run redis:4.0
```
**<ins>_Run - STDIN_</ins>** <br/><br/>
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/ea7df45a-cd01-44f3-9bae-864ea4b76621" width="600" background-size="cover"/>

**<ins>_Run - PORT Mapping_</ins>** <br/><br/>
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/f10ee882-7a96-4b67-ae3d-d8c3253ddb40" width="600" background-size="cover"/>

**<ins>_Run - Volume Mapping_</ins>** <br/><br/>
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/e5425e7d-2b5f-46d8-912f-fa97b3ba6c49" width="600" background-size="cover"/>

**<ins>_logs_</ins>** <br/><br/>
```bash
docker logs <"container_id">
```

**<ins>_Inspect Container_</ins>** <br/><br/>
```bash
docker inspect <"container_id">
```

## Docker registry
A Docker registry is a centralized repository for storing and distributing Docker container images. <br/><br/>
**Public Registries:** There are public Docker registries like Docker Hub, which allow anyone to upload and share container images publicly. <br/>
**Private Registries:** Organizations often use private Docker registries to securely store and manage their proprietary container images. Private registries require authentication and access control to ensure that only authorized users can pull or push images.


## Container Orchestration-Docker Swarm & Kubernetes

**<ins>_Why Orchestration_</ins>** <br/><br/>
When running a Node.js-based application within a Docker container, initially, you start with just one instance of your application on one Docker host. However, when the number of users increases, and that single instance can no longer handle the load effectively, you need to deploy additional instances manually by running the Docker command multiple times. This manual scaling process can become cumbersome.

Furthermore, you must actively monitor the application's load and performance using tools like CloudWatch. When you notice increased demand, you're responsible for deploying additional instances manually. Moreover, you also need to keep a watchful eye on the health of these application containers. If a container were to fail, it's your responsibility to detect the failure and initiate the Docker run command again to deploy another instance of the application. This manual intervention for scaling, monitoring, and handling failures can be time-consuming and error-prone.

Container orchestration tools, like Kubernetes or Docker Swarm, automate these tasks, making it easier to manage and scale your application in response to user demand, while also providing automated health monitoring and recovery mechanisms.

**<ins>_Container orchestration_</ins>** <br/><br/>

Container orchestration automates the deployment, management, scaling, and networking of containers.
It can help you to deploy the same application across different environments without needing to redesign it. 

**<ins>_What is container orchestration used for?_</ins>** <br/><br/>
Use container orchestration to automate and manage tasks such as:
 - Provisioning and deployment
 - Configuration and scheduling 
 - Resource allocation
 - Container availability 
 - Scaling or removing containers based on balancing workloads across your infrastructure
 - Load balancing and traffic routing 
 - Monitoring container health
 - Configuring applications based on the container in which they will run
 - Keeping interactions between containers secure


##################################################################################################<br/><br/>
**<ins>Ques 1</ins>. _How to check logs from my docker container and how do filter only the last 200 lines from the container log?_** <br/>
```bash
docker container logs --tail 200 [<container_id> or <container_name>]
```

**<ins>Ques 2</ins>. _What will happen to container logs if you restart the container? Will it be lost?_**  <br/>
If the container is stopped and started or restarted then we will not be losing any logs.

**<ins>Ques 3</ins>. _What will happen to container logs if you delete the container? Will it be lost?_>** <br/>
Yes, because containers are stateless, you will lose logs if you delete the container.

**<ins>Ques 4</ins>. _You encounter a docker image with size 2.7GB. Will this be a cause of concern? If yes how would you tackle this?_>** <br/>
- Bigger docker image would result in longer build time.
- Docker image download error or API rate limit issue (when you download from docker hub)
- Application will also become bulkier <br/><br/>
**<ins>SOLUTIONS</ins>**<br/><br/>
- Smaller Image Base (Alpine Images)
- Multi-Stage Builds feature when building docker image
- Remove package binaries after installing and don't install packages that isn't required
