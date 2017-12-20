FROM node:latest

RUN mkdir -p /usr/src/msTourism
WORKDIR /usr/src/msTourism
COPY msTourism2/package.json /usr/src/msTourism/
COPY msTourism2/package-lock.json /usr/src/msTourism/
RUN npm install
COPY . /usr/src/msTourism
EXPOSE 3000
CMD npm start

