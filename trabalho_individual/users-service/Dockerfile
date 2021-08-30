FROM node:14-alpine

WORKDIR /app

COPY package.json yarn.lock ./

RUN yarn

COPY . ./

RUN chmod +x ./startup.sh

CMD ["/bin/sh", "/app/startup.sh"]
