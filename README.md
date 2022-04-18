> _⚠️ GitHub & Heroku have turned off their integration while investigating a [breach](https://github.blog/2022-04-15-security-alert-stolen-oauth-user-tokens/), so changes will not automatically deploy after pushing to `master`. If you have access to do so, please [push your changes to the `master` branch of the Heroku git remote](https://devcenter.heroku.com/articles/git) once your PR is merged. Otherwise, please mention it in the PR and assign [@maxwofford](https://github.com/maxwofford) for review._

<h1 align="center">Airbridge</h1>
<p align="center">
  <a href="https://github.com/hackclub/airbridge/actions">
    <img alt="test" src="https://github.com/hackclub/airbridge/workflows/test/badge.svg">
    <img alt="format" src="https://github.com/hackclub/airbridge/workflows/format/badge.svg">
  </a>
</p>
<p align="center"><i>The bridges tying Hack Club's services together. (WIP) Illustrated below by <a href="https://gh.maxwofford.com">@maxwofford</a>.</i></p>
<p align="center"><img alt="Raft icon" src="https://cloud-gxlnkdt57.vercel.app/0untitled.png"></a>

## Reasoning

Our [previous API](https://github.com/hackclub/api/blob/master/README.md) was really good at a couple things. It hasn't been touched in years and it's still providing password-less authentication as a service at scale.

Hack Club (HQ & community) needs a service for easily reading & writing information that will last the test of time the same way our original API still handles authentication. Airbridge will create this by providing a JSON interface to an Airtable backend.

## Try the latest version here: [v0.1](./src/v0.1/README.md)

Version list:

- [v0.2 (in development)](./src/v0.2/README.md)
- [v0.1](./src/v0.1/README.md)
- [v0](./src/v0/README.md)

## Developing & Contributing

```sh
# Set it up locally
git clone https://github.com/hackclub/airbridge && cd airbridge
yarn

# Run locally with nodemon
yarn dev # then, go to localhost:5000/ping in your browser

# Run tests
yarn test

# Run specific tests
yarn test tests/v0/routes.test.js # (your choice of testfile here)
```
