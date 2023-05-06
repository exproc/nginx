FROM nginx:mainline-alpine
RUN apk add -U tzdata bash
ENV TZ=America/New_York
RUN cp /usr/share/zoneinfo/America/New_York /etc/localtime