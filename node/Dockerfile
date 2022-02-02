# Specify a base image
FROM node:alpine

# This indicates docker to choose this folder as a current working directory
WORKDIR /usr/app

# Install some depenendencies
# COPY ./ ./
# spliting COPY ./ ./ to given below because when we make only changes to files expect package.json than we
# have to reinstall all the dependencies even if we don't make changes to package.json which might be a little bit expensive
COPY ./package.json ./
RUN npm install

COPY ./ ./

# Default command
CMD ["npm", "start"]

# After the build is complete please run this command
# docker build -p <port_number>:8080 -t <your-docker_id>/nodeapp .