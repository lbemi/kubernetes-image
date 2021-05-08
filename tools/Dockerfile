FROM alpine
USER root

#apk add --no-cache python3 python3-dev py-pip

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories && \
	apk add  --no-cache openrc docker git curl tar gcc g++ make \
    bash shadow openjdk8 python3 python3-dev py-pip openssl-dev libffi-dev \
    libstdc++ harfbuzz nss freetype ttf-freefont chromium chromium-chromedriver && \
    mkdir -p /root/.kube && \
    usermod -a -G docker root

