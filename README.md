# Alice CodeCreator 中文参考文档
Alice CodeCreator 是一个通用代码生成辅助工具，支持生成包括不限于html、js、java、xml、sql等各种类型代码。

## 如何使用
* 直接访问 https://creator.liuxp.me
* 使用mkdocs本地编译md文件，生成HTML静态页面。

## 如何编辑文档
使用markdown书写并用mkdocs编译。

需要Python和Python package manager pip 来安装MkDocs
使用pip安装mkdocs:
```
$ pip install mkdocs
```
运行 mkdocs -V 以检查是否正确安装
```
$ mkdocs -V
```
进入项目文件夹，执行以下命令编译
```
mkdocs build --clean
```
会基于mkdocs.yml配置将docs中的原始md文件编译到site文件夹中形成静态页面。