# GoIndex-theme-nexmoe

主题基于 [yanzai/goindex](https://github.com/yanzai/goindex)


## 预览
![light](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.0/screenshot/light.jpg)
![dark](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.0/screenshot/dark.jpg)

nexmoe:  [demo.zgh.workers.dev/](https://demo.zgh.workers.dev/)

## 部署
1. 打开下列任意网址
- https://install.kenci.workers.dev/
- https://goindex.glitch.me/
- https://goindex-install.herokuapp.com/
- https://goindex-quick-install.glitch.me/
2. 授权并获取代码，把获取到的 `client_id` `client_secret` `refresh_token` ，填入模板
3. 将代码部署到 [Cloudflare Workers](https://www.cloudflare.com/)

## 自定义
```bash
themeConfig			//主题配置
	url				//仓库地址
	theme			//主题 ( light:亮色 | dark:深色 )
	main_color		//主色调
	accent_color	//强调色
	avatar			//导航栏头像
	bimg			//背景图片
	menu_show		//是否显示菜单
	menus			//菜单组
	name			//名称
	url			//地址
```

## 更新日志

### v2.0.0
- 之前的版本不在适用
- 界面进行了一定的修改，使其更加的美观
- 添加了一些的自定义，使用更加简单
- 添加了亮色和深色的主题