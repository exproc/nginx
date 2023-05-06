FROM nginx:mainline-alpine
ENV TZ=America/New_York
RUN apk add -U tzdata bash
RUN cp /usr/share/zoneinfo/America/New_York /etc/localtime
RUN date