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

您可以将通过如下**两种方式**将您的数据添加到地图并自行管理🚀

### 1. 提交 pull request

__这是最好的选择：__ Fork repo，添加或更新您的数据并发送pull request。 完成合并后，它将在地图上显示！ 💯

👉 你知道你不需要使用 Git 来添加你的条目吗？ GitHub在其网站上提供了所有工具，您可以立即开始使用它们 ，请参阅[操作方法：通过GitHub网站添加您的数据（Powerd by REDAXO）](https://github.com/HainanU-Application/HainanU-Alumni-Map/blob/main/_directory/howto-add-entry-via-github.md)。

### 2. 联系我们

❤️如果您根本没有 GitHub 帐户，请将您的数据发送给我们（请务必按照如下格式），__Email:__ eilo.pengyq@gmail.com

#### 数据格式

该地图需要您的姓名或昵称以及您的地理位置，其他一切都是可选的。 当然，我们都想了解更多关于您的信息，也许还会看到您的照片！ 但是否提供完全取决于您！

创建以您名字命名的文件夹（拼音或英文），并包含`data.yml`文件以及您的照片和头像，**目录树示例如下**。

![image-20220614234424552](https://cdn.jsdelivr.net/gh/peng-yq/Gallery/img/202206150036986.png)

其中**`data.yml`模板如下**，**您只需要修改成您的数据即可**。

```yaml
---
# 名称（必填）
# 可能是您的真实姓名或昵称
name: Home

# 地理位置（必填）
# 按位数提供您喜欢的详细程度（如 50.107811 或 50.11）
# 您可以使用诸如 openstreetmap.org 之类的服务来查找您的地理位置
latitude: 20.059876651066645
longitude: 110.3395963223301


# 描述你自己、例如去向或者工作单位以为校友提供帮助
# 若无博客地址，请在此处写明您的邮箱使得校友可以联系到您
# 最多应为 300 个字符。 没有标记或换行符！
bio: "Hainan University"

# 图片或头像
# 提供当前文件夹中的图像文件h
# 应该是正方形的，大小约为 200-300 像素！
image: HainanU.png

# 链接
# 一个或多个指向您的网站、您的 github 个人资料、twitter、facebook 等的链接。
# 最多4个链接
links:
- https://ha.hainanu.edu.cn/
- http://en.hainanu.edu.cn/
---
```

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
