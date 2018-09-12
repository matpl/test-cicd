FROM nginx as web-server
RUN apt-get update && apt-get install -y curl build-essential
RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -
RUN apt-get install -y nodejs
#FROM node as npm
#ADD package.json ./
#RUN npm i
WORKDIR /app
#COPY . .
COPY nginx.conf /etc/nginx/nginx.conf
#CMD nginx && ./node_modules/.bin/webpack-dev-server --port 8080

# docker run -it -d -p 8081:80 -v ./:/app --name wawa wawa
# docker run -it -d -p 8081:80 --name wawa wawa
# docker exec -it wawa ./node_modules/.bin/webpack-dev-server --port 8080 &