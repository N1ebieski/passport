# passport.local

Frontend implementation of authentication [by Laravel Passport](https://github.com/N1ebieski/api.passport.local) in Vue Nuxt.JS application. 

## Important things

.ENV config (my config in .env.example):

1. AUTH_URL must contains domain with root path to backend api (there are my endpoints of authentication)
2. API_URL must contains domain with path to backend api

nuxt.config.js file:

1. axios automatically places Authorization Bearer Token (from auth._token.local cookie) in Header for any request
2. 'auth.strategies.local.user' property must be set false

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
