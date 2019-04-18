# 常见问题

## 主题下载

> 我能从哪里下载 MDx？

MDx 提供 2 个官方发布渠道，从这 2 个发布渠道下载的 MDx 会是最新的：

- [MDx 网站](https://mdx.flyhigher.top)
- [Github Releases](https://github.com/yrccondor/mdx/releases/)

从其他渠道下载的 MDx 不一定是最新的，**请尽量不要使用。**

> 我可以通过直接 Clone 仓库的方式来下载吗？

尽量不要。

每当新版本发布时，MDx 的构建系统会自动拉取最新的主题文件并在进行一些修改（压缩 CSS、写入版本信息、去除不必要的文件等）后进行打包发布。如果你直接 `clone` 主题仓库，**可能会遇到 MDx 设置数据被清空、更新版本不正确等问题，请尽可能不要这么做。**

当然，我们并非不你允许 `clone` 主题仓库，**只是不建议通过这种方式下载主题。**

> 如何确保我下载的主题没有被第三方修改？

[MDx 网站](https://mdx.flyhigher.top) 提供了最新版本安装包的哈希值，你可以通过对比哈希值来确保你的安装包是最新且没有被第三方修改过的。

## 主题使用

> 安装主题后网站无法正常显示怎么办？

MDx 在主流环境配置中经过测试，**如果遇到问题请先检查你的环境配置，并确认是否是 MDx 造成的问题。** 如果的确是 MDx 引起的问题且无法解决，请向我们反馈。

> 使用中遇到问题，我该去哪里反馈？

你可以通过以下 2 个渠道向我们反馈问题、提出疑惑：

- [Github issues](https://github.com/yrccondor/mdx/issues)
- QQ 群：687577787

## 主题开发

> 我可以二次开发 MDx 吗？

当然可以。MDx 使用 GPL V3.0 协议发布，你可以 **随意且免费地修改主题**，但请遵守 GPL V3.0 协议。

作为附加条款，**你不能修改或移除主题页面底部的 "Theme: MDx By AxtonYao" 字样**，否则请不要使用 MDx。

如果你觉得自己所做的修改对其他用户也非常有帮助，欢迎向我们提交 Pull Request，详见 [帮助我们](help-us.md)。

> 更新后我对主题的修改丢失了怎么办？

这是 WordPress 的更新原理导致的。主题更新过程中 WordPress 会使用新版本的主题文件覆盖旧版本的主题文件，因此会覆盖你的修改。

要保持你的修改，请考虑使用 [子主题](https://codex.wordpress.org/zh-cn:子主题)。

## 其他问题

> 如何正确地提问？

请参阅 [提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/master/README-zh_CN.md)。

> MDx 不好用、很垃圾怎么办？

哦。
