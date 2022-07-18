# Kinde Starter Kit - Express.JS

To get started set up an account on [Kinde](https://app.kinde.com/register).

## Setup your local environment

Install dependencies with `npm i`

Make a copy of `.env-sample` and name it simply `.env`. Rename the value of the `KINDE_DOMAIN` environment variable to be the subdomain you set up on Kinde and the `KINDE_SECRET` variable to be the secret found on your Kinde settings page.

## Set your Callback and Logout URLs

Your user will be redirected to Kinde to authenticate. After they have logged in or registered they will be redirected back to this application.

You need to specify in Kinde which url you would like your user to be redirected to.

In the Kinde admin UI set `Redirect url` to `http://localhost:3000/kinde_callback` and Logout url to http://localhost:3000/.

Important! This is required for your users to succesfully log in to your app.

You will also need to set the Url they will be redirected to upon logout.

## Start the app

`npm start`
