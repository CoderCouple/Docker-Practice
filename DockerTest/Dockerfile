#https://nodejs.org/en/docs/guides/nodejs-docker-webapp/
#Refer to this webpage for any further clarification

FROM node:carbon

# Create app directory
WORKDIR /nodetest

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
ADD . /nodetest


RUN npm install
# If you are building your code for production
# RUN npm install --only=production

# Bundle app source
COPY . ./nodetest

EXPOSE 3000
CMD [ "npm", "start" ]
