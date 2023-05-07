#FROM nginx:mainline-alpine
FROM alpine:edge
ENV TZ=America/New_York
RUN apk add -U tzdata curl bash nginx
RUN cp /usr/share/zoneinfo/America/New_York /etc/localtime
RUN date
RUN nginx -v

EXPOSE 80

STOPSIGNAL SIGQUIT

CMD ["nginx", "-g", "daemon off;]
HEALTHCHECK --interval=60s --retries=5 CMD curl --fail http://127.0.0.1 || exit 1