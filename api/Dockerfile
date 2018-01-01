FROM node:latest

RUN mkdir -p /usr/src/msTourism2
WORKDIR /usr/src/msTourism

COPY ./msTourism2/package.json /usr/src/msTourism2/
COPY ./msTourism2/package-lock.json /usr/src/msTourism2/

ENV NPM_CONFIG_LOGLEVEL warn
RUN npm install
ENV PATH /var/node_modules/.bin:$PATH

COPY . /usr/src/msTourism2
EXPOSE 3000
CMD npm start

