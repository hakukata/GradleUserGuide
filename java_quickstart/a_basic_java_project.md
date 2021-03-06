# 一个基础的 Java 项目 {#revision1}

让我们先来看一个简单的例子.

我们可以加入下面的代码来使用 Java 插件:

**例子 7.1. 使用 Java 插件**

_build.gradle_

```
apply plugin: 'java'
```

（注：此例子的代码可以再所有“-all”结尾的发行版的samples/java/quickstart目录下找到）

它将会把 Java 插件加入到你的项目中,  这意味着许多预定制的任务会被自动加入到你的项目里.

Gradle 默认在 **src/main/java** 目录下寻找到你的正式（生产）源码, 在 **src/test/java** 目录下寻找到你的测试源码, 并在**src/main/resources**目录下寻找到你准备打包进jar的资源文件。测试代码会被加入到环境变量中设置的目录里运行。所有的输出文件都会被创建在构建目录里, 生成的JAR文件会被存放在 **build/libs** 目录下.

**都加了什么可以执行的任务呢?**

请在项目目录下使用 **gradle tasks** 来列出该项目的所有任务。

