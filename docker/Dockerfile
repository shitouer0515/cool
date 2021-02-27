FROM node:15.9.0-alpine3.12
LABEL maintainer="Evine Deng"
ARG JD_BASE_URL=https://github.com/shitouer0515/cool
ARG JD_BASE_BRANCH=main
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin \
    LANG=zh_CN.UTF-8 \
    SHELL=/bin/bash \
    PS1="\u@\h:\w \$ " \
    JD_DIR=/jd \
    ENABLE_HANGUP=true \
    ENABLE_WEB_PANEL=true
ARG KEY="-----BEGIN OPENSSH PRIVATE KEY-----\n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\n-----END OPENSSH PRIVATE KEY-----"
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk update -f \
    && apk upgrade \
    && apk --no-cache add -f bash \
                             coreutils \
                             moreutils \
                             git \
                             wget \
                             curl \
                             nano \
                             tzdata \
                             perl \
                             openssl \
                             openssh \
    && rm -rf /var/cache/apk/* \
    && ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && echo "Asia/Shanghai" > /etc/timezone \
    && mkdir -p /root/.ssh \
    && chmod 700 /root/.ssh \
    && cd /root/.ssh \
    && echo -e $KEY > /root/.ssh/id_rsa \
    && chmod 600 /root/.ssh/id_rsa \
    && ssh-keyscan gitee.com > /root/.ssh/known_hosts \
    && git clone -b ${JD_BASE_BRANCH} ${JD_BASE_URL} ${JD_DIR} \
    && cd ${JD_DIR}/panel \
    && npm install \
    && npm install -g pm2 \
    && ln -sf ${JD_DIR}/jd.sh /usr/local/bin/jd \
    && ln -sf ${JD_DIR}/git_pull.sh /usr/local/bin/git_pull \
    && ln -sf ${JD_DIR}/rm_log.sh /usr/local/bin/rm_log \
    && ln -sf ${JD_DIR}/export_sharecodes.sh /usr/local/bin/export_sharecodes \
    && cp -f ${JD_DIR}/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh \
    && chmod 777 /usr/local/bin/docker-entrypoint.sh \
    && rm -rf /root/.npm
WORKDIR ${JD_DIR}
ENTRYPOINT docker-entrypoint.sh