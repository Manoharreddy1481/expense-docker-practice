FROM node:20
EXPOSE 8080
ENV DB_HOST="mysql"
#ENV DB_HOST="localhost" #Host Network
#ENV DB_HOST="mysql" Bridge Network
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
CMD [ "node", "index.js" ]
