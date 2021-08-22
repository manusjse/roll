## roll
[![](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/manusjse/roll.git)

### Heroku deployment
- [x] support vm/vl protocol
- [x] definable ws path
- [x] homepage（3D element cycle table）
- [x] HTML5 speedtest
- [x] new version structure

request`/`，back to 3D element cycle table

![image](https://cdn.jsdelivr.net/gh/libsgh/v2ray-heroku@main/doc/1.png)

request`/speedtest/`，html5-speedtest page

![image](https://cdn.jsdelivr.net/gh/libsgh/v2ray-heroku@main/doc/2.png)

request`/test/`，file-downloading speed test

![image](https://cdn.jsdelivr.net/gh/libsgh/v2ray-heroku@main/doc/3.png)

request`/ray`（configurable）ws path


### Environmental variables explanation

|  Item | Value  | Remark  |
| ------------ | ------------ | ------------ |
|  PROTOCOL |  vm<br>vl（optional） |  protocol：nginx+vm+ws+tls or nginx+vl+ws+tls |
|  UUID |  [uuidgenerator](https://www.uuidgenerator.net "uuidonlinegenerator") | UserID  |
|  WS_PATH | deflaut`/ray` |  path，do not use`/speedtest`，`/`，`/test` etc which path alreadly occupied |
