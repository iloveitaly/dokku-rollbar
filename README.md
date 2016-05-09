# Dokku Rollbar

Dokku Rollbar is a plugin for [Dokku](https://github.com/progrium/dokku) that notifies Rollbar of deployments.

This dokku plugin could be easily modified to support other error trackers (Sentry, etc).

## Installation

Verified to work on dokku 0.5+, will probably work without modification on early dokku versions.
```sh
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
* https://github.com/nickstenning/dokku-webhooks

## [License](LICENSE)
