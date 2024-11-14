FROM node:12.16

WORKDIR /app

RUN npm install -g @angular/cli

COPY package*.json .
RUN npm install

COPY . .

EXPOSE 4200

ENTRYPOINT ["ng", "serve"]
