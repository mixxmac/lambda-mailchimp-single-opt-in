# :cloud: Mailchimp single opt-in Lambda
An Amazon Lambda function for creating MailChimp subscriptions with single opt-in.
Based on [Mailchimp Lambda](https://github.com/TaylorBriggs/mailchimp-lambda) and [Node Lambda](https://github.com/motdotla/node-lambda).

## Authentication

Set your API key and list ID in the .env file. Copy the sample to get started:

```
$ cp .env.sample .env

API_KEY=YOUR_API_KEY
LIST_ID=YOUR_LIST_ID

```

## Deployment

There's a handy script included to create your zip archive:

```
$ npm start
```

## Build (Babel ⇒ ES5)

```
$ npm run build
```

## Deploy

```
$ npm run deploy
```

```
$ curl -X POST -H "Content-Type: application/json" \
-d '{ "email": "hey@gmail.com", "first_name": "Anibal" }' \
YOUR_API_GATEWAY_URL
```
