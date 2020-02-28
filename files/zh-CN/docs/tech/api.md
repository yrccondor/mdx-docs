# API

为了更方便地实现某些高级功能，MDx 在开发过程中预留了部分 API。这些 API 是为程序调用预留的，并不直接向主题用户公开。这个页面将列出 MDx 中所有预留的 API 及调用方法。

## 最近评论

如果一位访客刚刚发表了评论，它将会带有名为 `mdx_recently_commented`，值为 `true` 的 Cookie 以便辨识。该 Cookie 有效期为 15 分钟。

这一 API 无需调用即可生效。

## 离线模式

当你的站点启用了 Service Worker 时，其可以被离线访问。但由于离线，此时站点的搜索和评论功能都不可用。MDx 提供离线模式，在被激活时可以优雅地禁用站点的搜索和评论功能并显示一条提示。

离线模式必须被手动激活。在位于页面末尾的 `js.js`, `post.js` 或 `page.js` 被载入前将名为 `offlineMode` 的 Javascript 变量设置为 `true` 即可激活离线模式。

```JavaScript
var offlineMode = true;
```

## 禁用 Cookie 使用提示

如果你启用了 Cookie 使用提示功能，你可能会希望对非欧盟地区的访客禁用该提示。MDx 提供了禁用 API，**但仅提供直接禁用的方法，具体判断逻辑还需另外编写。**

要禁用 Cookie 提示，你需要在位于页面末尾的 `js.js`, `post.js` 或 `page.js` 被载入前将名为 `displayCookie` 的 Javascript 变量设置为 `false`。

```JavaScript
var displayCookie = false;
```
