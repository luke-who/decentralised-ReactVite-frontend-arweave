# Permanently deploy a decentralized React frontends to Arweave

We will be building a very simple React app that lets people connect their wallets, and deploy it to [Arweave](https://www.arweave.org/).

## Requirement
* [Vite](https://vitejs.dev/): [Next.js](https://nextjs.org/) is basically a server that serves webpages. We use Vite instead of Next.js because Vite runs fully on the client-side i.e. in the browser. For a frontend to be really decentralized, it should ideally be running fully on the client.

* [Node.js](https://nodejs.org/en/): Node.js is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser, which was designed to build scalable network applications

* [Yarn](https://yarnpkg.com/): A package manager for JavaScript

* [RainbowKit](https://www.rainbowkit.com/): For connecting a wallet

## Project setup with Vite+Yarn:
[![demo](https://asciinema.org/a/7SitAl8xVY1AOcIosChAoDfiz.svg)](https://asciinema.org/a/7SitAl8xVY1AOcIosChAoDfiz)

Now the app will be live on [http://localhost:3000](http://localhost:3000)

## Building out the UI
* Modify `main.jsx` & `App.jsx` to change the conten,layout and functionality of our app.
* Modify `vite.config.js` & `package.json` to change the configuration and dependency of our app.

In a new terminal 

[![demo](https://asciinema.org/a/504386.svg)](https://asciinema.org/a/504386)

After this make sure `wallet.json` is created at the root of your project. The `wallet.json` file contains the seed phrase/private key for your Arweave wallet so let's make sure it does not get committed to Git:

```
   echo "wallet.json" >> .gitignore
```

## Arweave deployment
Now run `yarn deploy` at the root of your project to deploy our react app!

This page will now live on Arweave FOREVER. Current url:https://arweave.net/M-dpxq6UhWzKagvu1CedA8hMBULprkK2wVnmFdRMclA

Footnote: original tutorial can be found [here](https://mirror.xyz/dhaiwat.eth/NV--7dv8CO0NCcFCvRjDCxBe3VuxdB2_KggwFEfLGRc?utm_source=tldrnewsletter)
