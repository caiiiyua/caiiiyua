+++
categories = ["Development", "Go", "瞎想"]
date = "2015-02-20T01:17:55+08:00"
tags = ["golang", "Development", "瞎想"]
title = "Go by Example - 变量"

+++

在Go中，变量需要显示声明给编译器，因此并非解释性语言，而是如C/C++一样属于强类型语言。

如下面的例子：
```
package main

import "fmt"

func main() {
	var a = "literal"
	fmt.Println(a)

	var b, c = 1, 2
	fmt.Println(b, c)

	var d = true
	fmt.Println(d)

	var e int
	fmt.Println(e)

	f := "short"
	fmt.Println(f)
}
```
<!--more-->
通过var显示的声明变量如：

    var a ＝ "literal"

也可以同时定义多个变量，Go会根据变量的初始值为变量定义类型。

    var b, c = 1, 2

未初始化的变量会被初始化为0值，例如int型的0值是0.

    var e int

也可以通过:=这个简化版本来声明和初始化变量

    f := "short"

输出如下：
```
$ go run variables.go
literal
1 2
true
0
short
```

下节例子： [常量] [1]

[1]:
