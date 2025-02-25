# MySpace 迈斯贝斯

### 前言

***自用多功能聚合软件***：

- 之前是想做一个博客用来记录，使用wordpress搭建好之后发现并没有太多内容支撑，而且发布的过程属实是麻烦，文件管理和存储也很麻烦。，就更加不想写了。

- 而且我有是一个有病的人，不喜欢发朋友圈，但又很喜欢记录。平常用来记录生活的众多软件数都数不过来，不过主要是苦于大部分app不是需要会员就是有广告。

- 所以我有个大胆的想法--Do It Yourself。

***设计思路：***

​	本地部署好服务器并通过IPv6连接网络作为云服务器，使用WebDAV作为同步策略，用户端的设备只需要配置好MySpace的设置，就可以在本地浏览、修改文件，因为WebDAV会自动同步已上传的文件，所以只要在不同设备上部署好MySpace，就可以在不同设备之间无缝衔接，而且MySpace使用flutter架构故可以实现跨平台。

​	对于文件，我的需求只有文本、图片，所以图片全部以URL的形式储存在文本中，本体存在云服务器中，客户端使用的时候再在设备端进行渲染。文本既保存在本地又保存在云服务器。

***初步功能设计：***

| 希望的功能 | 目标                 |
| ---------- | -------------------- |
| 主页       | 将近期更新的动态显示 |
| 博客       | 自己玩               |
| 知识库     | 语雀样式             |
| 照片墙     | 小米云相册样式       |
| 生活空间   | 微博样式             |
| 书影墙     | Notion样式           |

多个愿望一次满足！但是要达到这个设计目标，难度那也不小。

我想做的不仅是一个展示的聚合网页，同时也是一个编辑平台、是一个笔记软件，一个可以没有广告、没有推送、全部定制化的完全属于我自己的软件-MySpace。
