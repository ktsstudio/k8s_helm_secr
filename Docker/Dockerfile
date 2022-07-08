FROM dtzar/helm-kubectl:latest

RUN helm plugin install https://github.com/jkroepke/helm-secrets --version v3.12.0

COPY sops /usr/bin/sops
