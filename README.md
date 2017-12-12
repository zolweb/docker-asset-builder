# Asset builder

This repository contains Dockerfile(s) to have a docker image to build assets with gulp, npm, bower, yarn ...

See docker hub image asset-builder

See https://nodejs.org/en/download/ to check npm version coming with node

| Version | Docker                       | NPM   | Bower | Gulp  |
|:-------:|:----------------------------:|:-----:|:-----:|:-----:|
| 1.0     | node:8.9.3-slim (latest LTS) | 5.5.1 | 1.8.2 | 3.9.1 |

### How to use it : 

```bash
docker run --rm --tty --volume $(PWD):/data # Mount your directory
```

You can use the option `--user` from docker run command to avoid permissions problems on generated files

This image extends from [node docker image](https://hub.docker.com/_/node/), you can refer to it for more informations