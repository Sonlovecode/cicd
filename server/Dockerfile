FROM node:18-alpine

# Update Alpine packages to reduce vulnerabilities
RUN apk update && apk upgrade

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .    

EXPOSE 3000

CMD ["npm", "start"]
