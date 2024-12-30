FROM node:14

WORKDIR /app

# if i use a . i'll copy into the workdir created previously
#I create a COPY layer just for the dependencies, because they don't change as often as the code
COPY package.json .

RUN yarn install

COPY . .

EXPOSE 80

#VOLUME ["/app/node_modules"]

#To use nodemon it is necesary to save files into the wls folder 
CMD ["npn", "start"]