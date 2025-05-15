FROM node:16-alpine AS firist

WORKDIR /app
COPY package-lock.json package.json .
RUN npm install
COPY . .

FROM node:16-alpine
WORKDIR /app
#RUN chown -R node:node /app
#USER node
COPY --from=firist /app .
EXPOSE 3000


CMD ["npm", "start"]
