# Our node app is based on `18-alpine` image 
FROM node:18-alpine

# Setting up the environment variables needed:
ENV DOMAIN="http://localhost:3000" \
PORT=3000 \
STATIC_DIR="./client" \
PUBLISHABLE_KEY="pk_test_51SNDfQDgMdoCI8XPW9g6N2VXMlCnDIzncvtXMWm6ztcOoTMReRNu0rqLE9bs3LbupMAxFlos8Cr1F5RISstTtv9G00eTVa103m"
WORKDIR /usr/src/app 

RUN npm install

COPY . .

EXPOSE 3000

CMD ["node", "server.js"]