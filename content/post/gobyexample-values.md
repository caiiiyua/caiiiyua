+++
categories = ["Development", "Go", "瞎想"]
date = "2015-02-20T00:59:19+08:00"
tags = ["golang", "Development", "瞎想"]
title = "Go by Example － 值"

+++

Go语言中的值有各种类型，如strings，intergers，floats，booleans等，下面是一些简单的例子：
```
package main

import "fmt"

func main() {
    fmt.Println("go" + "lang")
    fmt.Println("1+1=", 1+1)
    fmt.Println("7.0/3.0=", 7.0/3.0)
    fmt.Println(true && false)
    fmt.Println(true || false)
    fmt.Println(!true)
}
```
<!--more-->
Strings 可以通过＋来拼接。
Intergers，floats，booleans等都和我们之前所学的语言类似。
```
$ go run values.go 
golang
1+1= 2
7.0/3.0= 2.3333333333333335
false
true
false
```

下节例子： [变量] [1]

[1]: 
