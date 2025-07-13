FROM mcr.microsoft.com/devcontainers/universal:2

# Install Graphviz
RUN apt-get update \
    && apt-get install -y graphviz \
    && rm -rf /var/lib/apt/lists/*

# Install Java via SDKMAN
RUN curl -s "https://get.sdkman.io" | bash \
    && bash -c "source $HOME/.sdkman/bin/sdkman-init.sh && \
    sdk install java 17.0.8-tem && \
    sdk default java 17.0.8-tem"

# Install JHipster
RUN npm install -g generator-jhipster
