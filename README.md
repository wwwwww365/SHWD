# SHWD-YOLO

[SHWD（Safety Helmet Wearing Dataset）](https://github.com/njvisionpower/Safety-Helmet-Wearing-Dataset)
安全帽佩戴检测数据集的 YOLO 格式打包文件。

## 下载

数据集以 **Release 附件** 的形式发布（单个 1.06 GiB 文件，仓库本身只保留本说明）：

**https://github.com/wwwwww365/SHWD/releases/latest**

| 项目 | 值 |
| --- | --- |
| 文件名 | `SHWD-YOLO.zip` |
| 大小 | 1,141,576,107 字节（约 1.06 GiB） |
| SHA256 | `e0709d10a286e8a9dcc2fb3c278ff2578c1c523014810c04b899c91995d3832a` |

## 校验

Windows：

```bat
certutil -hashfile SHWD-YOLO.zip SHA256
```

Linux / macOS：

```bash
sha256sum SHWD-YOLO.zip   # macOS: shasum -a 256 SHWD-YOLO.zip
```

## 说明

- 单个文件超过 GitHub 单仓库 100 MB 的文件大小限制，因此不使用普通的 git 提交，
  而是作为 Release 附件发布（附件上限 2 GB，支持 `git clone` 之外的直接下载）。
- 解压后目录结构为 `images/`（`test/`、`train/` 等）与标注文件，共 15,172 个条目。
- 使用 GitHub CLI 下载：`gh release download v1.0 -R wwwwww365/SHWD`。
