<p align="center"><img src="images/ss.png"></p>

# goIndex-theme-nexmoe

Based on panta js, refer to OneIndex's theme nexmoe, magic change beautification.

App-v3.js is based on yanzai's js beautification, supports features such as multi-disk, search, pagination and call-to-external player, plus DPlayer playback.

This is just a English translation of the theme by @5MayRain : [Repo](https://github.com/5MayRain/goIndex-theme-nexmoe) </br>
All credits goes to him/her.

### How to Use
1. Open https://install.kenci.workers.dev

2. Complete authorisation and input all the details and generate code

3. Head over to the index.js file and input the client id ,client secret, refresh token and root id from the code generated in step 2

4. Deploy this index.js code to Cloudflare Workers

### Extra Options
``` js
const uiConfig = {
  .......
  "avatar": "https://i.ibb.co/jW0TDZH/image.png",  // Changes the avatar image in the navbar
  "disable_navicon": true // Disables useless nav menu in navbar
  .......
};
```
