# 框架和库

## MDUI

MDx 内置了 [MDUI](https://mdui.org) 框架的 0.4.2 版本。此框架位于 `主题根目录/mdui/` 下。

如果你希望借此进行其他开发，请注意：

- 内置版本中的 CSS 文件已被改动过（修改了一处样式），请从 MDUI 官方下载 MDUI 框架并自行替换
- 内置版本中的 `fonts` 文件夹已被移除，如果需要请自行从 MDUI 官方下载并添加

!!! info "更新 MDUI"
    MDx 会尽可能跟随 MDUI 更新内置的 MDUI 版本。

## jQuery

MDx 内置了 jQuery 3.2.1 版本。此文件位于 `主题根目录/js/` 下。

!!! info "移除 jQuery"
    MDx 计划在未来版本中移除对 jQuery 的依赖，但 jQuery 文件暂时不会被移除以应对可能的第三方需求。

## html2canvas

MDx 内置了 [html2canvas](https://html2canvas.hertzen.com) 1.0.0-alpha.11 版本。此文件位于 `主题根目录/js/` 下。

!!! info "更新 html2canvas"
    MDx 会尽可能跟随 html2canvas 更新内置的 html2canvas 版本。

## lazyload

MDx 内置了 [lazyload](https://github.com/jieyou/lazyload)。此文件位于 `主题根目录/js/` 下。

!!! info "更新 LazyLoad"
    MDx 计划在未来版本中使用另一 LazyLoad 库代替这个库以提供更好的性能和加载样式。

## Theme Update Checker Library

MDx 内置了 [Theme Update Checker Library](https://w-shadow.com/blog/2011/06/02/automatic-updates-for-commercial-themes/) 1.2 版本。此文件位于主题根目录下。

!!! info "替换 Theme Update Checker Library"
    MDx 计划在未来版本中使用 [Plugin Update Checker](https://github.com/YahnisElsts/plugin-update-checker/) 来替换这一老旧库。
