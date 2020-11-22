FROM node:15.2.1-alpine3.10
LABEL version="1.0" description="webserver nodejs"
RUN apk update && apk upgrade
RUN apk add bash && apk add git
RUN mkdir felipe && cd felipe && git clone https://github.com/felipefranca93/simple-chat.git
WORKDIR /felipe/simple-chat/
RUN npm install 
CMD ["node", "server.js"]
EXPOSE 3000/tcp
