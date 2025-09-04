FROM node:20-alpine3.21
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
RUN chown -R roboshop:roboshop /opt/server
Environment=MONGO=true
// highlight-start
Environment=REDIS_URL='redis://{{ REDIS_HOST }}:6379'
Environment=MONGO_URL="mongodb://{{ MONGODB_HOST }}:27017/users"
USER roboshop
ENV MONGO='true' \
    REDIS_URL='redis://redis:6379'
    MONGO_URL="mongodb://mongodb:27017/users"
CMD ["node", "server.js"]