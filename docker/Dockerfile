FROM ubuntu:18.04
LABEL version="1.0" description="webserver ubuntu nodeJS"
RUN apt update -y && apt upgrade -y
RUN apt install nodejs -y && apt install npm -y && apt install git -y
RUN mkdir felipe && cd felipe && git clone https://github.com/felipefranca93/simple-chat.git && cd simple-chat/
EXPOSE 3000
CMD [ "npm install -s express", "npm install -s body-parser", "npm install -s socket.io", "npm install -s mongoose" ]
