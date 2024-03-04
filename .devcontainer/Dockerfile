ARG VARIANT="20"
FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-${VARIANT}

# install some useful tools
RUN apt-get update && apt-get -y install --no-install-recommends curl git sqlite3

# Install SAP CAP SDK globally by using user node. 
# User `node` is created for 20 variant of miscosoft development docker
USER node
RUN npm install -g @sap/cds-dk
WORKDIR /home/node
