FROM node:18-alpine

WORKDIR /app

COPY package*.json tsconfig.json ./

RUN npm ci

COPY src ./src

RUN npm run build

EXPOSE 3005

CMD ["node", "dist/main.js"]
