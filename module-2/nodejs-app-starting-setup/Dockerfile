# To create the custom image based on the public node image
FROM node
 
# create a working directory
WORKDIR /app

# what to copy and then
#COPY . ./
#As we defined a working directory, we can use the following command to copy the files
# copy everything from the current directory to the working directory (./) The previous option should work too

COPY . /app

# Indicate docker to run a command
RUN yarn install

# Open the container port 80 to our local computer
EXPOSE 80

# Run the server when the container starts based on the image
CMD ["node", "server.js"]

