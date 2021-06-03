# Alice CodeCreator 中文参考文档
---

> [Alice CodeCreator](http://creator.liuxp.me) 是一个通用代码生成辅助工具，支持生成包括不限于html、js、java、xml、sql等各种类型代码。

## 项目特性

* 采用Velocity模板引擎构建并生成代码。
* 数据模型使用JDBC实现，提供数据类型映射配置页面。
* 支持模板分组，可以区分不同使用场景定义不同的分组。
* 灵活的全局级、分组级和模板级参数配置，适应多种场景。
* 支持网页版本的模板编辑器，可以代码高亮。
* 支持不同数据库，最新版本支持`MySQL`、`Oracle`和`SQLServer`。
* 支持多数据源配置，可以通过页面动态接入数据源地址。
* 可以项目组级别部署，支持用户自主注册。
* 数据权限隔离，用户和用户之间的数据源配置和模板分组互不可见。
* 详细的项目文档，手把手级别。

**该文档包含三个主要组成部分**：

* **用户手册** - 当您仅使用Alice CodeCreator生成代码时参考该部分文档
* **开发者手册** - 当您想扩展Alice CodeCreator功能时可以参考该部分文档
* **参考资料** - 一些相关的文档与资料

## 文档目录

* [首页](index.md)
* [更新日志](released.md)
* 用户手册
    - [快速开始](users/getting-started.md)
    - [数据类型配置](users/data-type.md)
    - [数据源配置](users/data-source.md)
    - [模板配置](users/template.md)
    - [生成代码](users/generator.md)
* 开发者手册
    - [开发计划](developers/plan.md)
    - [构建与运行](developers/building.md)
    - [软件结构介绍](developers/framework.md)
    - [贡献代码](developers/writing-code.md)
    - [编写文档](developers/writing-documents.md)
    - [贡献者列表](developers/contributors-of-documents.md)
* 参考资料
    - [FAQ](references/FAQ.md)
    
## 仓库地址

* 该项目的文档在[https://github.com/lxp135/alice-code-creator-docs](https://github.com/lxp135/alice-code-creator-docs)中，欢迎Star。
* 该项目的源码在[https://github.com/lxp135/alice-code-creator](https://github.com/lxp135/alice-code-creator)中，欢迎Star。