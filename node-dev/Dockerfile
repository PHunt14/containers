FROM node:lts-alpine

RUN apk update \
    && apk upgrade \
    && apk --no-cache add \
        git curl yq jq bash-completion mandoc\
    && source /etc/bash/bash_completion.sh \
    && rm -rf /var/cache/apk/*

ENTRYPOINT [ "/bin/bash" ]