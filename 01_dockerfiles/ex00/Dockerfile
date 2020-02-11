
# which image use as a base
FROM alpine

# command to run within container
RUN apk update && apk upgrade && apk add vim

# setting entry point
ENTRYPOINT ["vim"]

# build and run
# docker build -t ex00 . && docker run --rm -ti ex00

# -t		 	- name image

# docker build  - Build an image from a Dockerfile