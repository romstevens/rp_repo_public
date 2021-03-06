# RP Repo

A simple hosting site for play-by-post roleplays. Made by me!

## Demo
Check out the demo at https://repodemo.herokuapp.com/.

Please only post nice things on the demo, I don’t want to monitor it ;)

Log in with one of the following test accounts:
- fighter@example.com / password
- wizard@example.com / password
- rogue@example.com / password

## Project setup

1. `gem install bundler`
1. `bundle`
1. `rails db:create db:migrate db:seed`

## Running the server

1. `redis-server`
2. `bundle exec rails s`

Log in with `user@example.com / abcd1234`.

Foreman is set up for Heroku but it doesn't have a Procfile.dev yet.

## Development
Push to `develop` branch on GitHub. Branch off features into `feature/name-of-feature` and merge them in with a PR.

## Deploying

Deploys happen automatically to Heroku when the `master` branch is updated. [More info](https://dashboard.heroku.com/apps/rp-repo/deploy/github)

For a fresh deploy, you will need to add two addons to Heroku:
- Heroku Postgres (free tier)
- Heroku Redis (free tier)

Remember to run `rake db:migrate` after deploying!
