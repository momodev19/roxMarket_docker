FROM node:20-alpine

WORKDIR /srv/backend

COPY ../../backend/package*.json ./

RUN apk add --no-cache git
RUN apk add --no-cache openssh

RUN npm install

COPY ../../backend .

EXPOSE 5000

CMD ["npm", "run", "dev"]
