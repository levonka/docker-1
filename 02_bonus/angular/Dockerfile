FROM node:14.5.0
WORKDIR /app
COPY ./angular-pro/ ./
RUN npm install
ENTRYPOINT npm run start

# docker build -t <name> .
# docker run --rm -it -p 4201:4201 <name>
