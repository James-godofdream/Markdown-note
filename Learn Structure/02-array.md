# 数组与字符串
## C语言定义数组
### int array[N] 或 int *arrray=malloc()
### 对数组求值后返回地址
### *（array+0) == array[0] 后面array为指针
---
## C++定于数组
### int array[] 或 int *array = new int[]
### 释放内存为 delete
### C++ 另外提供STL: vector
## 运算符重载打印数组
### {
    ostream& operator << (ostream& o, const vector<int>& a){
        o << "[";
        for(auto x:a)
            o<<x <<",">;
        o << "]";
        return o;
    }
}

---
## Java定义数组
### Java只有引用型
### int[] array = new int[N]
{

    int array[] = new int[10];
    int [] array = new int[10];
    array[1] = 111;
    array[2] = 222;

    System.out.println(array);           一种定义数组的方法
    System.out.println(array.length);
}
### 还可以使用容器类：ArrayList
{

    ArrayList<Integer> al = new ArrayList<>();
    al.add(123);
    al.add(456);
    System.out.println(al);    
}

---
# 数组元素的查找
### 常见操作：查找、插入、删除
### 查找包括
### 找x的序号/是否包含x
### 找第K个元素
### 找max/min
### 统计个数    
---
# 二维数组如何定义与使用
## C语言定义二维数组 
## int array[N][M] 
## int** pa 不能表示二维数组，内存结构不同
## 使用数组名赋值指针的写法为int(*p)[M]
## 则可以 p = array;
---
# Java中如何使用二维数组
## int[][] array = new int [N][M];
## array[0] = new int[n];
---
# 字符串
## C语言使用
### char *str = "abc";
## C++ 使用
### char *str = "abc";
### string str;
### str = "abc";
## Java 使用
### String str;
### str = "abc";
### str = str + ", China"; // str = "abc, China";
# 字符串的常用操作
## 比较、拼接、复制
## 子串：截取、查找（定位）、替换、计数
## 匹配
## C语言：
### include<string.h>
### strcmp()比较
### strcpy()复制
### strcat()连接
### strstr()查找子串
### 其他通过字符数组来操作
## 正则表达式
### a 匹配a
### a|b 匹配 a或b
### [abc] 可以是a、b、c
### a-z  a到z都行
### a+ 至少有一个a，可以有多个a
### [a-z0-9]