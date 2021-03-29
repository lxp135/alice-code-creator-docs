# 软件结构介绍
---

[TOC]

```
|---java
|   |---alice
|       |---code
|           |---creator
|               |---common
|               |   |---dao
|               |   |---framework
|               |   |   |---config
|               |   |   |---context
|               |   |   |---handler
|               |   |   |---interceptor
|               |   |   |---listener
|               |   |   |---security
|               |   |---service
|               |   |---util
|               |---controller
|               |   |---base
|               |   |---generator
|               |   |---monitor
|               |---dao
|               |   |---base
|               |   |   |---impl
|               |   |---generator
|               |       |---impl
|               |---domain
|               |   |---constant
|               |   |---enums
|               |   |---model
|               |       |---base
|               |       |---generator
|               |---service
|                   |---base
|                   |   |---impl
|                   |---generator
|                       |---impl
|---resources
    |---log
    |---mybatis
    |   |---mysql
    |       |---base
    |       |---generator
    |---public
    |   |---assets
    |   |   |---css
    |   |   |---font
    |   |   |---img
    |   |   |---js
    |   |   |---lib
    |   |       |---bootstrap
    |   |       |---datetimepicker
    |   |       |---director
    |   |       |---echarts
    |   |       |---jqGrid
    |   |       |---jquery
    |   |       |---jquery-ui
    |   |       |---jquery.codemirror
    |   |       |---jquery.niftymodals
    |   |       |---jTemplates
    |   |       |---layer
    |   |       |---material-design-icons
    |   |       |---niceValidator
    |   |       |---perfect-scrollbar
    |   |       |---roboto
    |   |       |---select2
    |   |       |---webUploader
    |   |       |---zTree
    |   |---biz
    |   |   |---basic
    |   |   |   |---base
    |   |   |       |---dictionary
    |   |   |       |   |---area
    |   |   |       |   |---country
    |   |   |       |---menu
    |   |   |       |---role
    |   |   |       |---user
    |   |   |---generator
    |   |       |---config
    |   |       |   |---datasource
    |   |       |   |---group
    |   |       |   |   |---template
    |   |       |   |---individual
    |   |       |---mapping
    |   |---framework
    |---sql
```