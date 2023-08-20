# Specify a base image
FROM node:alpine

WORKDIR /usr/app
COPY ./package.json /usr/app

# Clear npm cache
# RUN npm cache clean --force

# Install some dependencies
RUN npm install
COPY ./ /usr/app

# Default command
CMD ["npm", "start"]
