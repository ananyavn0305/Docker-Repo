## Easy Level

Q: What is Docker networking?\
A: A system that connects containers for communication.

Q: What are the default network types?\
A: Bridge, host, and none.

Q: What is the bridge network?\
A: Default network allowing container-to-container communication.

Q: What is the host network?\
A: Shares the host’s network stack directly.

Q: What is the none network?\
A: Disables networking for the container.

Q: What command lists networks?\
A: docker network ls.

Q: How to inspect a network?\
A: docker network inspect <network_name>.

Q: How to create a network?\
A: docker network create <network_name>.

Q: How to remove a network?\
A: docker network rm <network_name>.

Q: Can multiple containers share a network?\
A: Yes, if connected to the same network.

## Moderate Level

Q: How to connect a container to a network?\
A: docker network connect <network> <container>.

Q: How do containers resolve names within a network?\
A: Docker’s internal DNS.

Q: What’s the default subnet for bridge networks?\
A: Typically 172.17.0.0/16.

Q: Can containers communicate across networks?\
A: Only if explicitly connected or routed.

Q: What’s an overlay network used for?\
A: For multi-host Docker setups like Swarm.

Q: How to disconnect a container from a network?\
A: docker network disconnect.

Q: What happens when you delete a network in use?\
A: Docker prevents deletion until all containers are detached.

Q: How can you test container connectivity?\
A: Use ping or curl commands between containers.

Q: What is MACVLAN?\
A: A driver allowing containers to have unique MAC addresses.

Q: What’s the difference between bridge and host networks?\
A: Bridge isolates; host shares network stack.

## Hard Level

Q: How does Docker use iptables for networking?\
A: To manage routing, NAT, and port forwarding.

Q: What’s the advantage of user-defined networks?\
A: Custom DNS and name-based resolution.

Q: How to attach multiple networks to one container?\
A: Use network connect multiple times.

Q: Can you control network IP ranges?\
A: Yes, via --subnet and --gateway.

Q: How do overlay networks work?\
A: They use VXLAN tunneling for multi-host communication.

Q: What happens when two networks overlap?\
A: IP conflict; Docker prevents creation.

Q: How can you expose internal services securely?\
A: Using reverse proxy containers like Nginx.

Q: Can you encrypt container traffic?\
A: Yes, through overlay encryption or service mesh.

Q: What is a network driver plugin?\
A: Custom networking integration modules.

Q: How does Docker handle DNS round-robin?\
A: It distributes requests among containers of same service.
