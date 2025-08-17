FROM node:15.14-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

RUN npm install --silent 

RUN npm install ajv@^8 ajv-keywords && npm install

COPY . ./

CMD ["npm", "start"]