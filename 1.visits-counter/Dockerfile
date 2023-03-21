# Specify a base image/Users/armando1514/Desktop/docker-and-kubernetes/simple-web/Dockerfile
FROM node:14-alpine


WORKDIR /usr/app

# Install some depenendencies
COPY ./package.json ./
RUN npm install

##
# We do 2 different copies because in case
# I change the code in index.js, 
# it doesn't start to rebuild everything,
# just just copy the file into the folder.
# If was before npm install, it would restart the rebuild.
## 
COPY ./ ./


# Default command
CMD ["npm", "start"]