# Use an existing docker image as a base
FROM alpine

# Download and Install a dependency
RUN apk add --update gcc
RUN apk add --update redis

# Tell the Image what to do when it starts as a container
CMD ["redis-server"]

