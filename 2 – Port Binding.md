## Easy Level

Q: What is port binding in Docker?\
A: It maps container ports to host ports for external access.

Q: What flag is used for port mapping?\
A: The -p flag is used for port mapping.

Q: Give an example of port binding.\
A: docker run -p 8080:80 nginx.

Q: What does 8080:80 mean in port mapping?\
A: Host port 8080 is mapped to container port 80.

Q: Can multiple containers use the same host port?\
A: No, each host port can be bound only once.

Q: What command shows mapped ports?\
A: docker port <container_id>.

Q: What is the default network type?\
A: Bridge network.

Q: What is localhost in Docker context?\
A: It refers to the host machine running Docker.

Q: Can you expose multiple ports in one container?\
A: Yes, using multiple -p options.

Q: What is the purpose of exposing ports?\
A: To make containerized services accessible externally.

## Moderate Level

Q: What’s the difference between EXPOSE and -p?\
A: EXPOSE documents ports in Dockerfile; -p actually maps them.

Q: How do you find which ports are bound?\
A: Run docker ps to see port mappings.

Q: What happens if you omit -p during run?\
A: The container runs, but its service isn’t accessible externally.

Q: What’s the effect of using -P instead of -p?\
A: -P maps all exposed ports to random host ports.

Q: How do you handle port conflicts?\
A: Use unique host ports for each container.

Q: What’s the significance of bridge networking for ports?\
A: Bridge networking isolates containers while allowing controlled communication.

Q: What is NAT in Docker networking?\
A: Docker uses NAT for translating container IPs to host IPs.

Q: How do you inspect port bindings?\
A: Use docker inspect and check “Ports” section.

Q: What command shows open ports on the host?\
A: netstat -tulpn or ss -tulpn.

Q: Can two containers communicate without port binding?\
A: Yes, if they share the same bridge or custom network.

## Hard Level

Q: Explain Docker’s internal DNS role in networking.\
A: Docker’s embedded DNS allows containers to resolve names within the same network.

Q: How does Docker route traffic between host and container?\
A: Through virtual Ethernet interfaces (veth pairs).

Q: What’s the role of iptables in Docker networking?\
A: Docker uses iptables rules to handle port forwarding and isolation.

Q: What’s a port publishing rule in Docker?\
A: A rule mapping host port traffic to container port.

Q: Can containers use host network directly?\
A: Yes, using --network host.

Q: How to expose internal ports without host mapping?\
A: Use EXPOSE in Dockerfile and access via internal network.

Q: What happens if you remove bridge network?\
A: Containers lose default connectivity and isolation.

Q: Why is port binding crucial in multi-container apps?\
A: It allows external access and inter-service communication.

Q: Can you bind ports dynamically in Compose?\
A: Yes, by setting host port to 0 in docker-compose.yml.

Q: How do you test port bindings?\
A: Use curl localhost:<port> or docker exec with netcat/ping.
