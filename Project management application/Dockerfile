FROM node:18.14-alpine
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
RUN npm build
COPY . .
EXPOSE 4000
CMD ["npm", "run", "start"]