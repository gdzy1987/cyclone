FROM alpine:3.8

LABEL maintainer="zhujian@caicloud.io"

ENV WORKDIR /workspace
WORKDIR $WORKDIR

RUN apk update && \
    apk add --no-cache ca-certificates git bash coreutils

COPY ./build/resolver/git/entrypoint.sh /

ENTRYPOINT ["/entrypoint.sh"]

CMD ["help"]