FROM mcr.microsoft.com/devcontainers/base AS base
ENV PATH=$PATH:/opt/node-v22.11.0-linux-arm64/bin
RUN curl -L https://nodejs.org/dist/v22.11.0/node-v22.11.0-linux-arm64.tar.xz | sudo tar -xJ -C /opt \
    && npm install -g @devcontainers/cli \
    && curl -L /usr/local/bin/lazygit https://github.com/jesseduffield/lazygit/releases/download/v0.44.1/lazygit_0.44.1_Linux_arm64.tar.gz | tar xzf - -C /usr/local/bin
COPY --chown=vscode:vscode lazygit.yml /home/vscode/.config/lazygit/config.yml