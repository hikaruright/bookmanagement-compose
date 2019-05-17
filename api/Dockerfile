FROM node:10.13-stretch

WORKDIR /app

ADD entrypoint.sh /
RUN chmod +x /entrypoint.sh
RUN git clone https://github.com/hikaruright/bookmanagement-api-server.git /app
RUN cd /app
RUN npm install
RUN ls

EXPOSE 4300

CMD [ "npm", "start" ]