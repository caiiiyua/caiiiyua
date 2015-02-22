+++
categories = ["Development", "Go"]
date = "2015-02-20T00:34:06+08:00"
tags = ["golang", "Development"]
title = "Go by Example - Hello World"
+++

我们的第一个Go程序将打印出经典的“hello world”，下面是完整的代码：
```
package main

import "fmt"

func main() {
        fmt.Println("Hello, World")
}
```
<!--more-->
我们将代码保存在hello-world.go中，可以通过go run来直接运行：

    go run hello-world.go

或者我们可以先将它编译成二进制的可执行程序：

    go build hello-world.go

接着可以直接运行它：

```
   $ ./hello-world
   Hello, World
```

现在我们可以编译和运行基本的Go程序了，下面让我们了解更多Go的知识咯.

下节例子: [值] [1]

[1]:
