FROM alpine:3.4
COPY qshell /
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apk add --update ca-certificates curl && rm -rf /var/cache/apk/*
RUN chmod +x /qshell

#ENTRYPOINT ["/qshell"]
