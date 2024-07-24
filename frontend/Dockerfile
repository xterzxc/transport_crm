FROM node:18-alpine

# Set working directory
WORKDIR /crm

COPY crm/package.json ./
COPY crm/package-lock.json ./

RUN npm install

COPY crm/public ./public
COPY crm/src ./src 

EXPOSE 3000

# Start the application
CMD [ "npm", "start" ]
