# To be run from the root of the repository so that we can pick up design-system too

FROM node:12

WORKDIR /app
ADD package.json package.json
ADD yarn.lock yarn.lock
ADD lerna.json lerna.json
ADD . .
RUN yarn install --frozen-lockfile
WORKDIR /app/packages/www
CMD yarn run start
