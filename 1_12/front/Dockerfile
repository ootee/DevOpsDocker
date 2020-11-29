FROM ubuntu:16.04

WORKDIR /mydir
EXPOSE 5000

RUN apt-get update && apt-get -y install curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN node -v && npm -v

COPY . .

RUN npm install
RUN API_URL=http://localhost:8000 npm run build
RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "dist"]
