FROM node:12.18-alpine
MAINTAINER Alex Felipe Barbosa <alexfelipebarbosa@yahoo.com.br>
ENV NODE_ENV production
WORKDIR /usr/src/app
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "yarn.lock","./"]
RUN yarn install --production --silent && mv node_modules ../
COPY . .
EXPOSE 9000
CMD yarn start
