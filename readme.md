# Kinde Starter Kit - Express.JS

## Register an account on Kinde

To get started set up an account on [Kinde](https://app.kinde.com/register).

## Setup your local environment

Clone this repo and install dependencies with `npm i`

Make a copy of `.env_sample` and name it simply `.env`. Set the following values from the Kinde `Settings -> Applications -> Backend app` page.

```
KINDE_ISSUER_URL - The Domain value
KINDE_CLIENT_ID - The client id
KINDE_CLIENT_SECRET - The client secret
```

e.g

```
KINDE_ISSUER_URL=https://your_kinde_subdomain.kinde.com
KINDE_CLIENT_ID=yourId5romKind3
KINDE_CLIENT_SECRET=some5ecretFromappKey5pag3
```

## Set your Callback and Logout URLs

Your user will be redirected to Kinde to authenticate. After they have logged in or registered they will be redirected back to your ExpressJS application.

You need to specify in Kinde which url you would like your user to be redirected to in order to authenticate your app.

On the App Keys page set `Redirect url` to `http://localhost:3000/kinde_callback`

> Important! This is required for your users to successfully log in to your app.

You will also need to set the url they will be redirected to upon logout. Set the `Logout url` to http://localhost:3000.

## Start the app

`npm start` and navigate to `http://localhost:3000`.

Click on `Sign up` and register your first user for your business! 🚀
