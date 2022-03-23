FROM node:16-alpine

ENV CI=true

WORKDIR /app
COPY package.json ./
#COPY ./node_modules ./node_modules
RUN npm install
COPY ./ ./

CMD ["npm", "start"]