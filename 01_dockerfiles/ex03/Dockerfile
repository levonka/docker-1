FROM ubuntu:16.04

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y ca-certificates openssh-server wget postfix

RUN wget https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh && \
	chmod 777 script.deb.sh && \
	./script.deb.sh && \
	apt-get install -y gitlab-ce

RUN apt update && apt install -y tzdata && \
  apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

EXPOSE 443 80 22

ENTRYPOINT (/opt/gitlab/embedded/bin/runsvdir-start &) && \
		   gitlab-ctl reconfigure && \
		   tail -f /dev/null

# How to build it?
# docker build -t ex03 .

# How to run it?
# docker run -it --rm -p 8080:80 -p 8022:22 -p 8443:443 --privileged ex03


# to make it work you need to allocate 2 GB of RAM and 2 processors to the virtual machine

# https://www.leaderssl.ru/articles/207-vse-pro-openssl-za-5-minut

# docker build -t ex03 .

# docker run -it --rm -p 8080:80 -p 8022:22 -p 8443:443 --privileged ex03

# --privileged        Give extended privileges to this container