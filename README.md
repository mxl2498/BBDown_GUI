# BBDown
一款命令行式哔哩哔哩下载器. Bilibili Downloader.

# 下载
https://github.com/mxl2498/BBDown_GUI/releases

# 开始使用
目前测试版的命令行参数支持情况
```
BBDown:
  BBDown是一个免费且便捷高效的哔哩哔哩下载/解析软件.

Usage:
  BBDown [options] <url> [command]

Arguments:
  <url>    视频地址 或 av|bv|BV|ep|ss

Options:
  -tv, --use-tv-api                  使用TV端解析模式(不支持版权内容)
  -hevc, --only-hevc                 下载hevc编码
  -info, --only-show-info            仅解析不下载
  -hs, --hide-streams                不要显示所有可用音视频流
  -ia, --interactive                 交互式选择清晰度
  -mt, --multi-thread                使用多线程下载
  -p, --select-page <select-page>    选择指定分p或分p范围
  -c, --cookie <cookie>              设置字符串cookie用以下载网页接口的会员内容
  --version                          Show version information
  -?, -h, --help                     Show help and usage information

Commands:
  login    通过APP扫描二维码以登录您的账号
```

# 功能
- [x] 番剧下载(Web)
- [x] 普通内容下载(Web|TV) `(TV接口可以下载部分UP主的无水印内容)`
- [x] 多分P自动下载
- [x] 选择指定分P进行下载
- [x] 选择指定清晰度进行下载
- [x] 下载外挂字幕并转换为srt格式
- [x] 自动合并音频+视频流+字幕流
- [x] 二维码登录账号
- [x] **多线程下载**

# TODO
- [ ] 支持更多自定义选项
- [ ] 支持旧flv资源解析
- [ ] 其他的懒得写了

# 更新日志
* 2020年7月31日 23:35  
  修复不二压视频只显示一个清晰度的问题  
  鉴于部分视频没有返回正确的字典，程序从此开始采用本地化DIC  
  支持下载无音频的稿件  
  其他优化  
  
* 2020年7月31日 19:07  
  修复无法加载cookie的问题  
  
* 2020年7月31日 0:02  
  增加二维码登录并支持本地存储cookie

* 2020年7月30日 10:40  
  修复不删除空文件夹的问题  
  对cmcc的cdn禁用多线程下载  
  
* 2020年7月30日 8:04  
  多线程优化进度反馈  
  多线程缩短超时时间  
  多线程最高8线程
  
* 2020年7月29日 21:32  
  修正`-info`的逻辑  
  修复某些电影无法下载的问题  
  临时文件存放至单独文件夹  
  增加多线程下载逻辑  
  
* 2020年7月28日 13:50  
  继续优化最高清晰度的自动选择逻辑  
  成为标准化的命令行程序  
  支持bv小写链接  
  支持ss链接解析  
  
* 2020年7月27日 22:49  
  优化最高清晰度寻找算法  
  支持选择分P下载  
  加入`-help`命令
  
* 2020年7月27日 20:29  
  更改解析接口，修复有时候获取不到分辨率编码等问题  
  修复分P下载异常问题  
  开始显示所有流信息
  
* 2020年7月27日 0:15  
  修复部分番剧无法下载问题
  
* 2020年7月26日 23:33  
  支持字幕自动封装
  
* 2020年7月26日 19:50  
  发布公测
