# 模板配置
---

[TOC]

## 模板的语法

当前模板使用的是Velocity的语法结构，我将简单介绍一些常见写法，完全文档可以参考[Velocity官方文档](https://velocity.apache.org/engine/devel/user-guide.html)。

### 变量

使用$取出在VelocityContext容器中存放的值。
```
$!{tablePrefix}
$!{tableNameEN}

#foreach(${column} in ${columns})
    $!{column.columnNameCH}
#end
```
需要注意，上面代码中 $!{}的写法，使用$var获取变量时，如果变量不存在，Velocity引擎会将其原样输出，通过使用$!{}的形式可以将不存在的变量变成空白输出。
### 条件控制

在Velocity中可以使用条件语法对流程进行控制
```
#if($!{column.javaType}  == "Date")
    ...
#elseif($!{column.javaType}=="String" and $!{column.likeFlag} == true)
    ...
#else
```
### 循环

在Velocity中可以使用循环语法遍历集合，语法结构如下：

```
#foreach($item in $list)
 $item
 $velocityCount 
#end
```
其中，$item代表遍历的每一项，velocityCount是Velocity提供的用来记录当前循环次数的计数器，默认从1开始计数。

## 模板可用参数

| 参数 | 类型 | 注释 |
| ------ | ------ | ------ |
| tablePrefix | `java.lang.String` | 表名前缀（带下划线），如果不去掉前缀则为空 |
| htmlPath | `java.lang.String` | 前台页面路径 |
| htmlFileName | `java.lang.String` | 前台页面名称 |
| packagePath | `java.lang.String` | 包路径 |
| tableNameCH | `java.lang.String` | 中文表名 |
| tableNameEN | `java.lang.String` | 英文表名 |
| tableNameENUpperCase | `java.lang.String` | 英文表名（大写） |
| tablePrefixLowerCase | `java.lang.String` | 表名前缀（小写） |
| tablePrefixUpperCase | `java.lang.String` | 表名前缀（大写） |
| tableClassNameEN | `java.lang.String` |  |
| tablePropertyNameEN | `java.lang.String` |  |
| author | `java.lang.String` | 创建者 |
| dateTime | `java.lang.String` | 创建日期 |
| pkColumn | `Column` | 主键字段 |
| extFlagColumns | `java.util.List<Column>` | 扩展标识字段 |
| effectiveFlagColumn | `Column` | 逻辑删除标识字段 |
| columns | `java.util.List<Column>` | 普通字段 |

## 自定义类型

你会注意到，在模板可用参数中，除了Java基本类型外，存在一个`Column`类型，这是一个自定义类体类，它的详细字段如下：

### Column类型解析

| 名称 | 类型 | 注释 |
| ------ | ------ | ------ |
| columnNameCH | `java.lang.String` | 字段中文名称 |
| columnNameEN | `java.lang.String` | 字段英文名称 |
| columnPropertyName | `java.lang.String` | 字段属性名称 |
| columnMethodName | `java.lang.String` | 字段方法名称 |
| jdbcType | `java.lang.String` | Jdbc数据类型 |
| javaType | `java.lang.String` | Java数据类型 |
| autoFill | `java.lang.String` | 自动填充 |
| likeFlag | `java.lang.String` | 模糊标识 |
| isNullable | `java.lang.Boolean` | 是否可以为空 |
| maxLength | `java.lang.String` | 字段长度 |