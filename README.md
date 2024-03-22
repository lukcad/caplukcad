# caplukcad

## Overview

This is template of basic container for development using SAP CAP approach. This can be donwloaded from git Hub into your workspace and enriched by your CDS projects whihc follows to recomendations from [SAP CAP](https://cap.cloud.sap/docs/about/).

Initial container includes:

* container with node.js;
* install of components: curl, git, sqlite3;
* non-root user: node
* workdir: home/node
* extensions for VS:
  * SAPSE.vscode-cds
  * dbaeumer.vscode-eslint
  * humao.rest-client
  * qwtel.sqlite-viewer
  * mechatroner.rainbow-csv
* installing globally during initializaiton container these libraries:
  * cds
  
You should clone this by command to provide your own name of docker container project:

    git clone https://github.com/lukcad/caplukcad.git <your_name_container_project>


You should open it by `VS code` as `contianer` and add into it as many as you wish CDS projects.

Use this command to add new project in container:

    cds init <your_name_project>

Use this command to add mock data into your new created project:

    cds add tiny-sample

or

    cds add data
