## Easy Level

Q: What is Docker?\
A: Docker is a containerization platform that allows applications to run in isolated environments called containers.

Q: What is a container?\
A: A container is a lightweight, standalone package that includes an application and all its dependencies.

Q: What is a Docker image?\
A: A Docker image is a read-only template used to create containers.

Q: What command lists all running containers?\
A: docker ps lists all running containers.

Q: What command lists all available images?\
A: docker images shows all images stored locally.

Q: What command starts a container?\
A: docker run starts a container from an image.

Q: What is Docker Hub?\
A: Docker Hub is a cloud-based repository for sharing Docker images.

Q: What is the difference between Docker and a virtual machine?\
A: Docker shares the host OS kernel, while VMs emulate separate OS environments.

Q: What is Docker Engine?\
A: Docker Engine is the core service that builds, runs, and manages containers.

Q: What command stops a running container?\
A: docker stop <container_id> stops a running container.

## Moderate Level

Q: What is the default network driver in Docker?\
A: The default network driver is the bridge driver.

Q: What command removes a stopped container?\
A: docker rm <container_id> removes a stopped container.

Q: What command removes an image?\
A: docker rmi <image_id> deletes an image.

Q: How do you check Docker’s version?\
A: Use the docker --version command.

Q: What is the Docker daemon?\
A: It’s the background service that manages Docker containers and images.

Q: What is a registry?\
A: A registry is a storage location for Docker images.

Q: What is the difference between CMD and ENTRYPOINT?\
A: CMD provides default arguments, while ENTRYPOINT defines the executable.

Q: How do you restart a stopped container?\
A: Use docker start <container_id>.

Q: What is the purpose of docker exec?\
A: It runs a command inside a running container.

Q: What does the -d flag do in Docker?\
A: It runs a container in detached mode (background).

## Hard Level

Q: Explain Docker’s client-server architecture.\
A: The Docker client communicates with the Docker daemon using a REST API.

Q: What happens when you run docker run on an image that doesn’t exist locally?\
A: Docker pulls the image from the registry before running it.

Q: How does Docker ensure isolation?\
A: Through Linux namespaces and cgroups.

Q: Explain how Docker achieves portability.\
A: Containers package the app and dependencies, ensuring consistent environments everywhere.

Q: What is the difference between an image layer and a container layer?\
A: Images are read-only layers, while containers add a writable layer on top.

Q: How do you check logs of a container?\
A: Use docker logs <container_id>.

Q: How can you view detailed info about a container?\
A: Use docker inspect <container_id>.

Q: How does Docker handle networking by default?\
A: It connects containers through a virtual bridge network.

Q: How do you clean up unused images and containers?\
A: Use docker system prune.

Q: What’s the purpose of the docker commit command?\
A: It creates a new image from container changes.
