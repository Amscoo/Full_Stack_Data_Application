FROM node:alpine
RUN mkdir /frontend
WORKDIR /frontend
COPY . .
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN npm install
RUN npm install node-sass
RUN chmod 777 /frontend/node_modules
ENTRYPOINT ["npm"]
CMD ["start"]
