FROM alpine:3.12

RUN apk add --no-cache tini
# Tini is now available at /sbin/tini
ENTRYPOINT ["/sbin/tini", "--"]

CMD /bin/sh -c 'while true; do sleep 15; done;'
