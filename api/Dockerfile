FROM node:latest

RUN mkdir -p /usr/src/msTourism2
WORKDIR /usr/src/msTourism2

COPY ./msTourism2/package.json /usr/src/msTourism2/
COPY ./msTourism2/package-lock.json /usr/src/msTourism2/

ENV NPM_CONFIG_LOGLEVEL warn
RUN npm install
ENV PATH /var/node_modules/.bin:$PATH

COPY ./msTourism2 /usr/src/msTourism2
EXPOSE 80
CMD npm start

