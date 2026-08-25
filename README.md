# SVG Icon Library

一套按主题分类的 SVG 图标集合，共 13 万余个文件。

## 目录结构

| 目录 | 内容 |
|------|------|
| `face/` | 人脸／表情图标 |
| `mark/` | 标记、符号类图标 |
| `object/` | 物件、工具、器物类图标 |
| `people/` | 人物、活动、场景中的人 |
| `scene/` | 场景类图标（`uistate` 界面状态、`vignette` 情景小图） |

## 索引文件

`_index.csv` 是完整索引，字段如下：

```
slug,category,subgroup,title,keywords,file
```

- `slug` — 图标唯一标识
- `category` / `subgroup` — 所属分类与子分类
- `title` — 图标标题
- `keywords` — 检索关键词（空格分隔）
- `file` — 相对路径，如 `object/tool/3d-printer.svg`

## 用法

按关键词检索索引即可定位文件：

```bash
grep -i "printer" _index.csv
```

克隆仓库：

```bash
git clone https://github.com/buildinpublichub/svg-icon-library.git
```
