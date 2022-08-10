FROM dtzar/helm-kubectl:latest
RUN apk add --no-cache gpg gpg-agent \
  && helm plugin install https://github.com/jkroepke/helm-secrets --version v3.12.0
COPY --from=mozilla/sops:v3.6.0-alpine /usr/local/bin/sops /usr/bin/sops
COPY kubedog /usr/bin/kubedog
