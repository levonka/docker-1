FROM debian

# Ports config (optional)
EXPOSE 9987/udp 10011 30033

ENV TS3SERVER_LICENSE=accept

RUN apt-get update && apt-get upgrade -y && \
	apt-get install -y apt-utils bzip2 wget
RUN	wget http://dl.4players.de/ts/releases/3.0.13.4/teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2
RUN tar -jxvf teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2


WORKDIR teamspeak3-server_linux_amd64

ENTRYPOINT sh ts3server_minimal_runscript.sh


# build and run
# docker build -t ex01 . && docker run --rm -p 9987:9987/udp -p 10011:10011 -p 30033:30033 ex01