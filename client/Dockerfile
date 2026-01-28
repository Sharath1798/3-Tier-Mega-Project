#Setting up the baseimage (light weight linux distribution)

FROM node:22-alpine

#set up the working directory in container
WORKDIR /client-dir

#COPY the  package json file to the working directory 

COPY package.json ./

#install the dependencies
RUN npm install #RUN npm install 

#COPY the rest of the application code to the working directory
COPY . .

#expose the port 3000
EXPOSE 3000

#start the application
CMD ["npm", "start"]