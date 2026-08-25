# SVG Icon Library

**English** · [简体中文](README.zh-CN.md)

> **Copyright notice** — All icons in this repository are copyright of
> [koboyo.com/icons](https://koboyo.com/icons). This repository grants **no rights**
> to them and therefore contains no LICENSE file. Read [NOTICE](NOTICE) and comply
> with koboyo.com's official terms before using them.

A collection of 133,464 SVG icons organised by theme, with a full CSV index.

## Directory structure

| Directory | Contents | Count |
|---|---|---:|
| `face/` | Faces and expressions | 1,305 |
| `mark/` | Marks, symbols and textures | 11,830 |
| `object/` | Objects, tools and artefacts | 78,858 |
| `people/` | People, activities and events | 39,448 |
| `scene/` | Scenes — `uistate` UI states, `vignette` vignettes | 2,023 |

## Index file

`_index.csv` is the complete index. Its columns are:

```
slug,category,subgroup,title,keywords,file
```

| Column | Meaning |
|---|---|
| `slug` | Unique identifier |
| `category` / `subgroup` | Category and subcategory |
| `title` | Human-readable title |
| `keywords` | Space-separated search terms |
| `file` | Relative path, e.g. `object/tool/3d-printer.svg` |

## Usage

Search the index by keyword to locate a file:

```bash
grep -i "printer" _index.csv
```

Clone the repository:

```bash
git clone https://github.com/buildinpublichub/svg-icon-library.git
```

The repository is around 895 MB. To fetch the index and file listing without
downloading every icon up front, use a blobless clone:

```bash
git clone --filter=blob:none https://github.com/buildinpublichub/svg-icon-library.git
```

The icons are plain SVG with `fill="currentColor"`, so they inherit the surrounding
text colour when inlined.

## Copyright

Icons are copyright of [koboyo.com/icons](https://koboyo.com/icons).
See [NOTICE](NOTICE) for details.
