# Electron Test App
Example app to convert a HTML game to an electron game to deploy on steam.

## 1. Electron Forge
The following were the commands I used to get a basic Electron Forge project working from scratch:
```
npm install -g @electron-forge/cli
npx create-electron-app my-app -- --template=webpack-typescript
cd my-app
npm install @electron-forge/plugin-auto-unpack-natives --save-dev
npm install electron --save-dev
npm install
npm start
```
N.B. Replace `my-app` with the name of your project

## 2. Prepare Steam credentials
[Get Started with Steamworks](https://partner.steamgames.com/doc/gettingstarted) has a list of steps to take.
- [ ] Set Up Steamworks Account
- [ ] Download the Steamworks SDK
- [ ] Create your Steam build & depots
- [ ] Configure Steamworks features
- [ ] Creating your store page & pricing
- [ ] Preparing for Release

## 3. Build and Deploy to Steam
[Trashmoon has a great walkthrough](https://trashmoon.com/blog/2022/automating-steam-releases-for-html-games-with-electron-forge-and-github-actions/) which I referenced to get the project ready and deployed to steam.

## 4. Integrate Electron and Steam API
Greenworks is deprecated, use [Steamworks.js](https://github.com/ceifa/steamworks.js) instead. This [useful walkthrough of the process](https://liana.one/integrate-electron-steam-api-steamworks) helped.