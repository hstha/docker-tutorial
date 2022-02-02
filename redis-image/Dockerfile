# Create the img file
# for this use an ezisting docker image as a base
# alpine is an OS
FROM alpine

# Install additional dependencies
# apk is a package manager in alpine which is used to install redis
# similar to sudo apt install redis in ubuntu
RUN apk add --update redis

# Tell img what to do when it starts as a container
CMD ["redis-server"]

# After the build is complete please run this command
# docker build -t <your-docker_id>/redis-image .