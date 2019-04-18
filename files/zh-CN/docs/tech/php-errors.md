# 常见 PHP 错误

在使用 MDx 时，你可能会发现一些预料之外的 PHP 错误。不要紧张，这很可能不是 MDx 的问题。 查阅下面的内容将有助于解决问题。

## 未定义函数 mb\_strimwidth\(\)

MDx 使用了此函数来截断字符串以生成摘要。此问题出现于 `php.ini` 中未启用此函数的情况下，尤其是自行安装的 PHP。

要解决此问题，你可以在 `php.ini` 中启用此函数。以 PHP 7.2.0 为例，找到：

```
;extension=mbstring
```

去除第一个分号即可。即：

```
extension=mbstring
```

其他版本的 PHP 启用方法可能稍有不同。

## 在后台出现 file\_get\_contents\(\) 警告

此错误发生于 MDx 试图从 CDN 获取最新版本信息时。由于你的 `php.ini` 限制， MDx 无法从启用了 https 的 CDN 中获取版本信息。你可以通过修改 `php.ini` 启用 OpenSSL 来解决此问题。以 PHP 7.2.0 为例，找到：

```
;extension=openssl
```

去除第一个分号即可。即：

```
extension=openssl
```

其他版本的 PHP 启用方法可能稍有不同。

!!! info "安装 OpenSSL"
    在 Linux 中你可能需要先安装 OpenSSL （很可能已经安装）。

## PHP Warning

你可能会在一些地方发现 PHP Warning。请不要担心，这很可能是由于你开启了 [WordPress Debug 模式](https://codex.wordpress.org/WP_DEBUG)（默认关闭）导致的，并不影响使用。

要关闭 WordPress Debug 模式，你需要修改 WordPress 安装根目录下的 `wp-config.php` 文件。找到：

``` php
define( 'WP_DEBUG', true );
```

将 `true` 改为 `false` 即可。即：

``` php
define( 'WP_DEBUG', false );
```
