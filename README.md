# Dokku Rollbar

Dokku Rollbar is a plugin for [Dokku](https://github.com/progrium/dokku) that notifies Rollbar of deployments.

## Installation

```sh
# dokku 0.4+
$ dokku plugin:install https://github.com/iloveitaly/dokku-rollbar.git
```

The plugin pulls the Rollbar access token from your app's `ROLLBAR_TOKEN` and
your environment from `RAILS_ENV`. The app environment will default to `production`
if `RAILS_ENV` is not found

## Commands

No commands. If `ROLLBAR_TOKEN` is set, Rollbar will be notified of each deploy.

## Inspiration

* https://github.com/Flink/dokku-airbrake-deploy
* https://github.com/ribot/dokku-slack

## [License]
