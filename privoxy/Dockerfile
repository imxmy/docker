FROM alpine:3.14
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk add --update --no-cache privoxy \
    && echo 'listen-address  0.0.0.0:8118' > /etc/privoxy/config
EXPOSE 8118
CMD ["privoxy", "--no-daemon", "/etc/privoxy/config"]