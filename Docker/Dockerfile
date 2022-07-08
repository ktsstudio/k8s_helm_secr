FROM dtzar/helm-kubectl:latest

RUN helm plugin install https://github.com/jkroepke/helm-secrets --version v3.12.0

COPY sops /usr/bin/sops

RUN apk add --no-cache age

ENV SOPS_AGE_KEY_FILE="key.txt"
ENV SOPS_AGE_RECIPIENTS="age1x46yt595nqutgmszkh6z3acucqw9w5rzfxed6zq48g2ww26e79aq6urccz"