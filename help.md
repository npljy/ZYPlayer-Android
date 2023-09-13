**本软件不使用任何敏感权限都可拒绝。所有资源均来自互联网，本软件仅供学习参考使用。**
有任何问题可先尝试重装最新版
[1.青少年模式](#1)
[2.搜索方法](#2)
[3.单个添加视频源](#3)
[4.批量添加视频源](#4)
[5.无法播放,无法全屏](#5)
[6.DLNA投屏](#6)
[7.隐私权限问题](#7)
[8.数据备份和分享](#8)
[9.关于广告](#9)
<span class="an" class="" id="1"></span>
**1. 青少年模式**
此模式下屏蔽部分内容。
内置过滤词已尽可能过滤所有，但并不能保证完全过滤。可自添加过滤词。

<span class="an" class="" id="2"></span>
**2. 搜索方法**
并不是智能搜索，所以搜索的时候，尽量少字，不能有错字。
比如搜索“西行纪第四季”，如果资源站的名字是“西行纪第4季”，那么就搜不到，所以尽量之搜索名字，比如搜索“西行纪”即可

<span class="an" id="3"></span>
**3. 自己添加视频源**
请点击看这篇文章[如何添加、导入、分享视频资源站](https://mp.weixin.qq.com/s/2w_ULaQxF58hAMKxf_yUrA)

>部分视频源包含大量 违规违法 资源, 请用户自行甄别；请勿非法传播下载 违规违法 资源, 后果自负。

<span class="an" id="4"></span>
**4. 批量添加视频源JSON格式。**
  
  **不要什么都往里面导入，json格式必须符合，否则无效。不会的就一条一条导入吧。**

  >部分视频源包含大量 违规违法 资源, 请用户自行甄别；请勿非法传播下载 违规违法 资源, 后果自负。

```json
  // 左右滑动查看完整内容
  [
    {
      "name": "[必填]源站名称",
      "api": "[必填]源站地址,MacCMS10格式的api",
      "type":"接口类型，默认xml类型，可选：json",
      "group": "写“18+”可用于青少年模式过滤,其他分类可不填",
      "needjx": "[选填]取值 true|false,是否始终使用解析,针对加密源、官源,如果源站有m3u8格式,则为false,源站如果有m3u8加速解析接口直接填写jiexiUrl即可",
      "jiexiUrl": "[选填]解析接口地址,源站提供的解析接口",
      "download": "[选填]下载接口地址,MacCMS10格式的api"
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

<span class="an" id="5"></span>
**5. 资源加载不出来、视频无法播放、无法全屏**

  1. 一般是资源网服务器不稳定，或者资源网屏蔽了IP，带宽具有地域性，不同地区限制不同，请尝试切换到其他视频源，

  2. 某些源站的大分类（如：连续剧），并没有数据，遇到此问题，请切换到具体的分类（如：国产剧）即可

  3. 视频播放页面和播放器本身都是全屏

<span class="an" id="6"></span>
**6. 关于DNLA投屏**
DNLA投屏不稳定，故提供m3u8地址，可使用m3u8下载工具自行下载，后可使用本地播放方式进行投屏。

<span class="an" id="7"></span>
**7. 隐私权限问题**

* 本软件仅供学习参考。所有资源均来自互联网。
* **不收集任何隐私，可关闭任何权限，所有用户数据都保存在手机端**。
* **不会自启动，不会私自启动三方应用，[点击广告除外,此种属于主动触发]**。
* 部分视频播放页面是资源站的，**不可控**。会有统计代码和广告代码。

<span class="an" id="8"></span>
**8. 数据备份**

* **仅为方便使用，不要过分依赖备份，仅为临时存储，请及时导入和恢复数据。**
* 数据备份是将数据加密后(如下图)备份至云端，用于恢复数据。删除云端备份，会彻底删除。
![https://laonongmin.online](https://s4.ax1x.com/2021/12/24/Tt3FZd.png)

<span class="an" id="9"></span>
**9. 关于广告**
默认有广告，来自腾讯和快手，正规渠道。
> **视频打开后出现的任何广告,包括但不限于：横幅，片头，片中，片尾，下载、启动(快)应用 等都属于源站，与本应用无关！安全性不保证！不要相信!!!**。

<span class="an" id="10"></span>
**10. 内置数据来源**
[[内置视频源](https://github.com/npljy/video-resource)] 均搜自互联网
[内置漫画源] 来自互联网