FROM node:20

#Working directory
WORKDIR /app

#Install gatsby-cli
RUN npm install -g gatsby-cli

#Copy package.json and package-lock.json to the container
COPY package*.json ./

#Install dependencies
RUN npm install


# Copy the code into the container
COPY . . 

#Expose port 8080
EXPOSE 8080

#Start the site 
CMD ["gatsby", "develop", "-H","0.0.0.0", "-p" , "8080"]