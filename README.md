<!-- # GoIndex-theme-nexmoe -->

主题基于 [yanzai/goindex](https://github.com/yanzai/goindex)


## 预览
![light](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.2/screenshot/light.jpg)
![dark](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.2/screenshot/dark.jpg)
![caption](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.2/screenshot/caption.jpg)
![thumbnails-dplayer](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.2/screenshot/thumbnails-dplayer.jpg)
![thumbnails-plyr](https://cdn.jsdelivr.net/gh/5MayRain/GoIndex-theme-nexmoe@2.0.2/screenshot/thumbnails-plyr.jpg)

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
themeConfig				//主题配置
	url				//仓库地址
	theme				//主题 ( light:亮色 | dark:深色 )
	main_color			//主色调
	accent_color			//强调色
	avatar				//导航栏头像
	bimg				//背景图片
	menu_show			//是否显示菜单
	menus				//菜单组
		name			//名称
		url			//地址
```

## 获取团队盘
- [https://td.hackgence.com/](https://td.hackgence.com/)
- [https://team.hackgence.com/](https://team.hackgence.com/)

## 更新日志

### v2.0.2
- 支持缩略图
- DPlayer 缩略图名必须为 `thumbnails.jpg` [预览](https://demo.zgh.workers.dev/1:/Video/Live/%E5%8D%97%E6%9D%A1%E7%88%B1%E4%B9%83%20-%20Only%20My%20Railgun/%E5%8D%97%E6%9D%A1%E7%88%B1%E4%B9%83%20-%20Only%20My%20Railgun.flv?a=view)
- Plyr 缩略图文件名必须为 `thumbnails.vtt` [预览](https://demo.zgh.workers.dev/1:/Video/Live/%E5%8D%97%E6%9D%A1%E7%88%B1%E4%B9%83%20-%20Only%20My%20Railgun/%E5%8D%97%E6%9D%A1%E7%88%B1%E4%B9%83%20-%20Only%20My%20Railgun.mp4?a=view)
- 缩略图要和视频处于同一个目录下
- 缩略图生成 [Plyr](https://github.com/radiantmediaplayer/rmp-create-vtt-thumbnails) [DPlayer](https://github.com/MoePlayer/DPlayer-thumbnails)
- 修复部分 BUG

### v2.0.1
- 添加 Plyr 播放器
- 支持播放 `hls` [预览](https://demo.zgh.workers.dev/1:/Video/Live/LiSA%20-%20Rising%20Hope/LiSA%20-%20Rising%20Hope.m3u8?a=view)
- 支持播放 `flv` [预览](https://demo.zgh.workers.dev/1:/Video/Live/%E5%8D%97%E6%9D%A1%E7%88%B1%E4%B9%83%20-%20Only%20My%20Railgun/%E5%8D%97%E6%9D%A1%E7%88%B1%E4%B9%83%20-%20Only%20My%20Railgun.flv?a=view)
- 支持外挂字幕，字幕仅支持 `Webvtt` 格式 [预览](https://demo.zgh.workers.dev/1:/Video/Movie/%E9%A6%99%E6%B8%AF/%E6%91%A9%E7%99%BB%E4%BB%99%E5%B1%A5%E5%A5%87%E7%BC%98/%E6%91%A9%E7%99%BB%E4%BB%99%E5%B1%A5%E5%A5%87%E7%BC%98.mp4?a=view)
- 字幕文件名必须和视频名相同，且处于同一个目录下
- 视频封面的格式需为 `jpg` ，名字需和视频名相同，且处于同一个目录下
- DPlayer 字幕不可用
- 仅 `hls` 和 `flv` 使用 DPlayer 播放，其它使用 Plyr 播放 

### v2.0.0
- 之前的版本不在适用
- 界面进行了一定的修改，使其更加的美观
- 添加了一些的自定义，使用更加简单
- 添加了亮色和深色的主题

