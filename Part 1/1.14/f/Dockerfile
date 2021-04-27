FROM node:14

RUN npm install -g serve

RUN npm install

ENV REACT_APP_BACKEND=localhost:8080

RUN serve -s -l 5000 build

EXPOSE 5000

CMD ["npm" "start" ]