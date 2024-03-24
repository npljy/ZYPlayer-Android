# 本仓库不再维护更新。

## kk player

CMS 视频资源播放器, 兼容 zyplayer，支持 Android 和 iOS ，内置播放器 [mui-player](https://github.com/muiplayer/hello-muiplayer)  

## 学习研究

👉 [谷歌Play商店](https://play.google.com/store/apps/details?id=cn.xuehuayu.player)

## 特色

* 无登录，直接看
* 支持MAC CMS资源站，自动识别（xml，json）
* alist网盘，建议mp4格式
* 漫画阅读，来自网络
* 视频源添加，批量添加，导出
* 本地源分享、导入分享
* 数据备份、恢复
* WebDAV备份与恢复
* DLNA投屏【Android】
* 可自定义过滤词，过滤视频名称和分类
* 青少年模式，内置过滤词，如有不足，请自定义过滤词
* 深色模式，系统太古老不支持
* ~小说阅读(如有稳定资源，再上线)~
* ~电视观看(下线，失效太快)~
* ~短视频(下线，刷抖音快手去吧)~
* 三方工具：视频解析，音乐下载，热搜排行，历史价格

## 感谢

* 资源站接口参考[ZY-Player](https://github.com/Hunlongyu/ZY-Player)
* 网盘功能参考[ZyPlayer](https://github.com/Hiram-Wong/ZyPlayer)

## 声明

* 请大家支持正版. 所有资源来自互联网, 本软件不参与任何制作, 上传, 储存等内容, 禁止传播违法资源.
* 该软件仅供学习交流使用，禁止个人用于非法商业用途, 请于安装后 24 小时内删除.

## 关于隐私

* 不收集任何隐私，**可关闭任何权限**，弹出权限提示，点拒绝就是了。部分功能使用某些权限，仅用于本地操作，用到的时候再打开就行。
* 所有用户数据都保存在`手机端`（用户主动备份除外，加密存储）
* 不会自启动，不会私自启动三方应用。
* 部分视频播放页面(如：网页播放，一般非m3u8的就是)是资源站的，`不可控`。可能有统计代码或广告代码等。
* 本APP开发过程中没有添加任何统计工具和代码(没有打包相关SDK)，开发者不会知道使用者的任何操作。但uni平台，三方的SDK(如:广告)、工具(如:播放器)等有无统计和追踪,开发者并不清楚，不做保证。

## iOS版本说明

iOS版本因使用测试证书，视频更新时没有Push通知。目前通知方式为app内部吐司通知。

## 青少年模式

此模式下屏蔽部分内容。
内置过滤词已尽可能过滤所有，但并不能保证完全过滤。可自定义过滤词。

## 搜索方法

并不是智能搜索，所以搜索的时候，尽量少字，不能有错字。
比如搜索“西行纪第四季”，如果资源站的名字是“西行纪第4季”，那么就搜不到，所以尽量之搜索名字，比如搜索“西行纪”即可

## 批量添加视频源JSON格式
  
  **不要什么都往里面导入，json格式必须符合，否则无效。不会的就一条一条导入吧。**

  >部分视频源包含大量 违规违法 资源, 请用户自行甄别；请勿非法传播下载 违规违法 资源, 后果自负。

```json
  // 左右滑动查看完整内容
  [
    {
      "name": "[必填]源站名称",
      "api": "[必填]源站地址,MacCMS10格式的api",
      "type":"接口类型，默认xml类型，可选：json",
      "group": "写“18+”可用于青少年模式过滤,其他分类随意",
      // ↓ 为true，则强制使用解析,针对加密源、官源；
      // ↓ 如果源站有m3u8格式,则为false；如果想使用其加速解析接口，为false，直接填写jiexiUrl字段即可
      "needjx": "[选填] 取值 true|false，注意 无引号",
      "jiexiUrl": "[选填]解析接口地址,源站提供的解析接口,建议不填,除非不使用解析无法播放",
      "download": "[选填]下载接口地址,MacCMS10格式的api,没多大意义了,大多数资源站已不提供下载"
    },
    {
      "name": "源站1",
      "api": "http://cj.ffzyapi.com/api.php/provide/vod/",
      "type":"json",
      "group": "18+"
    },
    {
      "name": "源站2",
      "api": "http://www.605zy.co/inc/api.php",
      "needjx": true, // 取值 true|false，注意 无引号
      "jiexiUrl": "https://jx.xmflv.com/?url="
    },
    {
      "name": "源站3",
      "api": "https://www.rrzyw.cc/api.php/provide/vod/at/xml/"
    }
  ]
```

## 资源加载不出来、视频无法播放、无法全屏

  1. 一般是资源网服务器不稳定，或者资源网屏蔽了IP，带宽具有地域性，不同地区限制不同，请尝试切换到其他视频源，

  2. 某些源站的大分类（如：连续剧），并没有数据，遇到此问题，请切换到具体的分类（如：国产剧）即可

  3. 视频播放页面和播放器本身已经是全屏

## 关于DNLA投屏

DNLA投屏不稳定，故提供复制m3u8地址，可使用m3u8下载工具自行下载，后可使用本地播放方式进行投屏。

## 关于广告

默认有广告，来自正规合法合规渠道，可关闭。

**现在的广告诡的很，点点没什么，但是填写个人信息等场景，千万谨慎，遇到支付的情况，不要支付！**  
**视频打开时(加载时以及加载完成后)出现的任何广告,包括但不限于：跑马灯，横幅，片头，片中，片尾，弹窗，下载、启动(快)应用 等都属于源站，与本应用无关！安全性不保证！不要相信!!!**
