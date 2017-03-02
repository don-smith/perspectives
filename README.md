# Perspectives

> A static publishing platform for IPFS

## To get started

* Install the latest version of Node.js & npm.
* Install [IPFS](http://ipfs.io) and make sure `ipfs id` doesn't fail.

```sh
# In terminal window #1
ipfs daemon

# In terminal window #2
npm clone https://github.com/don-smith/perspectives
cd perspectives && npm install
./init && ./build
```

* If you're using a domain name, wire it up to IPNS using [these instructions](https://ipfs.io/ipfs/QmNZiPk974vDsPmQii3YbrMKfi12KTSNM7XMiYyiea4VYZ/example#/ipfs/QmRFTtbyEp3UaT67ByYW299Suw7HKKnWK6NJMdNFzDjYdX/websites/README.md).


## The typical workflow

* Make sure you have the IPFS daemon running: `ipfs daemon`
* Create a new markdown file inside of the `pages` folder
* Add a new hyperlink to `built/index.html`
* Run `./build` to recreate all HTML files and add them to IPFS
  - This will open your browser to the `/ipfs` path on localhost
* Run `./publish` to update the IPNS reference
  - This will open your browser to the gateway's `/ipns` path
