# goIndex-theme-nexmoe

基于 [盘ta](https://github.com/Hidove/goindex) 的js,参考OneIndex的主题nexmoe,魔改美化.

app-v3.js 是基于[yanzai](https://github.com/yanzai/goindex)的js美化的，支持多盘、搜索、分页加载和调用外部播放器等功能，另外添加了DPlayer播放。

app-v3.js 的模板为GoIndex_v2.js


# 使用

1.打开 https://install.kenci.workers.dev/ 网站,验证并获取代码

2.使用对应app.js的模板代码，将获取到的id和授权填入

3.将代码部署到 [Cloudflare Workers](https://www.cloudflare.com/)

4.使用 https://cdn.jsdelivr.net/gh/5MayRain/goIndex-theme-nexmoe@1.1.2/app-v2.js 替换获取代码中的js
> var html = `
> 
> ......
> <script src="替换"></script>
> 
> ......
> 
> `;

5.其中app.js有部分链接为外链，app-v2.js的所有链接均连接仓库中的文件

6.app-v3.j地址：https://cdn.jsdelivr.net/gh/5MayRain/goIndex-theme-nexmoe@1.1.6/app-v3.js

7.[详细教程](https://5mayrain.github.io/posts/%E6%95%99%E7%A8%8B/%E4%BD%BF%E7%94%A8goindex%E6%90%AD%E5%BB%BAgoogledrive%E7%BD%91%E7%AB%99%E7%9B%AE%E5%BD%95/)

# 预览
[app-v2.js](https://go.zgh.workers.dev/) 

[app-v3.js](https://demo.zgh.workers.dev/) 
