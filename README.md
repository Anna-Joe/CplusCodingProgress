## 第一阶段 C++Primer 5th 学习笔记
[unsigned与signed](#unsigned与signed)    
[变量](#变量)   
[复合类型](#复合类型)   
[const限定符](#const限定符)   
[](#)   
[](#)   
### unsigned与signed
C++的基本数据类型：字符、布尔、整型、浮点    
- 字符型：位数与机器数相同
- 布尔型：0值为False，其他值为True      
- 整型：short《=int 《=long《=long long     
- 浮点型：float double
#### 除了布尔类型之外都有有符号类型和无符号类型的区别。
有符号型（默认）：有符号位，数字只占2^(该基本数据类型所占位数-1)位     
无符号型：没有符号位，数字占2^(该基本数据类型所占位数)位    
尤其要注意无符号型和有符号型的混合运算，会先把有符号型转化为无符号型，再进行计算。    

### 变量   
变量定义：类型说明符 变量名列表    
- 初始化和赋值：两个过程    
初始化是创建变量时赋予一个初始值。赋值是擦除当前的值，用新值代替。    
- 声明和定义   
声明使得名字为程序所知。定义负责创建与名字有关的实体。 
```c++
extern int i;//声明i
int i;//声明并定义i
extern int pi=3.1415926;//定义i
```

### 复合类型
- 指针   
指向某个对象的对象。   
 1.指针本身就是一个对象，允许对指针赋值和拷贝，并且在指针的生命周期内它可以指向不同的对象。   
 2.指针无须在定义时赋值。（如果没有赋值，就跟其他对象一样，指向一个不确定的值。）
 **建议初始化所有指针**

- void* 指针
一种特殊类型的指针，可以存放任意对象的地址。   
用法：拿它跟别的对象比较/作为函数的输入或输出/或者赋给另一个void* 指针。   
**不能直接操作void* 指针所指向的对象，因为不知道它所指向的类型。**    
 
- 引用（左值引用）   
某个对象的别名。（不存放对象）   
> 定义引用时，程序把引用和他的初始值绑定在一起，而不是将初始值拷贝给引用。一旦初始化完成，引用将和它的初始值对象一直绑定在一起。因为无法令引用绑定到另一个对象，所以引用必须初始化。   
**引用不可以指向引用**

**有指向指针的引用，没有指向引用的指针。（指针只能指向对象，引用不是对象）**

### const限定符

## 第二阶段 （浙大翁恺老师）C++视频课+github笔记 查缺补漏

## 第三阶段 （陈越版本）数据结构

 [是否使用typedef定义结构体的区别](https://github.com/Anna-Joe/CplusCodingProgress/blob/master/%E6%98%AF%E5%90%A6%E4%BD%BF%E7%94%A8typedef%E5%AE%9A%E4%B9%89%E7%BB%93%E6%9E%84%E4%BD%93%E7%9A%84%E5%8C%BA%E5%88%AB.md)

 [关于树形结构的小结](https://github.com/Anna-Joe/CplusCodingProgress/blob/master/%E5%85%B3%E4%BA%8E%E6%A0%91%E5%BD%A2%E7%BB%93%E6%9E%84%E7%9A%84%E5%B0%8F%E7%BB%93.md)
