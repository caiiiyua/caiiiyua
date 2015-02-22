+++
categories = ["Development", "Go"]
date = "2015-02-20T01:38:38+08:00"
tags = ["golang", "Development"]
title = "Go by Example - 常量"

+++

Go 支持的常量类型有字符型，string， boolean以及数字型。

在代码中通过关键字*const*来声明常量。
const表达式可以出现在任何可以通过var表达式声明变量的地方。
<!--more-->
如下面的例子：
```
package main

import (
	"fmt"
	"math"
)

const s string = "constant"

func main() {
	fmt.Println(s)

	const n = 500000000
	const d = 3e20 / n
	fmt.Println(d)

	fmt.Println(int64(d))
	fmt.Println(math.Sin(n))
}
```

输出如下：
```
$ go run constants.go
constant
6e+11
600000000000
-0.28470407323754404
```

下节例子： [for]

[for]:
