FROM alpine:latest
# RUN curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
# RUN chmod 700 get_helm.sh 
# RUN ./get_helm.sh
RUN apk update \
    && apk upgrade \
    && apk --no-cache add \
        helm terraform git curl yq jq nodejs npm bash-completion aws-cli mandoc\
    && source /etc/bash/bash_completion.sh \
# install kubectl
    && curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" \
    && install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl \
    && rm -rf /var/cache/apk/*
