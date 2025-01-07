FROM node:18.20.4-alpine3.20
WORKDIR /opt/server
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop
EXPOSE 8080
RUN chown roboshop:roboshop /opt/server
USER roboshop
COPY server.js   /opt/server/
COPY package.json /opt/server/
RUN npm install
CMD ["node", "server.js"]