FROM node:20-alpine

WORKDIR /srv/frontend

COPY ../../frontend/package*.json ./

RUN apk add --no-cache git

RUN npm install

COPY ../../frontend .

EXPOSE 3000

# RUN npm run build
CMD ["npm", "run", "dev"]