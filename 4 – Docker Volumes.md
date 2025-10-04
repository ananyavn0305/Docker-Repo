## Easy Level

Q: What is a Docker volume?\
A: A volume is a persistent storage mechanism for Docker containers.

Q: Why do we use volumes?\
A: To persist data even after container deletion.

Q: How to create a volume?\
A: docker volume create <volume_name>.

Q: How to list all volumes?\
A: docker volume ls.

Q: How to inspect a volume?\
A: docker volume inspect <volume_name>.

Q: What command removes a volume?\
A: docker volume rm <volume_name>.

Q: What is the default volume location in Linux?\
A: /var/lib/docker/volumes/.

Q: What’s the difference between bind mount and volume?\
A: Volumes are managed by Docker; bind mounts use host paths.

Q: How to use a volume with a container?\
A: docker run -v <volume_name>:/path/in/container.

Q: Can multiple containers share a volume?\
A: Yes, for data sharing or communication.

## Moderate Level

Q: How do volumes help in stateful applications?\
A: They store persistent data like databases or logs.

Q: What is an anonymous volume?\
A: A volume created without a specific name.

Q: How can you back up a volume?\
A: Use docker run with tar to copy volume contents.

Q: How do you remove unused volumes?\
A: docker volume prune.

Q: What happens to volume data when container is removed?\
A: It remains unless manually deleted.

Q: How to mount host directory as a volume?\
A: docker run -v /host/path:/container/path.

Q: Can you use read-only volumes?\
A: Yes, with -v volume:/path:ro.

Q: Why prefer named volumes over bind mounts?\
A: Easier management and better portability.

Q: How to check volume usage?\
A: docker system df --volumes.

Q: Can Docker Compose manage volumes?\
A: Yes, under the volumes: section in docker-compose.yml.

## Hard Level

Q: How are Docker volumes different from host-mounted directories?\
A: Volumes are isolated, portable, and Docker-managed.

Q: How does Docker manage volume drivers?\
A: Drivers define how and where volumes are stored.

Q: What is a custom volume driver?\
A: A plugin that allows external storage integrations.

Q: Can volumes be encrypted?\
A: Yes, via external storage or driver configuration.

Q: What’s the impact of using tmpfs mounts?\
A: They store data in memory, not disk.

Q: How to migrate data between volumes?\
A: Use a temporary container to copy contents.

Q: Why use volumes in multi-container systems?\
A: To enable data sharing and persistence between services.

Q: Can volumes be shared across hosts?\
A: Yes, with networked or remote volume drivers.

Q: What’s the difference between overlay and volume data persistence?\
A: Overlay handles container layers; volumes store user data.

Q: How does Docker handle volume garbage collection?\
A: Unused volumes are deleted with prune.
