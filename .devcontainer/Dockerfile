FROM jetpackio/devbox:latest

WORKDIR /code
USER root:root
RUN mkdir -p /code && chown ${DEVBOX_USER}:${DEVBOX_USER} /code
USER ${DEVBOX_USER}:${DEVBOX_USER}
COPY --chown=${DEVBOX_USER}:${DEVBOX_USER} devbox.json devbox.json

RUN devbox run -- echo "Installed Packages." && \
    devbox shellenv --init-hook >> ~/.profile && \
    nix-collect-garbage && \
    rm -rf /tmp/* /var/tmp/*
