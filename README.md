# HainanU Alumni Map | 海南大学校友地图

一张满是海南大学校友的地图，他们愿意为海南大学的学生提供帮助。 本地图托管在 [GitHub](https://github.com/HainanU-Application/HainanU-Alumni-Map)，欢迎校友添加地图条目，加入我们！

👉 __https://hainanu-application.github.io/HainanU-Alumni-Map/__

![image-20220614214207613](https://cdn.jsdelivr.net/gh/peng-yq/Gallery/img/202206142231559.png)

上面的屏幕截图显示了校友条目的外观。 您可以添加自己的头像、描述以及博客，这太棒了！ 看，这是[海南大学的链接](https://hainanu-application.github.io/HainanU-Alumni-Map/#home)。

## 致谢及开源证书

- 感谢REDAXO的[模板](https://github.com/FriendsOfREDAXO/community)
- 搭建过程中参考了[SUSTech-Alumni-Map](https://github.com/SUSTech-Application/SUSTech-Alumni-Map)

- Licensed under the [MIT](https://github.com/peng-yq/peng-yq.github.io/blob/main/LICENSE) 开源证书

## 如何添加和管理您的数据？

您可以将标记添加到地图并自行管理数据，**了解[管理您数据的三种方式](https://github.com/HainanU-Application/HainanU-Alumni-Map/tree/main/_directory)！** 🚀

## 地图的用途？

该地图适用于任何海南大学的学生（在读或已毕业的本科生、硕士生、博士生）或教职员工等。 这是海南大学校友分布的可视化，如果您是海南大学的一员，那么地图就是为您准备的！

## 这张地图是如何工作的？

GitHub 允许从存储库中生成静态网站，本地图使用 [Jekyll](https://jekyllrb.com)（一个基于 ruby 的生成器）， Jekyll 带有 [Liquid](https://shopify.github.io/liquid/) 模板，它帮助我们将所有地图条目注入到 HTML 底部的 JSON 中。 JavaScript 抓取数据并使用 [CARTO](https://carto.com/location-data-services/basemaps/) 提供的漂亮图块创建一个漂亮的 [Leaflet](http://leafletjs.com) 地图。

## 我该如何改进这个网站？

我们建议您将 repo 下载为 zip 文件，并首先使其在本地计算机上运行（请参阅 [SETUP.md](https://github.com/HainanU-Application/HainanU-Alumni-Map/blob/main/SETUP.md) 以获取说明)。

如果您遇到困难，我们很乐意提供帮助：eilo.pengyq@gmail.com。

## 如何在我的机器上运行地图？

有关说明，请参阅 [SETUP.md](https://github.com/HainanU-Application/HainanU-Alumni-Map/blob/main/SETUP.mdd)。

## TO DO

- 更换地图源为高德/百度以加快渲染速度
