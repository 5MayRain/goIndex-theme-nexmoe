<!-- # GoIndex-theme-nexmoe -->

主题基于 [yanzai/goindex](https://github.com/yanzai/goindex)


## 预览
![light](https://raw.githubusercontent.com/5MayRain/goIndex-theme-nexmoe/master/screenshot/light.jpg)
![dark](https://raw.githubusercontent.com/5MayRain/goIndex-theme-nexmoe/master/screenshot/dark.jpg)
![caption](https://raw.githubusercontent.com/5MayRain/goIndex-theme-nexmoe/master/screenshot/caption.jpg)
![thumbnails-dplayer](https://raw.githubusercontent.com/5MayRain/goIndex-theme-nexmoe/master/screenshot/thumbnails-dplayer.jpg)
![thumbnails-plyr](https://raw.githubusercontent.com/5MayRain/goIndex-theme-nexmoe/master/screenshot/thumbnails-plyr.jpg)

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
### 模板
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
	view				//定义可预览的文件
	player_dp			//使用 DPlayer 播放，未填入的默认使用 Plyr 播放
	thumbnails			//缩略图组
		name			//名称
		url			//地址
	video_cover			//视频封面
	video_subtitle			//视频字幕
```

### 示例
```bash
  // 仓库地址
  "url": "//cdn.jsdelivr.net/gh/5MayRain/goIndex-theme-nexmoe",
  // 主题 ( light:亮色 | dark:深色 )
  "theme": "light", 
  // 主色
  "main_color": "blue-grey",
  // 强调色
  "accent_color": "blue",
  // 头像
  "avatar": "//cdn.jsdelivr.net/gh/5MayRain/ImageHosting/Blog/Website/avatar.png",
  // 背景图片
  "bimg": "//cdn.jsdelivr.net/gh/5MayRain/ImageHosting/Blog/Posts/2021/07/20/cover_01.jpg",
  // 显示菜单
  "menu_show": true,
  // 菜单组
  "menus": [
    {
      name: "Blog",
      url: "//mrzgh.top"
    },
    {
      name: "Log in",
      url: "//drive.google.com"
    }
  ],
  // 定义可预览的文件
  "view": "|html|php|css|go|java|js|json|txt|sh|md|mp4|webm|avi|bmp|jpg|jpeg|png|gif|m4a|mp3|flac|wav|ogg|mpg|mpeg|mkv|rm|rmvb|mov|wmv|asf|ts|flv|m3u8|",
  // 使用 DPlayer 播放，未填入的默认使用 Plyr 播放
  "player_dp": "|m3u8|flv|",
  // 缩略图组
  "thumbnails": [
    {
      name: "dplayer",
      url: "Thumbnail/dplayer.jpg"
    },
    {
      name: "plyr",
      url: "Thumbnail/plyr.vtt"
    }
  ],
  // 视频封面，${fileName} 表示当前视频的名字
  "video_cover": "${fileName}.jpg",
  // 视频字幕
  "video_subtitle": "${fileName}.vtt",
```

## 获取团队盘
- [https://td.hackgence.com/](https://td.hackgence.com/)
- [https://team.hackgence.com/](https://team.hackgence.com/)

## 更新日志
### v2.0.5
- 修复自定义头像不可用

### v2.0.4
- 修复 `${fileName} ` 参数不可用
- `${fileName} ` 参数仅适用于自定义项的`视频封面 `和`视频字幕 `

### v2.0.3
- 支持更多的自定义

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

