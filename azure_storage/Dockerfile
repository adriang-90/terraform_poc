# sets the base image
FROM node:12.18.1-alpine 

# sets directory in image
WORKDIR /usr/scr/app

# copies package.json file into the image
COPY package*.json ./

# installs only the production dependencies
RUN npm install --only=production

# copies the source code
COPY ./src ./src

# starts the microservice with npm start
CMD npm start