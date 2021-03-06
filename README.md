**Inactive Project:** I've stopped using this project in favor of running fidelius on Heroku

dock0/fidelius
=======

[![Automated Build](https://img.shields.io/docker/build/dock0/fidelius.svg)](https://hub.docker.com/r/dock0/fidelius/)
[![Build Status](https://img.shields.io/travis/com/dock0/fidelius.svg)](https://travis-ci.com/dock0/fidelius)
[![MIT Licensed](http://img.shields.io/badge/license-MIT-green.svg)](https://tldrlegal.com/license/mit-license)

Container to run [fidelius](https://github.com/akerl/fidelius), a web app that checks for password security.

## Usage

```
docker pull dock0/fidelius
docker run -d -p 80:80 -e "REDIS_URL=redis://user:password@host:port/db" dock0/fidelius
```

Make sure that REDIS_URL is accessible for the container

I'd recommend using [dock0/redis](https://github.com/dock0/redis), but I'll admit to being a bit biased.

## License

This repo is released under the MIT License. See the bundled LICENSE file for details.

