## Easy Level

Q: How do you check running containers?\
A: docker ps.

Q: How do you attach to a running container?\
A: docker attach <container_id>.

Q: How do you execute a command in a running container?\
A: docker exec -it <container> <command>.

Q: How do you view logs in real-time?\
A: docker logs -f <container>.

Q: How do you prune unused resources?\
A: docker system prune.

Q: How do you remove all stopped containers?\
A: docker container prune.

Q: How to remove unused images?\
A: docker image prune.

Q: How to inspect container metadata?\
A: docker inspect <container_id>.

Q: How to monitor container resource usage?\
A: docker stats.

Q: How do you commit changes to a new image?\
A: docker commit <container_id> <new_image_name>.

## Moderate Level

Q: How do you troubleshoot a container failing to start?\
A: Check logs with docker logs and inspect the container.

Q: How to debug network issues between containers?\
A: Use docker network inspect, ping, or curl.

Q: How to optimize image size?\
A: Use minimal base images, multi-stage builds, and remove unnecessary files.

Q: How do you handle environment-specific configurations?\
A: Use environment variables or Compose .env files.

Q: How to backup container data?\
A: Use volumes with docker run --rm -v ... tar commands.

Q: How to restore container data?\
A: Use docker cp or mount volume backups.

Q: How to handle conflicting port mappings?\
A: Assign unique host ports or use dynamic ports.

Q: How to connect containers across hosts?\
A: Use overlay networks or Docker Swarm.

Q: How to persist logs outside container?\
A: Mount host directories or use logging drivers.

Q: How to perform rolling updates?\
A: Use Docker Swarm services or Compose with recreated containers.

## Hard Level

Q: How to secure container communication?\
A: Use encrypted overlay networks or TLS.

Q: How to handle secrets in Docker?\
A: Use Docker secrets or environment variables with restricted access.

Q: How to migrate running containers between hosts?\
A: Use docker commit to create an image and deploy on the new host.

Q: How to handle container failures automatically?\
A: Use restart policies like always or orchestration tools.

Q: How to analyze container performance bottlenecks?\
A: Use docker stats and profiling inside containers.

Q: How to isolate containers for security?\
A: Use user namespaces, seccomp, AppArmor, or SELinux profiles.

Q: How to manage multi-host deployment?\
A: Use Docker Swarm or Kubernetes orchestration.

Q: How to version control Docker images?\
A: Tag images with semantic versioning.

Q: How to handle dependency order in multi-container apps?\
A: Use healthchecks and depends_on in Compose.

Q: How to integrate Docker in CI/CD?\
A: Build, test, and deploy container images in pipeline scripts.
