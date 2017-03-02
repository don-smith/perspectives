# Perspectives

> A static publishing platform for IPFS

## To get started

* Install the latest version of Node.js and npm.
* Install IPFS and make sure `ipfs id` doesn't fail.

```sh
npm clone [this repo]
npm cd perspectives
npm install

mv built/index.html.sample built/index.html
mv src/footer.html.sample src/footer.html
mv src/header.html.sample src/header.html
```

## The typical workflow

* Make sure you have IPFS running (`ipfs daemon`).
* Create a new markdown file inside `./pages`.
* Add a link to the HTML file in `./built/index.html`.
* Run `./build` to create the HTML files and add them to IPFS.
  - This will open your browser to localhost's `/ipfs` path.
* Run `./publish` to update the IPNS reference.
  - This will open your browser to the gateway's `/ipns` path.
