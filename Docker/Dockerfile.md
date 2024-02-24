A Dockerfile is a script that contains instructions for building a Docker image. It defines the base image, sets up environment variables, installs software, and configures the container for a specific application or service.

## Basic Anatomy of a Dockerfile 
```Dockerfile
# Specifies the base image.
FROM image_name:tag #

# Sets the working directory.
WORKDIR /path/to/directory

# Copies files/directories from 
# the build context to the container.
COPY host_source_path container_destination_path

# Executes commands.
RUN command1 command2

# Sets environment variables.
ENV KEY=VALUE

# Informs Docker that the container listens 
# on specified network ports at runtime.
EXPOSE port

# Provides default commands or parameters 
# for an executing container.
CMD ["executable","param1","param2"]

```

Other commands:
```Dockerfile
# Defines variables that users can pass 
# at build-time with build command.
ARG VARIABLE_NAME=default_value

# Creates a mount point for external volumes.
VOLUME /path/to/volume

# Specifies the username or UID to use.
USER user_name

# Adds metadata(kv pairs) to an image.
LABEL key="value"

# Similar to COPY, but with additional capabilities(extracting zips).
ADD source_path destination_path

```

## Example
```Dockerfile
# Use an official Node.js runtime as a base image
FROM node:20-alpine

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the current directory contents to the container at /app
COPY . .

# Expose port 8080 to the outside world
EXPOSE 8080

# Define environment variabl
ENV NODE_ENV=production

# Run app.js when the container launches
CMD node app.js
```