FROM node:20-alpine

# Add configuration here
WORKDIR /app

COPY package.json /app
COPY package-lock.json /app

RUN npm ci 

COPY . /app

RUN npm run build

EXPOSE 4001

CMD ["npm", "run", "serve"]

