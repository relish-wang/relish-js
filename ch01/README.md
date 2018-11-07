# 第一章 JavaScript简介
---------------------

JS诞生初期(1995), 是用于处理输入验证的。那时候拨号上网带宽有限, 输入验证交若给服务端处理是极其挑战人的耐性的。

## 1.1 JavaScrip简史

LiveScript(1995.2)
    |
JavaScript(为了搭Java的热度而更名)
    |
JScript(IE)(1996.8)微软, 此命名是为了避开授权问题
    |
ECMAScript(1997,欧洲计算机制造商协会制定)
    |
标准(ISO/IEC-16262)(1998, 国际标准化组织和国际电工委员会采用此标准)

## 1.2 JavaScript实现

############################
#          JavaScrip       #
# ____________ _____ _____ #
# |ECMAScript| |DOM| |BOM| #
# ￣￣￣￣￣￣￣ ￣￣￣ ￣￣￣ #
############################

- 核心(ECMAScript)
- 文档对象模型(DOM)
- 浏览器对象模型(BOM)

### 1.2.1 ECMAScript

Web浏览器只是ECMAScript实现的**宿主环境**之一。(Node是一种服务端JavaScript平台)

ECMAScript的组成部分: **语法**、**类型**、**语句**、**关键字**、**保留字**、**操作符**、**对象**。

本书写作背景: ECMA-262第5版(2009年)
- 第1版: **与JavaScript1.1大致相同**, 仅删除了针对浏览器的代码和一些小改动。
- 第2版: **编辑加工**。（一般不适用第2版来衡量ECMAScript实现的兼容性）
- 第3版: 第一次真正的修改。标志着ECMAScript成为了一门**真正的编程语言**。(正则、新控制语句、try-catch)
- 第4版: **全面检核修订**。(强类型变量、新语句、真正的类、经典继承、数据交互新方式)

## 1.2.2 文档对象模型(DOM)

注: DOM并不只是针对JavaScript, 其他语言也实现了DOM。

Document Object Model

DOM把整个页面映射为一个多层节点结构。开发人员可以轻松自如地删除、添加、替换或修改任何节点。

- 1.为什么使用DOM

负责制定Web通信标准的W3C(World Wide Web Consortium, 万维网联盟)开始着手规划DOM。

html
|- head
|   |- title
|       |- Sample Page
|- body
    |- p
        |- Hello World!

- 2.DOM级别

DOM1级(DOM Level 1)于1998年10月成为W3C的推荐标准。

DOM1级(DOM Level 1):
- DOM核心(DOM Core)
- DOM HTML

DOM2级(DOM Level 2):
- DOM视图(DOM Views): 定义了跟踪不同文档视图的接口。
- DOM时间(DOM Events): 定义了事件和事件处理的接口。
- DOM样式(DOM Styles): 定义了基于CSS为元素应用样式的接口。
- DOM遍历和范围(DOM Traversal and Range): 定义了遍历和操作文档树的接口。

DOM3级(DOM Level 3):
- DOM加载和保存(DOM Load and Save): 引入以统一方式加载和保存文档的方法。
- DOM验证(DOM Validation): 验证文档的方法。
- DOM核心开始支持XML 1.0规范。

## 1.2.3 浏览器对象模型(BOM)
