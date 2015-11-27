# Self Ghost Blog 
---------------------------------
个人博客 http://blog.iphilip.net
---------------------------------

Ghost 作为一个博客平台，最大的优势就在于写博客变得如此简单方便，没有任何后台管理、没有任何载入后台的等待，更重要的是，不需要用户自己再去操心购买服务器的事了。
Ghost 的内容写作及编辑就和 Email 的体验差不多，界面左边是编辑器，右边则是页面预览，添加标签等等细节功能都如此方便。

---------------------------------
部署于Linux
---------------------------------

``安装 Node.js``

可以通过从 http://nodejs.org 下载 .tar.gz 存档或者是通过包管理器安装(like "apt-get install xx"||"yum install xx")
通过在终端窗口中输入 node -v 和 npm -v检查 Node 和 npm 是否安装成功

``安装并运行 Ghost``

登录到 http://ghost.org，然后点击蓝色的 'Download Ghost Source Code' 按钮
在下载页，点击下载最新的 zip 压缩文件然后将文件解压到你想运行 Ghost 的地方

如果你以 guest 身份登陆的 linux 或者以 SSH 远程连接只有终端，那么：
使用以下命令下载 Ghost 的最新版：

```$ curl -L https://ghost.org/zip/ghost-latest.zip -o ghost.zip```
使用以下命令解压存档：

```$ unzip -uo ghost.zip -d ghost```
在你解压好之后，打开一个终端：

切换到刚才解压的 Ghost 文件夹目录下

```$ cd /你的 Ghost 解压目录```
输入以下命令安装 Ghost ：

```npm install --production```
注意是两个 -

在 npm 结束安装后，输入以下命令让 Ghost 以开发模式启动：

```$ npm start```
```Ghost 将会运行在 127.0.0.1:2368  你可以在 config.js 中修改IP地址和端口```

```在浏览器中，访问 127.0.0.1:2368 即可查看最新搭建的 Ghost 博客```

```访问 127.0.0.1:2368/ghost 并且设置管理员用户并登陆 Ghost 管理员```

个人部署于ECS上,因此可以参考这篇很全: http://www.ghostchina.com/install-ghost-on-ali-ecs-forth-step-install-ghost/
