FROM nginx:mainline-alpine
ENV TZ=America/New_York
RUN apk add -U tzdata curl bash
RUN cp /usr/share/zoneinfo/America/New_York /etc/localtime
RUN date

HEALTHCHECK --interval=60s --retries=5 CMD curl --fail http://localhost || exit 1