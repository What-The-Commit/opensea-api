# How to use

First include ethers in your header
```html
<script src="https://cdn.ethers.io/lib/ethers-5.5.3.umd.min.js" type="application/javascript"></script>
```

Then include opensea-api.js either from jsDelivr or by yourself
```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/What-The-Commit/opensea-api@v1.0.0/opensea-api.min.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/What-The-Commit/opensea-api@v1.0.0/opensea-api.js"></script>
<script type="text/javascript" src="opensea-api.js"></script>
```

Creating an instance
```js
const openseaApi = new OpenseaApi(ethers.utils);
```

Creating an instance with an api key
```js
const openseaApi = new OpenseaApi(ethers.utils, 'your-api-key');
```

General communication with opensea api
```js
const openseaApi = new OpenseaApi(ethers.utils);
openseaApi._doFetch('your-request-string', {'optional-request-config-object'})
```