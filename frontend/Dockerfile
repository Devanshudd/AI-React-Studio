# Node alpine
FROM node:20.10.0-alpine

WORKDIR /app

# package.json && package-lock.json 
COPY package*.json ./

RUN npm install --legacy-peer-deps 

COPY . .

RUN npm run build

EXPOSE 9000

CMD ["npm", "start"]
