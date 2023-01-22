FROM node:17-alpine3.14

WORKDIR /home/node/app

COPY *.js /home/node/app/

COPY *.json /home/node/app/

RUN npm install

CMD ["node", "index.js"]

EXPOSE 3000

