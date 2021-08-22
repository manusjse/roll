## roll
[![](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/manusjse/roll.git)

### heroku上部署
- [x] 支持vm和vl两种协议
- [x] 支持自定义ws路径
- [x] 伪装首页（3D元素周期表）
- [x] HTML5测速
- [x] 使用最新版构建

请求`/`，返回3D元素周期表

![image](https://cdn.jsdelivr.net/gh/libsgh/v2ray-heroku@main/doc/1.png)

请求`/speedtest/`，html5-speedtest测速页面

![image](https://cdn.jsdelivr.net/gh/libsgh/v2ray-heroku@main/doc/2.png)

请求`/test/`，文件下载速度测试

![image](https://cdn.jsdelivr.net/gh/libsgh/v2ray-heroku@main/doc/3.png)

请求`/ray`（可配置）ws路径


### 环境变量说明

|  名称 | 值  | 说明  |
| ------------ | ------------ | ------------ |
|  PROTOCOL |  vm<br>vl（可选） |  协议：nginx+vm+ws+tls或是nginx+vl+ws+tls |
|  UUID |  [uuid在线生成器](https://www.uuidgenerator.net "uuid在线生成器") | 用户主ID  |
|  WS_PATH | 默认为`/ray` |  路径，请勿使用`/speedtest`，`/`，`/test` 等已经被占用的请求路径 |

### 进阶
heorku可以绑卡（应用一直在线，不扣费），绑定域名，套cf，[uptimerobot](https://uptimerobot.com/) 定时访问防止休眠
