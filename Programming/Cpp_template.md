# C++ Template

C++ 模板，是一种实现泛类型的解决方案，广泛用于 STL（Standard Template Library）库中。常见的定义式如下：
```cpp
map<_T1, _T2> map_name;

map<int, char> mymap1;
map<int, bool> mymap2;
```

C+＋的模板机制，其实就是编译器根据代码情况生成了对应类的代码，相当于复制、粘贴了类模板的代码，并替换了参数类型。

比如说上述例子中就有可能生成了如下两个类：
```cpp
class map_int_char {
    char get(int);
    ...
}

class map_int_bool {
    bool get(int);
    ...
}
```
这虽然巧妙地实现了泛类型，提高了程序员的开发效率，但是编译器的实现变得非常复杂。模板的展开会生成大量重复代码，导致最终的二进制文件膨胀和编译缓慢，并且需要链接器来解决代码重复的问题。