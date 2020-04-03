FROM node:lts-alpine

RUN npm install -g http-server

WORKDIR /app

# COPY package.json.deploy ./package.json
# COPY package-lock.json.deploy ./package-lock.json
COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 8080
CMD [ "http-server", "dist" ]
