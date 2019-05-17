FROM node:10.13-stretch

WORKDIR /app

ADD entrypoint.sh /
RUN chmod +x /entrypoint.sh
RUN git clone https://github.com/hikaruright/bookmanagement-angular-complete.git /app
RUN cd /app
RUN npm install -g @angular/cli
RUN npm install

RUN pwd

EXPOSE 4200

CMD [ "ng", "serve" ]