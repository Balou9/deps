FROM node:22.17.0-alpine

RUN apk update && \
    apk add --no-cache pngcrush \
    rm -rf /var/cache/apk/*

WORKDIR /workdir

ENTRYPOINT ["/usr/bin/pngcrush"]
CMD ["-ow", "-brute", "-reduce", "-rem", "allb"]