FROM node:alpine

RUN npm install -g serve \
    npm install \
    serve -s -l 4000 build \
    useradd -m frontenduser

ENV REACT_APP_BACKEND_URL=localhost:8080

EXPOSE 4000

USER frontenduser

CMD ["npm" "start"]