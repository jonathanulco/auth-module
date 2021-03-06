# Auth0 Provider

[Source Code](https://github.com/nuxt-community/auth-module/blob/dev/lib/providers/auth0.js)

[Auth0](https://auth0.com) is a great authentication-as-a-service platform for free!

## Usage

```js
auth: {
  strategies: {
    auth0: {
      domain: 'domain.auth0.com',
      client_id: '....'
    }
  }
}
```

Anywhere in your application logic:

```js
this.$auth.loginWith('auth0')
```

User will be redirected to a page like this:

<img align="center" src="https://cdn2.auth0.com/docs/media/articles/web/hosted-login.png">


💁 This provider is based on [oauth2 scheme](../schemes/oauth2.md) and supports all scheme options.

### Obtaining `client_id` and **`domain`**

This options are **REQUIRED**. Your application needs some details about this client to communicate with Auth0. You can get these details from the Settings section for your client in the [Auth0 dashboard](https://manage.auth0.com).

<img align="center" src="https://cdn2.auth0.com/docs/media/articles/dashboard/client_settings.png">
