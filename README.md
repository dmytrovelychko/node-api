## Overview

Simple API for manage information about organizations: names and relations.
Built with Express.js - 4.15.2 for Ubuntu servers.

Available endpoints:

POST /api/organizations
GET /api/organizations/:name/relations

### Features

- Detect organizations related to itself, return 422 http status code
- Uses [http-status](https://www.npmjs.com/package/http-status) to set http status code.
- Uses docker-compose to run app in containers
- Uses yuidoc to auto generate documentations


## Getting Started

Clone the repo:
```sh
git clone git@github.com:dmitriyvelichkodev/node_api.git
cd node_api
```

Install docker:
https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#uninstall-docker-ce

Install docker-compose:
https://docs.docker.com/compose/install/#install-compose

Install yuidoc globally(If need regenerate documentation):
```js
npm install -g yuidoc
```

Build and run containers:
```sh
docker-compose up

# In webserver container available options for running are:
npm start - sets NODE_ENV to `development`
npm test - sets NODE_ENV to `test`
npm prod - sets NODE_ENV to `production`

By default container runs with npm start.


Tests:



## License
This project is licensed under the [MIT License]

## Meta
