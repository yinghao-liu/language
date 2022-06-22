# 005 循环



## for

通过一个简单的功能：查找某个string是否在数组中，分析for循环语法优化。
```go

var items = []string{"a", "b", "c"}

// is "d" in items?
var isdin = false
for _, j := range items {
	if "d" == j {
		isdin = true
		fmt.Printf("d is in items")
	}
}
if !isdin {
	fmt.Printf("d is not in items")
}
```


添加关键字，表示for循环全部遍历完了，没有通过break跳出。备选关键字：
- afterall
- final
- notbreak
- else (python)
- ...
```
var items = []string{"a", "b", "c"}

// is "d" in items?
for _, j := range items {
	if "d" == j {
		fmt.Printf("d is in items")
	}
} afterall {
	fmt.Printf("d is not in items")
}
```



