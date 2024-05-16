# Go 模块中的 “!”

Go 语言利用文件系统来读取 modules（模块）。

但是，有的文件系统不区分大小写（比如 win 和 macOS ，它们无法区分 `rsc.io/QUOTE` 和 `rsc.io/quote`）。

所以，Go 决定在小写字母之前使用 `!` 来表示大写字母，比如说：

```
Azure  ->  !azure
CATS   ->  !c!a!t!s
```

*tips：这与盲文当中的 shift 符号有些相像。*

*注：因为 Go 模块名不允许使用`!`符号，所以不会弄混。*