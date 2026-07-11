FROM node:20
#creates /app and set the working directory to the /app directory
WORKDIR /app
COPY package*.json ./
COPY *.JS ./
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]

