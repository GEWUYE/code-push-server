FROM node:8.11.4-alpine

RUN apk add --update git openssh
RUN npm i -g https://github.com/GEWUYE/code-push-server pm2@latest --no-optional

COPY ./process.json /process.json

EXPOSE 3000

CMD ["pm2-docker", "start", "/process.json"]
