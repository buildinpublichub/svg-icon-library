# SVG 图标库

[English](README.md) · **简体中文**

> **版权提示** —— 本仓库所有图标版权归 [koboyo.com/icons](https://koboyo.com/icons) 所有。
> 本仓库**不授予任何权利**，因此不含 LICENSE 文件。使用前请先阅读 [NOTICE](NOTICE)
> 并遵守 koboyo.com 的官方授权条款。

一套按主题分类的 SVG 图标集合，共 133,464 个文件，附完整 CSV 索引。

## 目录结构

| 目录 | 内容 | 数量 |
|---|---|---:|
| `face/` | 人脸／表情 | 1,305 |
| `mark/` | 标记、符号、纹理 | 11,830 |
| `object/` | 物件、工具、器物 | 78,858 |
| `people/` | 人物、活动、事件 | 39,448 |
| `scene/` | 场景类 —— `uistate` 界面状态、`vignette` 情景小图 | 2,023 |

## 索引文件

`_index.csv` 是完整索引，字段如下：

```
slug,category,subgroup,title,keywords,file
```

| 字段 | 含义 |
|---|---|
| `slug` | 图标唯一标识 |
| `category` / `subgroup` | 所属分类与子分类 |
| `title` | 图标标题 |
| `keywords` | 检索关键词（空格分隔） |
| `file` | 相对路径，如 `object/tool/3d-printer.svg` |

## 用法

按关键词检索索引即可定位文件：

```bash
grep -i "printer" _index.csv
```

克隆仓库：

```bash
git clone https://github.com/buildinpublichub/svg-icon-library.git
```

仓库约 895 MB。若只想拿索引和文件清单、不预先下载全部图标，可用 blobless clone：

```bash
git clone --filter=blob:none https://github.com/buildinpublichub/svg-icon-library.git
```

图标为纯 SVG 且使用 `fill="currentColor"`，内联时会自动继承外层文字颜色。

## 版权

图标版权归 [koboyo.com/icons](https://koboyo.com/icons) 所有，详见 [NOTICE](NOTICE)。
