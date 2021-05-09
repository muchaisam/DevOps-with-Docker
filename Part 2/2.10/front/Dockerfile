FROM node:14

RUN npm install -g serve

RUN npm install

ENV REACT_APP_BACKEND_URL=localhost:8080

RUN serve -s -l 4000 build

EXPOSE 4000

CMD ["npm" "start"]