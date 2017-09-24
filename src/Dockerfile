FROM node:argon

# Create app directory
RUN mkdir -p /src
WORKDIR /src

# Install app dependencies
COPY package.json /src
RUN npm install

# Bundle app source
COPY . /src

EXPOSE 8080
CMD [ "npm", "start" ]