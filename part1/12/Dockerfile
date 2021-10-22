FROM ubuntu:latest

WORKDIR /src/usr/app/
COPY ./example-frontend .

RUN apt-get update && apt-get install curl -y

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash
RUN apt install -y nodejs

RUN node -v && npm -v
RUN npm install && npm run build && npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]

EXPOSE 5000