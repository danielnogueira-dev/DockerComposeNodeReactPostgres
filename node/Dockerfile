FROM node:12.10.0-stretch

RUN mkdir -p /var/www/html/app && chown -R node:node /var/www/html/app

COPY . /var/www/html/app

WORKDIR /var/www/html/app

COPY --chown=node:node . .

USER node

EXPOSE 3000

CMD yarn start