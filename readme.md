# Graphicsmagick buildpack for Dokku

A Buildpack for [dokku](https://github.com/progrium/dokku) that installs graphicsmagick in your dokku container

Designed to used with [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi) that allow multiple buildpacks to be used together.

# Usage

Create a .env file in the root of your git repo with the following contents:

```
export BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git
```

Again, in the root of your repo, add a .buildpacks file containing:

```
https://github.com/heroku/heroku-buildpack-nodejs.git#v60
https://github.com/unclouded/dokku-buildpack-graphicsmagick.git#v1
```

(yeah i know it's not pretty fixing the heroku build pack — needs to be a cleaner way to use the same buildpack in dokku — something for the future).
