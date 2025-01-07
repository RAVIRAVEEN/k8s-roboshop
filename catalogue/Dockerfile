FROM node:18.20.4-alpine3.20
WORKDIR /opt/server
EXPOSE 8080
COPY server.js   /opt/server/
COPY package.json /opt/server/
#ENV MONGO=true
RUN npm install
CMD ["node", "server.js"]