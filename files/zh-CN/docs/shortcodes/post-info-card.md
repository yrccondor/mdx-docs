# 文章信息卡

MDx 提供了多种短代码的支持，在文章中插入短代码即可调用相关功能。「文章信息卡」是其中的一种。

## 基本用法

```
[mdx_post]URL 内容[/mdx_post]
```

## URL 内容

同一域名下使用 MDx 主题或 [Open Graph](https://ogp.me) 信息完整的页面的 URL。

## 例子

```
[mdx_post]https://samedomain.com/mdx.html[/mdx_post]
```

!!! tip "技巧"
    URL 必须完整（包含协议、主机名、路径等）且必须位于同一域名下。受 MDx 控制的页面可以被正常预览，同一域名下的其他页面在 [Open Graph](https://ogp.me) 信息完整的情况下也可以被预览。

!!! bug "加载失败"
    如果预览信息加载失败，在信息卡的原本位置将会显示错误信息，并提供一个指向目标页面的链接。

## 预览

![Preview](.../img/post-info.jpg)
