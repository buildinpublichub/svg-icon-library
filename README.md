# SVG Icon Library

> **Copyright notice** — All icons in this repository are copyright of
> [koboyo.com/icons](https://koboyo.com/icons). This repository grants **no rights**
> to them and therefore contains no LICENSE file. Read [NOTICE](NOTICE) and comply
> with koboyo.com's official terms before using them.
>
> **版权提示** —— 本仓库所有图标版权归 [koboyo.com/icons](https://koboyo.com/icons) 所有。
> 本仓库**不授予任何权利**，因此不含 LICENSE 文件。使用前请先阅读 [NOTICE](NOTICE)
> 并遵守 koboyo.com 的官方授权条款。

A collection of 133,464 SVG icons organised by theme, with a full CSV index.

一套按主题分类的 SVG 图标集合，共 133,464 个文件，附完整 CSV 索引。

## Directory structure / 目录结构

| Directory 目录 | Contents 内容 | Count 数量 |
|---|---|---:|
| `face/` | Faces and expressions — 人脸／表情 | 1,305 |
| `mark/` | Marks, symbols and textures — 标记、符号、纹理 | 11,830 |
| `object/` | Objects, tools and artefacts — 物件、工具、器物 | 78,858 |
| `people/` | People, activities and events — 人物、活动、事件 | 39,448 |
| `scene/` | Scenes — `uistate` UI states, `vignette` vignettes<br>场景类（`uistate` 界面状态、`vignette` 情景小图） | 2,023 |

## Index file / 索引文件

`_index.csv` is the complete index. Its columns are:

`_index.csv` 是完整索引，字段如下：

```
slug,category,subgroup,title,keywords,file
```

| Column 字段 | Meaning 含义 |
|---|---|
| `slug` | Unique identifier — 图标唯一标识 |
| `category` / `subgroup` | Category and subcategory — 所属分类与子分类 |
| `title` | Human-readable title — 图标标题 |
| `keywords` | Space-separated search terms — 检索关键词（空格分隔） |
| `file` | Relative path, e.g. `object/tool/3d-printer.svg`<br>相对路径，如 `object/tool/3d-printer.svg` |

## Usage / 用法

Search the index by keyword to locate a file:

按关键词检索索引即可定位文件：

```bash
grep -i "printer" _index.csv
```

Clone the repository:

克隆仓库：

```bash
git clone https://github.com/buildinpublichub/svg-icon-library.git
```

The repository is around 895 MB. To fetch the index and file listing without
downloading every icon up front, use a blobless clone:

仓库约 895 MB。若只想拿索引和文件清单、不预先下载全部图标，可用 blobless clone：

```bash
git clone --filter=blob:none https://github.com/buildinpublichub/svg-icon-library.git
```

The icons are plain SVG with `fill="currentColor"`, so they inherit the surrounding
text colour when inlined.

图标为纯 SVG 且使用 `fill="currentColor"`，内联时会自动继承外层文字颜色。

## Copyright / 版权

Icons are copyright of [koboyo.com/icons](https://koboyo.com/icons). See [NOTICE](NOTICE)
for details.

图标版权归 [koboyo.com/icons](https://koboyo.com/icons) 所有，详见 [NOTICE](NOTICE)。
