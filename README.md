## Fox Finance
Fox Finance is a deflationary reflection token on the Binance Smart Chain that joins investors, innovative decentralized products, and the wild world around us in a common mission.

![foxfinance io_Marketplace](https://user-images.githubusercontent.com/105137625/194287145-ae053038-0a87-4b38-9d6f-dce1dbb113dd.png)

## Build Setup Testing
### Live: https://shop.foxfinance.io/
```bash
# create .env file locally from development.env
$ cp development.env .env

# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# generate static project to deploy to production
$ npm run generate

# upload to Amazon s3
$ aws s3 sync dist s3://fox-market

# clear cloudfront cache
$ aws cloudfront create-invalidation \
    --distribution-id E3MHC1NKTPE0P2 \
    --paths "/" "/homepage" "/homepage/" "/contribution-success" "/contribution-success/"
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
