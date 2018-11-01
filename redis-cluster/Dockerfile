FROM docker:latest

RUN apk update
RUN apk add alpine-sdk linux-headers
RUN cd /tmp && \
wget http://download.redis.io/redis-stable.tar.gz && \
tar xvzf redis-stable.tar.gz && \
cd redis-stable && \
make && \
cp src/redis-cli /usr/local/bin/ && \
chmod 755 /usr/local/bin/redis-cli
