## Easy Level

Q: What is a Dockerfile?\
A: It’s a script with instructions to build a Docker image.

Q: What command builds an image from Dockerfile?\
A: docker build -t <image_name> ..

Q: What is the purpose of the FROM instruction?\
A: It sets the base image for the build.

Q: What does the RUN instruction do?\
A: Executes commands during image build.

Q: What does CMD do?\
A: Defines the default command to run in the container.

Q: What is ENTRYPOINT used for?\
A: Defines the main executable in the image.

Q: What does COPY do?\
A: Copies files from host to image.

Q: What is WORKDIR?\
A: Sets the working directory inside the container.

Q: What is ENV used for?\
A: Sets environment variables.

Q: What does EXPOSE do?\
A: Documents ports that the container will use.

## Moderate Level

Q: What’s the difference between CMD and ENTRYPOINT?\
A: CMD provides defaults; ENTRYPOINT runs commands directly.

Q: How do you reduce image size?\
A: Use smaller base images and multi-stage builds.

Q: What’s the purpose of .dockerignore file?\
A: To exclude files from being copied into the build context.

Q: How do you pass build arguments?\
A: Use ARG in Dockerfile and --build-arg flag.

Q: What’s the effect of multi-stage builds?\
A: They optimize image size by discarding unnecessary layers.

Q: How to label images for metadata?\
A: Use the LABEL instruction.

Q: What’s the difference between ADD and COPY?\
A: ADD supports remote URLs and archive extraction.

Q: What does USER do in Dockerfile?\
A: Specifies the user for running commands.

Q: What’s the default user if USER isn’t defined?\
A: The root user.

Q: How can you debug Dockerfile issues?\
A: Build with --progress=plain and review logs.

## Hard Level

Q: What is layer caching in Docker builds?\
A: Docker reuses unchanged layers to speed up builds.

Q: How can you force Docker to rebuild all layers?\
A: Use --no-cache flag.

Q: How does Docker handle environment inheritance in builds?\
A: ENV persists across layers, but ARG doesn’t after build.

Q: What happens if multiple CMD instructions are present?\
A: Only the last CMD takes effect.

Q: What happens if you combine ENTRYPOINT and CMD?\
A: CMD provides default arguments to ENTRYPOINT.

Q: How can you minimize layer count?\
A: Combine commands in RUN using &&.

Q: What’s the advantage of using Alpine base images?\
A: They are lightweight and reduce build size.

Q: How do you verify build layers?\
A: Use docker history <image_name>.

Q: What is the default shell used in RUN commands?\
A: /bin/sh -c.

Q: Why use explicit versions in FROM?\
A: Ensures consistent builds across environments.
