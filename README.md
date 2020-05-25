# goIndex-theme-nexmoe

Based on panta js, refer to OneIndex's theme nexmoe, magic change beautification.

App-v3.js is based on yanzai's js beautification, supports features such as multi-disk, search, pagination and call-to-external player, plus DPlayer playback.

This is just a English translation of the theme by @5MayRain : [Repo](https://github.com/5MayRain/goIndex-theme-nexmoe) </br>
All credits goes to him/her.

Use
1. Open the https://install.kenci.workers.dev/ website, verify and get the code

2. Use the template code for the corresponding app.js, and fill in the id and authorization obtained

3. Deploy code to Cloudflare Workers

4. Replace the js in the get code with https://rawcdn.githack.com/icodelifee/goIndex-theme-nexmoe/d5f6a22701b3308e93d6b0db73a21c4f51b407f8/app_v3_en.js

``` js
var html = '
......
<script src="https://rawcdn.githack.com/icodelifee/goIndex-theme-nexmoe/d5f6a22701b3308e93d6b0db73a21c4f51b407f8/app_v3_en.js"></script>
......
`;
```

### Extra Options
``` js
const uiConfig = {
  .......
  "avatar": "https://i.ibb.co/jW0TDZH/image.png",  // Changes the avatar image in the navbar
  "disable_navicon": true // Disables nav menu in navbar
  .......
};
```
