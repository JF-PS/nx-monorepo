helllo

nx run next-app:build:production

heroku create -a next-app-nx-monorepo

heroku buildpacks:add -a next-app-nx-monorepo heroku/nodejs

heroku buildpacks:add -a next-app-nx-monorepo heroku-community/multi-procfile

heroku config:set -a next-app-nx-monorepo PROCFILE=apps/next-app/Procfile

heroku config:set -a next-app-nx-monorepo PROJECT_NAME=next-app
