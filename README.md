# vno-dmego-yuzr 个人主页

修改自 [dmego](https://github.com/dmego/home.github.io) 和 [vno](https://github.com/onevcat/vno-jekyll) 模板。

### 修改内容

- 删除了不明所以的头像翻页动画
- 修改了社交媒体为我个人使用的内容
- 不再使用Github Action和Bing壁纸API相关内容
- 改用随机动漫壁纸API作为背景
  - 在这里推荐[爱搜](https://imgapi.xl0408.top/index.php)和[呓喵酱](https://api.yimian.xyz/img?type=moe&size=1920x1080)的API，又快又稳，我用的是前者，后者质量更高但是风景图偏多。
- 添加了备案的页脚
- 发布了npm包，对一些你们不会修改的资源使用了unpkg加速（使用饿了么国内镜像）

## 预览

<img title="电脑界面" src="https://s2.loli.net/2023/01/13/iZE18TNtsRc5MrJ.png" alt="预览" data-align="center">

<img title="手机预览" src="https://s2.loli.net/2023/01/14/yWHAC5vDYjfnmk2.png" alt="" width="260" data-align="inline">     <img title="手机展开" src="https://s2.loli.net/2023/01/14/ujwIKPtbVJ3EzGB.png" alt="" width="260" data-align="inline">

## 使用方法

1. 下载源码或fork后本地拉取

2. 修改根目录下的 `favicon.ico` （网站图标）以及 `apple-touch-icon.jpg`（苹果手机保存到桌面的应用图标），可以使用 [PNG转ICO - 在线转换图标文件](https://www.aconvert.com/cn/icon/png-to-ico/)

3. 修改根目录下的 `\assets\img\headimg.png` 为你自己的头像，长宽比建议为1:1（正方形）

4. 修改 `index.html` 以下内容：
   
   - 修改 [L9-L12](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L9-L12) 的标题和元数据
   
   - 修改 [L30](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L30) 的链接
   
   - 修改 [L35](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L35) 的名字
   
   - 修改 [L37](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L37) 的格言（也可以设置为个人简介等）
   
   - 修改 [L47-L58](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L47-L58) 的导航栏的地址和内容
   
   - 修改 [L65-L83](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L65-L83) 的社交媒体和联系方式，如果想添加其他账号的话需要根据自己需求使用iconfont并修改，具体使用方法可以看这篇博客 -> [iconfont字体图标的使用方法--超简单! - 全堆栈溢出攻城狮 - 博客园](https://www.cnblogs.com/hjvsdr/p/6639649.html) （改完后放在对应位置，建议修改 `iconfont.css` 中 `.iconfont` 的 `font-size` 属性为 `24px`）
   
   - 修改 [L86](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L86) 的加密邮箱（防爬虫和垃圾广告），可以使用 [base64encode](https://www.base64encode.org/) 进行加密，或者改用 [L87](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L87) 的明文方式（不推荐）
   
   - 修改 [L102](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L102) 为你的Copyright和备案（如果没有可以注释掉，也可以注册一个免费的 [萌备](https://icp.gov.moe/) ）
   
   - 如果需要的话，你也可以修改 [L27](https://github.com/Mitr-yuzr/vno-dmego-yuzr/blob/master/index.html#L27) 中壁纸背景API为你的API或静态图片资源
   
   - 如果需要的话，你也可以在任意合理的位置加入Google Analytics的统计代码

5. 将修改后的网页上传至服务器，或push到自己的仓库后使用github pages等代码托管服务

### 吐槽

有一说一，最初 [vno](https://github.com/onevcat/vno-jekyll) 的页面设计非常好，[dmego](https://github.com/dmego/home.github.io) 的动效设计也不赖，但这份代码的风格，这里悄悄的基于个人的看法非常不文明且不礼貌的毫不客气的说一句：简直就是依托答辩。

或许跟我个人习惯有关，或许跟使用的框架和库有关，或许是我水平太低，或许是他代码真的写的稀烂。