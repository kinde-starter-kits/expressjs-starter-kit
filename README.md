# Kinde ExpressJS Starter Kit

The Kinde Starter Kit for ExpressJS.


[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com) [![Kinde Docs](https://img.shields.io/badge/Kinde-Docs-eee?style=flat-square)](https://kinde.com/docs/developer-tools) [![Kinde Community](https://img.shields.io/badge/Kinde-Community-eee?style=flat-square)](https://thekindecommunity.slack.com)

## Development

### Initial set up

1. Clone the repository to your machine:

   ```bash
   git clone https://github.com/kinde-starter-kits/expressjs-starter-kit.git
   ```

2. Go into the project:

   ```bash
   cd expressjs-starter-kit
   ```

3. Install the dependencies:

   ```bash
   npm install
   ```

### Setup your local environment

To get started set up an account on [Kinde](https://app.kinde.com/register). Make a copy of `.env_sample` and name it simply `.env`. Set the following values from the Kinde `Settings -> Applications -> Backend app` page.

```
KINDE_ISSUER_URL - The domain value
KINDE_CLIENT_ID - The client id
KINDE_CLIENT_SECRET - The client secret
KINDE_SITE_URL - Your App's domain value
KINDE_REDIRECT_URL - Kinde will redirect here after login
KINDE_POST_LOGOUT_REDIRECT_URL - Kinde will redirect here after logout
```

e.g

```
KINDE_SITE_URL=http://localhost:3000
KINDE_ISSUER_URL=https://<your_subdomain>.kinde.com
KINDE_POST_LOGOUT_REDIRECT_URL=http://localhost:3000
KINDE_CLIENT_ID=<YOUR_CLIENT_ID>
KINDE_CLIENT_SECRET=<YOUR_CLIENT_SECRET>
KINDE_REDIRECT_URL=http://localhost:3000/kinde_callback
```

### Set your Callback and Logout URLs

Your user will be redirected to Kinde to authenticate. After they have logged in or registered they will be redirected back to your ExpressJS application.

You need to specify in Kinde which url you would like your user to be redirected to in order to authenticate your app.

On the App Keys page set `Redirect url` to `http://localhost:3000/kinde_callback`

> Important! This is required for your users to successfully log in to your app.

You will also need to set the url they will be redirected to upon logout. Set the `Logout url` to http://localhost:3000.

## Start the app

`npm start` and navigate to `http://localhost:3000`.

Click on `Sign up` and register your first user for your business! 🚀


## Contributing

Please refer to Kinde’s [contributing guidelines](https://github.com/kinde-oss/.github/blob/489e2ca9c3307c2b2e098a885e22f2239116394a/CONTRIBUTING.md).

## License

By contributing to Kinde, you agree that your contributions will be licensed under its MIT License.
