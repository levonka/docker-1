FROM node:14.5.0
WORKDIR /app
COPY ./angular-pro/ ./
RUN npm install
ENTRYPOINT npm run start --host 0.0.0.0 --port 4201
#COPY ./angular-pro/* ./

