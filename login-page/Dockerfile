# Dockerfile for add
#
# @author       Younggil, Lee(iamleeyounggil@gmail.com)
# @date         June/18/2023 created.
# @copyright    
#

FROM node:18.16.0-alpine

WORKDIR /usr/src/app

COPY package.json ./
COPY package-lock.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]`