## Easy Level

Q: What is Docker Compose?\
A: A tool to define and run multi-container Docker applications using a YAML file.

Q: What is the default Compose file name?\
A: docker-compose.yml.

Q: How do you start services with Compose?\
A: docker-compose up.

Q: How do you stop services in Compose?\
A: docker-compose down.

Q: How do you scale a service?\
A: docker-compose up --scale <service>=<num>.

Q: How do you view Compose logs?\
A: docker-compose logs.

Q: How do you rebuild images in Compose?\
A: docker-compose build.

Q: How do you run a one-time command in Compose?\
A: docker-compose run <service> <command>.

Q: Can Compose manage volumes?\
A: Yes, under the volumes: section.

Q: Can Compose manage networks?\
A: Yes, under the networks: section.

## Moderate Level

Q: How does depends_on work in Compose?\
A: It defines container startup order dependencies.

Q: How to pass environment variables in Compose?\
A: Using environment: or .env file.

Q: How to override Compose files?\
A: Use multiple -f flags: docker-compose -f file1.yml -f file2.yml.

Q: What is a service in Compose?\
A: A definition of a container with image, volumes, ports, etc.

Q: Can you define multiple networks in Compose?\
A: Yes, and attach services to specific networks.

Q: What is the command key used for?\
A: Overrides default CMD in image.

Q: How do you remove stopped Compose containers?\
A: docker-compose rm.

Q: How to check Compose version?\
A: docker-compose --version.

Q: How do you run detached mode in Compose?\
A: docker-compose up -d.

Q: How to connect Compose containers to external networks?\
A: Define external networks in docker-compose.yml.

## Hard Level

Q: How do you update a running Compose service?\
A: Use docker-compose up -d after modifying the YAML.

Q: Can Compose handle build arguments?\
A: Yes, with args: under service build:.

Q: What’s the difference between docker-compose up and docker-compose start?\
A: up builds and recreates containers; start only starts stopped ones.

Q: How does Compose handle service dependencies at runtime?\
A: It only controls start order, not readiness; healthchecks are needed.

Q: How to define restart policies in Compose?\
A: Use restart: with values like always, on-failure.

Q: How to limit resources in Compose?\
A: Use deploy.resources.limits in version 3+ or mem_limit in older versions.

Q: How to scale different services independently?\
A: Use --scale <service>=<num> for each service.

Q: Can Compose use custom networks with specific subnets?\
A: Yes, by defining subnet and IP range in networks:.

Q: How to handle persistent storage for multi-container apps?\
A: Define volumes in Compose and attach to services.

Q: How can Compose help in CI/CD pipelines?\
A: Automates multi-container environment setup consistently.
