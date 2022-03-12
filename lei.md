# 类

{% embed url="https://docs.python.org/zh-cn/3/tutorial/classes.html#class-objects" %}

### 一个类不自带任何参数 `class Person(）`

#### 我想通过这个类初始化一个实例

* 在这个类的外面，`tom = Person()`

#### 实例调用类中的方法

`tom.f()`

### 修改类中`i`的值

```python
class MyClass:
    """A simple example class"""
    i = 12345

    def f(self):
        return 'hello world'
```

#### python修改类属性`i`

<mark style="color:red;">**在类的外面**</mark>

```python
MyClass.i = 9897
print(MyClass.i)
>>9897
```

### `_init_`到底是什么意思？

我觉得ta就是构造函数的意思，假设现在有一个`_init_()`,它里面的参数应该是什么样的？里面的参数是实例的参数。

```python
class Person():
    def __init__(self,color,height):
        self.c = color
        self.h = height
zhangyimeng = Person(987,160)
print(zhangyimeng.c)
print(zhangyimeng.h)
>>987
>>160
```

#### 一个问题：\_init\_的参数类型如何设置？换句话说：函数的参数如何指定？
