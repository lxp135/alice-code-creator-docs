# 编写文档

[TOC]

## 如何使用

* 直接访问 https://creator.liuxp.me
* 使用MkDocs本地编译md文件，生成HTML静态页面。
  
## 如何编辑文档
使用markdown书写并用MkDocs编译。
  
需要Python和Python package manager pip 来安装MkDocs
使用pip安装MkDocs:
```
$ pip install mkdocs
```
运行 `mkdocs -V` 以检查是否正确安装
```
$ mkdocs -V
```
进入项目文件夹，执行以下命令编译
```
mkdocs build --clean
```
会基于`mkdocs.yml`配置将`docs`路径中的原始md文件编译到`site`路径中形成静态页面。

## 注意事项

* **[必须]** 页面标题和章节标题使用 `#` 、 `##` 和 `###` 。 **不要**使用 `=======` 或者 `-------`。
* **[必须]** 使用 `[TOC]` 添加一个目录。

## 其他

查阅[MkDocs官网](https://www.mkdocs.org/)获取更多信息。