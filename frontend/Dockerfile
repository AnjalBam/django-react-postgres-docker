FROM node:16

WORKDIR /app/frontend

COPY package*.json /app/frontend/

RUN npm install 

RUN npm i -g react-scripts

COPY . /app/frontend/

RUN chown -R node /app/frontend/node_modules

USER node

CMD [ "npm", "start" ]