## Typecho 图片水印插件

本插件仅支持 png \ jpg 格式的图片作为水印。

推荐使用 png 格式的图片作为水印，以保证水印的质量。

## 使用方法

将 waterMark 目录上传至网站的 `usr/plugins` 目录，然后在后台启用即可。

保持目录结构如下：

```
waterMark/
├── imgfunc.php
├── Plugin.php
├── watermark.png
└── watermark2x.png
```

## 更新

**2018-9-21**
- 取消了对 typecho 版本的要求
- 增加了 2x 水印的支持
- 支持小图片不加水印

**2026-5-31**
- 兼容 PHP 8.0+
- 修复 `ImgWaterMark()` 函数参数顺序：将必选参数 `$w_pct`、`$w_quality` 移至可选参数之前
- 解决 PHP 8.0+ 报 `Deprecated: Optional parameter declared before required parameter` 警告的问题
- 修复因该警告导致 Typecho 上传图片后 JSON 响应被污染、前端提示"上传失败"的 bug


原作者：https://github.com/internelp/waterMark

Update by RONGYAN:https://github.com/aiyaya2004/waterMark-fro-php8
