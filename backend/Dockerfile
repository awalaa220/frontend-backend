FROM node:16-alpine

WORKDIR /app

# 
COPY package*.json package-lock.json ./

RUN npm install

# Copy application files
COPY . .


EXPOSE 3001

CMD ["npm", "start"]
