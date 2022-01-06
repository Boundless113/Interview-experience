# C++

## 面向对象

## 部分关键字
### static
### extern
### const

## 模版

## C++11的新特性

1. auto简化声明，实现自动类型推断。常用例如vector迭代器 类型直接用auto。不能用于函数形参以及数组类型。
2. nullptr代替NULL，用于区分0和NULL。类型为 nullptr_t，能够隐式的转换为任何指针或成员指针的类型。
3. decltype用于推导表达式的类型（但不计算）。作为函数返回值时比较麻烦，后来在C++14里面可以直接用auto作为返回值。
4. 区间迭代，类似python，用冒号：
```c++
for(auto &i : arr) {    
    std::cout << i << std::endl;
}
```
5. 初始化列表，等号可加可不加；对象的构造函数直接用列表初始化
```c++
int x = {5};
double y {2.75};
short quar[5] {1, 2, 3, 4, 5};
int * ar = new int [4] {2, 3, 4, 5};
class Stump {

private:

            int roots;

            double weight;

public:

            Stump(int r, double w) : roots(r), weight(w) {}

};
Stump s1(3, 15.6);
Stump s2{5, 43.4};
Stump s3 = {4, 32.1}；
```
6. 正则表达式
